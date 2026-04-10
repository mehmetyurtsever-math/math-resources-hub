---
layout: default
title: Logic and Proofs (Mantık ve İspatlar)
---

# ⊢ Logic and Proofs (Mantık ve İspatlar)

Matematiksel düşüncenin temeli: önerme mantığı, küme teorisi, ispat teknikleri ve sayılabilirlik teorisi.

---

## Quick Overview

- [Book of Proof — Richard Hammack (Ücretsiz PDF)](https://www.people.vcu.edu/~rhammack/BookOfProof/)
- [MIT 6.042J — Mathematics for Computer Science](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2010/)
- [Proof Wiki](https://proofwiki.org/)

## Core Concepts


### Temel Kavramlar

#### Önerme Mantığı
- **Önerme:** Doğru ya da yanlış olabilen ifade.
- **Bağlaçlar:** $\neg$ (değil), $\wedge$ (ve), $\vee$ (veya), $\Rightarrow$ (ise), $\Leftrightarrow$ (ancak ve ancak ise).
- **Doğruluk Tablosu:** Bileşik önermelerin doğruluk değerleri.
- **Totoloji ve Çelişki:** Her yorumda doğru / her yorumda yanlış.
- **Mantıksal Denklik:** $P \equiv Q$ — aynı doğruluk tablosuna sahip.

#### Yüklem Mantığı
- **Niceleyiciler:** $\forall$ (tüm), $\exists$ (bazı), $\exists!$ (tek).
- **Değilleme:** $\neg(\forall x, P(x)) \equiv \exists x, \neg P(x)$.
- **İspat:** Bir önermenin aksiyomlardan mantıksal olarak türetilmesi.

#### İspat Teknikleri
- **Doğrudan İspat:** $P \Rightarrow Q$'yu doğrudan göster.
- **Çelişki ile İspat (Reductio ad Absurdum):** $\neg Q$ varsay, çelişki elde et.
- **Karşıt Önerme:** $\neg Q \Rightarrow \neg P$ ispat et.
- **Tümevarım (İnduction):** Taban durumu + tümevarım adımı.
  - Güçlü tümevarım: $k \leq n$ varsay, $n+1$ için göster.
- **Varoluş İspatı:** Yapıcı (construct) ve yapıcı olmayan (non-constructive).
- **Örnekle çürütme (Counterexample):** Evrensel önermeyi yanlışla.

#### Küme Teorisi
- **Küme Aksiyomları (ZFC):** Zermelo-Fraenkel aksiyomları + Seçim Aksiyomu.
- **İşlemler:** $A \cup B$, $A \cap B$, $A \setminus B$, $A^c$, $\mathcal{P}(A)$.
- **Fonksiyonlar:** İnjektif (birebir), sürjektif (örten), bijektif.
- **Kardinalite:** $|A| = |B| \iff \exists$ bijeksiyon $f: A \to B$.

#### Sayılabilirlik
- **Sayılabilir Kümeler:** $\mathbb{N}, \mathbb{Z}, \mathbb{Q}$ sayılabilir.
- **Sayılamaz Kümeler:** $\mathbb{R}$, Cantor köşegen argümanı.
- **Cantor Teoremi:** $|A| < |\mathcal{P}(A)|$ her küme için.
- **Schroeder-Bernstein:** $|A| \leq |B|$ ve $|B| \leq |A| \Rightarrow |A| = |B|$.


## Recommended Books


### Başlangıç Seviyesi

- **Daniel Velleman** — *How to Prove It*
  - İspat yazımının nasıl yapıldığını öğretir, başlangıç için en iyi seçim.
  - Zorluk: ★★☆☆☆ | Dil: İngilizce

- **Book of Proof** — *Richard Hammack* (Ücretsiz PDF)
  - Açık erişim, kapsamlı ve anlaşılır. [bookofproof.com](https://www.people.vcu.edu/~rhammack/BookOfProof/)
  - Zorluk: ★★☆☆☆ | Dil: İngilizce

- **Polya** — *How to Solve It*
  - Problem çözme stratejileri, klasik rehber.
  - Zorluk: ★★☆☆☆ | Dil: İngilizce

### İleri Seviye

- **Enderton** — *A Mathematical Introduction to Logic*
  - Formel mantık, tamlık teoremi, karar verilemezlik.
  - Zorluk: ★★★★☆ | Dil: İngilizce

- **Halmos** — *Naive Set Theory*
  - Akıcı ve öz, küme teorisinin temelleri.
  - Zorluk: ★★★☆☆ | Dil: İngilizce

- **Jech** — *Set Theory*
  - Büyük kardinallar dahil kapsamlı referans.
  - Zorluk: ★★★★★ | Dil: İngilizce


## Web Resources


### Ücretsiz Kaynaklar

- [Book of Proof (Ücretsiz PDF)](https://www.people.vcu.edu/~rhammack/BookOfProof/) — Hammack'ın açık erişim kitabı
- [Mathematical Reasoning — Rinker](https://math.libretexts.org/) — LibreTexts matematik kütüphanesi
- [Proof Wiki](https://proofwiki.org/) — İspatlar wiki'si

### Problem Setleri

- [Putnam Archive](https://kskedlaya.org/putnam-archive/) — Olimpiyat seviyesi ispat problemleri
- [Math StackExchange — Proof Writing](https://math.stackexchange.com/questions/tagged/proof-writing)


## Video Lectures


### Üniversite Dersleri

- [MIT 6.042J — Mathematics for Computer Science](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2010/) — Mantık, kümeler, indüksiyon
- [Harvard — Sets, Counting and Probability](https://online-learning.harvard.edu/)

### YouTube Kanalları

- [Trefor Bazett — Proof Techniques](https://www.youtube.com/@DrTreforBazett) — İspat yöntemleri serisi
- [Logic & Proof — Lara Alcock](https://www.youtube.com/results?search_query=lara+alcock+proof) — İspat okuma ve yazma
- [Michael Penn — Proof Videos](https://www.youtube.com/@michaelpennmath) — Günlük ispat videolar


---

[← Group Theory]({{ '/group-theory/' | relative_url }}) | [Ana Sayfa]({{ '/' | relative_url }}) | [Galois Theory →]({{ '/galois-theory/' | relative_url }})
