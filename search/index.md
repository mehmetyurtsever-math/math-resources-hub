---
layout: default
title: Search
permalink: /search/
---

<h1>Search Results</h1>

<div id="search-container">
  <p id="search-summary" class="search-summary"></p>
  <ul id="search-results" class="search-results-list"></ul>
  <p id="search-empty" class="search-empty"></p>
</div>

<script>
(function () {
  var INDEX_URL = '{{ "/search.json" | relative_url }}';

  function normalize(str) {
    return str.normalize('NFD').replace(/[\u0300-\u036f]/g, '').toLocaleLowerCase('tr-TR');
  }

  function getQuery() {
    try {
      return new URLSearchParams(window.location.search).get('q') || '';
    } catch (e) {
      var m = window.location.search.match(/[?&]q=([^&]*)/);
      return m ? decodeURIComponent(m[1].replace(/\+/g, ' ')) : '';
    }
  }

  function escapeHtml(str) {
    return String(str)
      .replace(/&/g, '&amp;')
      .replace(/</g, '&lt;')
      .replace(/>/g, '&gt;')
      .replace(/"/g, '&quot;');
  }

  function getSnippet(content, query) {
    var normContent = normalize(content);
    var normQuery = normalize(query);
    var normIdx = normContent.indexOf(normQuery);
    if (normIdx === -1) return escapeHtml(content.substring(0, 160)) + '&hellip;';
    // Map normalized index to original content index.
    // Combining characters (length 0 after normalization) are skipped so we
    // always land on a visible base character, handling both precomposed and
    // NFD-decomposed source text correctly.
    var normPos = 0;
    var origStart = 0;
    for (var i = 0; i < content.length; i++) {
      var nc = normalize(content[i]);
      if (normPos >= normIdx && nc.length > 0) { origStart = i; break; }
      normPos += nc.length;
    }
    // Advance through original content until normQuery.length normalized chars consumed.
    var origEnd = origStart;
    var charsLeft = normQuery.length;
    for (var j = origStart; j < content.length && charsLeft > 0; j++) {
      charsLeft -= normalize(content[j]).length;
      origEnd = j + 1;
    }
    var start = Math.max(0, origStart - 60);
    var end = Math.min(content.length, origEnd + 100);
    var snippet = (start > 0 ? '&hellip;' : '') +
      escapeHtml(content.substring(start, origStart)) +
      '<mark class="search-highlight">' + escapeHtml(content.substring(origStart, origEnd)) + '</mark>' +
      escapeHtml(content.substring(origEnd, end)) +
      (end < content.length ? '&hellip;' : '');
    return snippet;
  }

  function fetchIndex(callback) {
    var xhr = new XMLHttpRequest();
    xhr.open('GET', INDEX_URL);
    xhr.onload = function () {
      if (xhr.status === 200) {
        try { callback(JSON.parse(xhr.responseText)); }
        catch (e) { callback([]); }
      } else {
        callback([]);
      }
    };
    xhr.onerror = function () { callback([]); };
    xhr.send();
  }

  function search(index, query) {
    var normQ = normalize(query);
    var results = [];
    index.forEach(function (item) {
      var normTitle = normalize(item.title || '');
      var normContent = normalize(item.content || '');
      var titleMatch = normTitle.indexOf(normQ) !== -1;
      var contentMatch = normContent.indexOf(normQ) !== -1;
      if (titleMatch || contentMatch) {
        results.push({ item: item, score: titleMatch ? 2 : 1 });
      }
    });
    results.sort(function (a, b) { return b.score - a.score; });
    return results;
  }

  function render(results, query) {
    var summary = document.getElementById('search-summary');
    var list = document.getElementById('search-results');
    var empty = document.getElementById('search-empty');

    if (!query) {
      summary.textContent = '';
      list.innerHTML = '';
      empty.style.display = '';
      empty.textContent = 'Enter a search term in the header search box and press Enter.';
      return;
    }

    if (results.length === 0) {
      summary.textContent = '';
      list.innerHTML = '';
      empty.style.display = '';
      empty.innerHTML = 'No results found for <strong>' + escapeHtml(query) + '</strong>. Try a different search term.';
      return;
    }

    empty.style.display = 'none';
    summary.textContent = results.length + ' result' + (results.length === 1 ? '' : 's') + ' for \u2018' + query + '\u2019';

    list.innerHTML = results.map(function (r) {
      var item = r.item;
      var snippet = getSnippet(item.content || '', query);
      return '<li class="search-result-item">' +
        '<a class="search-result-title" href="' + escapeHtml(item.url) + '">' + escapeHtml(item.title) + '</a>' +
        '<span class="search-result-url">' + escapeHtml(item.url) + '</span>' +
        '<p class="search-result-snippet">' + snippet + '</p>' +
        '</li>';
    }).join('');
  }

  var query = getQuery();
  if (query) {
    document.getElementById('search-summary').textContent = 'Searching\u2026';
    fetchIndex(function (index) {
      render(search(index, query), query);
    });
  } else {
    render([], '');
  }
})();
</script>
