---
layout: default
title: Galois Theory (Galois Teorisi)
---

# 𝔾 Galois Theory (Galois Teorisi)

Évariste Galois'nın polinom denklemlerin çözülebilirliğini cisim uzantıları ve grup teorisiyle ilişkilendiren devrimci teorisi.

---

## Quick Overview

- [James Milne — Fields and Galois Theory (PDF)](https://www.jmilne.org/math/CourseNotes/FT.pdf)
- [Keith Conrad — Galois Theory Notes](https://kconrad.math.uconn.edu/blurbs/)
- [MIT 18.702 — Algebra II](https://ocw.mit.edu/courses/18-702-algebra-ii-spring-2011/)

## Core Concepts


### Temel Kavramlar

#### Cisim Uzantıları
- **Cisim Uzantısı:** $F \subseteq K$ — $K$, $F$ üzerinde vektör uzayı.
- **Derece:** $[K:F] = \dim_F K$.
- **Basit Uzantı:** $K = F(\alpha)$ — tek eleman ekleyerek elde edilir.
- **Cebirsel Eleman:** $\alpha \in K$, $F$ üzerinde bir polinomun kökü.
- **Minimal Polinom:** $\alpha$'nın $F$'e göre minimal polinomu, irredüktibil.
- **Kule Yasası:** $[K:F] = [K:E][E:F]$ ($F \subseteq E \subseteq K$).

#### Bölüm Cisimleri
- **Bölüm Cismi $F(\alpha)$:** $F[x]/\langle p(x) \rangle$ — $p(x)$ irredüktibil polinomun bölüm halkası.
- **Splitting Field (Ayrışım Cismi):** Bir polinomun tüm köklerini içeren en küçük cisim uzantısı.
- **Cebirsel Kapanış:** Her polinom köke sahip olan cisim uzantısı $\overline{F}$.

#### Galois Grubu
- **Galois Grubu:** $\text{Gal}(K/F)$ — $F$'i sabit tutan $K \to K$ otomorfizmaları.
- **Galois Uzantısı:** Normal ve separable cisim uzantısı; $|\text{Gal}(K/F)| = [K:F]$.
- **Fundamental Teorem:** Alt gruplar $\leftrightarrow$ Ara cisimler arasında bire-bir Galois yazışması.

#### Çözülebilirlik
- **Çözülebilir Grup:** Subnormal serisi abelyan bölümlerle sonlanan grup.
- **Abel Teoremi:** Genel 5. ve üzeri dereceli denklemler kök radikalleri ile çözülemez.
- **Galois Kriteri:** $f(x)$ kök radikalleriyle çözülebilir $\iff$ $\text{Gal}(K/F)$ çözülebilir.

### Örnekler

- $\text{Gal}(\mathbb{Q}(\sqrt{2})/\mathbb{Q}) \cong \mathbb{Z}_2$.
- $\text{Gal}(\mathbb{Q}(\zeta_n)/\mathbb{Q}) \cong (\mathbb{Z}/n\mathbb{Z})^*$ — devirli cisim uzantıları.
- $x^4 - 2$ polinomunun ayrışım cismi ve Galois grubu $D_4$.


## Recommended Books


### Başlangıç Seviyesi

- **Ian Stewart** — *Galois Theory* (4. baskı)
  - Tarihsel perspektif, erişilebilir anlatım.
  - Zorluk: ★★★☆☆ | Dil: İngilizce

- **Artin** — *Algebra* (Galois Theory bölümleri)
  - Sıkı ve öz klasik kaynak.
  - Zorluk: ★★★☆☆ | Dil: İngilizce

- **Cox** — *Galois Theory*
  - Bol örnek, tarihsel bağlam, çözülebilirlik.
  - Zorluk: ★★★☆☆ | Dil: İngilizce

### İleri Seviye

- **Lang** — *Algebra* (Cisim teorisi bölümleri)
  - Kapsamlı ve kategorik yaklaşım.
  - Zorluk: ★★★★★ | Dil: İngilizce

- **Milne** — *Fields and Galois Theory* (Ücretsiz)
  - [math.jmilne.org](https://www.jmilne.org/math/) üzerinden ücretsiz.
  - Zorluk: ★★★★☆ | Dil: İngilizce


## Web Resources


### Ücretsiz Kaynaklar

- [James Milne — Fields and Galois Theory (PDF)](https://www.jmilne.org/math/CourseNotes/FT.pdf) — Ücretsiz ders notları
- [Keith Conrad — Galois Theory Notes](https://kconrad.math.uconn.edu/blurbs/) — Detaylı açıklayıcı makaleler
- [Galois Theory — Wikipedia](https://en.wikipedia.org/wiki/Galois_theory) — Genel bakış

### Problem Setleri

- [Algebra Qualifying Exams — Field Theory](https://math.stackexchange.com/questions/tagged/galois-theory)
- [MIT 18.702 — Problem Sets](https://ocw.mit.edu/courses/18-702-algebra-ii-spring-2011/pages/assignments/)


## Video Lectures


### Üniversite Dersleri

- [MIT 18.702 — Algebra II](https://ocw.mit.edu/courses/18-702-algebra-ii-spring-2011/) — Galois teorisi dahil cebir II dersi
- [Fields and Galois Theory — YouTube](https://www.youtube.com/results?search_query=galois+theory+lecture) — Çeşitli üniversite dersleri

### YouTube Kanalları

- [Richard Borcherds — Galois Theory](https://www.youtube.com/@RichardBorcherds) — Derinlemesine Galois teorisi
- [Mathador](https://www.youtube.com/results?search_query=galois+theory) — Türkçe ve İngilizce kaynaklar
- [Socratica](https://www.youtube.com/@Socratica) — Cisim teorisi temelleri


---

[← Logic & Proofs]({{ '/logic-and-proofs/' | relative_url }}) | [Ana Sayfa]({{ '/' | relative_url }}) | [Commutative Algebra →]({{ '/commutative-algebra/' | relative_url }})
