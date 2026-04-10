---
layout: default
title: Analysis (Analiz)
---

# ∫ Analysis (Analiz)

Gerçel ve karmaşık sayılar üzerinde fonksiyonların davranışını, limit, süreklilik, türev ve integral kavramlarını inceleyen matematik dalı.

---

## Quick Overview

Bu sayfa Analysis konusundaki temel kaynakları tek yerde toplar.

- [MIT 18.100A — Real Analysis](https://ocw.mit.edu/courses/18-100a-real-analysis-fall-2020/)
- [Paul's Online Math Notes](https://tutorial.math.lamar.edu/)
- [Khan Academy — Calculus](https://www.khanacademy.org/math/calculus-1)

## Core Concepts


### Temel Kavramlar

#### Sayı Sistemleri ve Tamamlılık
- **Gerçel Sayılar (ℝ):** Tam sayılar, rasyonel ve irrasyonel sayıların birleşimi. Tamamlılık aksiyomu: Her üstten sınırlı boş olmayan alt kümenin bir üstten sınırı (supremum) vardır.
- **Supremum ve İnfimum:** $\sup A$ ve $\inf A$ tanımları, varlık ve teklik.
- **Arşimet Özelliği:** $\forall x \in \mathbb{R},\ \exists n \in \mathbb{N}$ öyle ki $n > x$.

#### Diziler ve Limitler
- **Dizi Tanımı:** $a: \mathbb{N} \to \mathbb{R}$ fonksiyonu; $(a_n)_{n=1}^{\infty}$.
- **Limit:** $\lim_{n \to \infty} a_n = L \iff \forall \varepsilon > 0,\ \exists N \in \mathbb{N}:\ n \geq N \Rightarrow |a_n - L| < \varepsilon$.
- **Cauchy Dizisi:** $(a_n)$ Cauchy $\iff \forall \varepsilon > 0,\ \exists N:\ m,n \geq N \Rightarrow |a_m - a_n| < \varepsilon$.
- **Teorem:** ℝ'de her Cauchy dizisi yakınsar.

#### Süreklilik
- **Nokta Süreklilik:** $f$, $c$'de sürekli $\iff \lim_{x \to c} f(x) = f(c)$.
- **$\varepsilon$–$\delta$ Tanımı:** $\forall \varepsilon > 0,\ \exists \delta > 0:\ |x-c| < \delta \Rightarrow |f(x)-f(c)| < \varepsilon$.
- **Düzgün Süreklilik:** $\delta$, $c$'den bağımsız seçilebilir.
- **Teorem (Ara Değer):** $f:[a,b]\to\mathbb{R}$ sürekli ve $f(a) < 0 < f(b)$ ise $\exists c \in (a,b):\ f(c) = 0$.

#### Türev
- **Tanım:** $f'(c) = \lim_{h \to 0} \dfrac{f(c+h)-f(c)}{h}$.
- **Türev Kuralları:** Toplam, çarpım, bölüm, zincir kuralları.
- **Ortalama Değer Teoremi:** $f:[a,b]\to\mathbb{R}$ sürekli, $(a,b)$'de türevlenebilir ise $\exists c \in (a,b):\ f'(c) = \dfrac{f(b)-f(a)}{b-a}$.
- **L'Hôpital Kuralı:** $\frac{0}{0}$ ya da $\frac{\infty}{\infty}$ belirsizliklerini çözmek için.

#### Riemann İntegrali
- **Tanım:** Alt ve üst Riemann toplamları, $\underline{S}(f,P)$ ve $\overline{S}(f,P)$.
- **Riemann İntegrallenebilirlik:** $\inf_P \overline{S}(f,P) = \sup_P \underline{S}(f,P)$.
- **Newton-Leibniz Teoremi:** $F'(x) = f(x)$ ise $\int_a^b f(x)\,dx = F(b) - F(a)$.

### Metrik Uzaylar

- **Metrik Uzay:** $(X, d)$ — $d: X \times X \to [0,\infty)$ metrik aksiyomlarını sağlar.
- **Açık ve Kapalı Kümeler**, **İç Nokta**, **Birikim Noktası**.
- **Tamlık:** Her Cauchy dizisinin yakınsadığı metrik uzaylar.
- **Kompaktlık:** Her açık örtünün sonlu bir alt örtüsü var ise kompakttır.
- **Teorem (Heine-Borel):** $\mathbb{R}^n$'de kompaktlık $\iff$ kapalılık ve sınırlılık.

### İspatlar

- **Squeeze Theorem:** $a_n \leq b_n \leq c_n$ ve $a_n, c_n \to L$ ise $b_n \to L$.
- **Bolzano-Weierstrass:** Her sınırlı dizi yakınsak bir alt dizi içerir.
- **Taylor Serisi:** $f(x) = \sum_{n=0}^{\infty} \dfrac{f^{(n)}(a)}{n!}(x-a)^n$ — yakınsaklık koşulları.


## Recommended Books


### Başlangıç Seviyesi

- **Walter Rudin** — *Principles of Mathematical Analysis* (Baby Rudin)
  - Klasik referans, sıkı ve öz yazım. Metrik uzaylar, diziler, türev ve integral.
  - Zorluk: ★★★★☆ | Dil: İngilizce

- **Tom Apostol** — *Mathematical Analysis*
  - Rudin'den biraz daha açıklayıcı, tarihsel notlar içerir.
  - Zorluk: ★★★★☆ | Dil: İngilizce

- **Charles Pugh** — *Real Mathematical Analysis*
  - Görsel açıklamalar ve çok sayıda örnek. Başlangıç için ideal.
  - Zorluk: ★★★☆☆ | Dil: İngilizce

- **Serge Lang** — *Undergraduate Analysis*
  - Geniş kapsam, lisans seviyesi için uygun.
  - Zorluk: ★★★☆☆ | Dil: İngilizce

### İleri Seviye

- **Walter Rudin** — *Real and Complex Analysis* (Big Rudin)
  - Measure teorisi, $L^p$ uzayları, Fourier analizi.
  - Zorluk: ★★★★★ | Dil: İngilizce

- **Gerald Folland** — *Real Analysis: Modern Techniques and Their Applications*
  - Uygulamalı perspektif, kapsamlı measure teorisi.
  - Zorluk: ★★★★☆ | Dil: İngilizce

- **Elias Stein & Rami Shakarchi** — *Princeton Lectures in Analysis* (4 cilt)
  - Fourier analizi, karmaşık analiz, gerçel analiz, fonksiyonel analiz.
  - Zorluk: ★★★★☆ | Dil: İngilizce

### Türkçe Kaynaklar

- **Ahmet Okay Çelebi** — *Analiz I–II*
  - Türk üniversitelerinde yaygın kullanılan kapsamlı ders kitabı.


## Web Resources


### İnteraktif Kaynaklar

- [Khan Academy — Calculus](https://www.khanacademy.org/math/calculus-1) — Sezgisel açıklamalar, alıştırmalar
- [Paul's Online Math Notes](https://tutorial.math.lamar.edu/) — Detaylı ders notları ve örnekler
- [Brilliant.org — Real Analysis](https://brilliant.org/courses/real-analysis/) — İnteraktif alıştırmalar
- [3Blue1Brown — Essence of Calculus](https://www.3blue1brown.com/topics/calculus) — Geometrik sezgi videoları

### Problem Setleri

- [Art of Problem Solving](https://artofproblemsolving.com/) — Olimpiyat ve ileri matematik problemleri
- [Project Euler](https://projecteuler.net/) — Analitik düşünce gerektiren hesaplamalı problemler
- [MIT OpenCourseWare — Problem Sets](https://ocw.mit.edu/courses/18-100a-real-analysis-fall-2020/) — Ödev ve sınav soruları

### Ansiklopedi ve Referans

- [ProofWiki](https://proofwiki.org/) — Teoremler ve ispatlar wiki'si
- [Encyclopedia of Mathematics](https://encyclopediaofmath.org/) — Matematik ansiklopedisi
- [MathWorld — Analysis](https://mathworld.wolfram.com/analysis.html) — Wolfram kapsamlı referans


## Video Lectures


### Üniversite Dersleri

- [MIT 18.100A — Real Analysis (2020)](https://ocw.mit.edu/courses/18-100a-real-analysis-fall-2020/) — Casey Rodriguez, tam ders videoları
- [MIT 18.100B — Real Analysis](https://ocw.mit.edu/courses/18-100b-analysis-i-fall-2010/) — Klasik versiyon, notlar ve problemler
- [Harvard Math 55a](https://people.math.harvard.edu/~ctm/home/text/class/harvard/55a/08/html/index.html) — Yoğun lisans analiz dersi

### YouTube Kanalları

- [3Blue1Brown](https://www.youtube.com/@3blue1brown) — Matematiksel sezgi ve görselleştirme
- [Professor Leonard](https://www.youtube.com/@ProfessorLeonard) — Kapsamlı Calculus serisi, açıklayıcı anlatım
- [The Bright Side of Mathematics](https://www.youtube.com/@brightsideofmaths) — Real Analysis playlist
- [MathMajor](https://www.youtube.com/@mathmajor) — Lisans seviyesi analiz dersleri
- [Dr. Peyam](https://www.youtube.com/@drpeyam) — Analiz problemleri ve çözümleri

### Türkçe Video Kaynaklar

- [Türkiye Bilimler Akademisi — Matematik](https://www.youtube.com/@TUBA_Turkiye) — Türkçe matematik dersleri
- [YTÜ Uzaktan Eğitim](https://www.youtube.com/@ytuuzaktanegitim) — Üniversite seviyesi Türkçe dersler


---

[← Ana Sayfa]({{ '/' | relative_url }}) | [Linear Algebra →]({{ '/linear-algebra/' | relative_url }})
