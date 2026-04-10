---
layout: default
title: Complex Analysis (Karmaşık Analiz)
---

# ℂ Complex Analysis (Karmaşık Analiz)

Karmaşık sayılar üzerinde tanımlı fonksiyonların analizi. Fizik, mühendislik ve ileri matematiğin güçlü aracı.

---

## Quick Overview

- [MIT 18.04 — Complex Variables](https://ocw.mit.edu/courses/18-04-complex-variables-with-applications-spring-2018/)
- [3Blue1Brown — Visualizing Complex Analysis](https://www.youtube.com/watch?v=5PcpBw5Hbwo)
- [Visual Complex Analysis — Needham](https://en.wikipedia.org/wiki/Visual_Complex_Analysis)

## Core Concepts


### Temel Kavramlar

#### Karmaşık Sayılar
- **Tanım:** $\mathbb{C} = \{a + bi \mid a, b \in \mathbb{R},\ i^2 = -1\}$.
- **Modül ve Argüman:** $|z| = \sqrt{a^2+b^2}$, $\arg(z) = \arctan(b/a)$.
- **Euler Formülü:** $e^{i\theta} = \cos\theta + i\sin\theta$.
- **De Moivre:** $(r e^{i\theta})^n = r^n e^{in\theta}$.

#### Karmaşık Fonksiyonlar
- **Analitik (Holomorphic) Fonksiyon:** Her noktada karmaşık türevi olan fonksiyon.
- **Cauchy-Riemann Denklemleri:** $u_x = v_y$, $u_y = -v_x$ ($f = u + iv$).
- **Harmonik Fonksiyonlar:** $\Delta u = u_{xx} + u_{yy} = 0$.
- **Örnekler:** $e^z$, $\sin z$, $\cos z$, $\log z$, $z^n$.

#### Cauchy Teoremi ve İntegral
- **Karmaşık İntegral:** $\int_\gamma f(z)\,dz = \int_a^b f(\gamma(t))\gamma'(t)\,dt$.
- **Cauchy-Goursat Teoremi:** $f$ analitik, $\gamma$ basit kapalı $\Rightarrow \oint_\gamma f(z)\,dz = 0$.
- **Cauchy İntegral Formülü:** $f(a) = \dfrac{1}{2\pi i}\oint_\gamma \dfrac{f(z)}{z-a}\,dz$.
- **Cauchy'nin Türev Formülü:** $f^{(n)}(a) = \dfrac{n!}{2\pi i}\oint_\gamma \dfrac{f(z)}{(z-a)^{n+1}}\,dz$.

#### Laurent Serisi ve Rezidüler
- **Taylor Serisi:** Analitik fonksiyon için $f(z) = \sum_{n=0}^\infty a_n (z-a)^n$.
- **Laurent Serisi:** İzole tekillik etrafında $f(z) = \sum_{n=-\infty}^\infty a_n (z-a)^n$.
- **Tekillikler:** Kaldırılabilir, kutup (pole), esaslı tekillik.
- **Rezidü:** $\text{Res}(f, a) = a_{-1}$ — Laurent serisinin $-1$. katsayısı.
- **Rezidü Teoremi:** $\oint_\gamma f(z)\,dz = 2\pi i \sum \text{Res}(f, a_k)$.

### Uygulamalar

- **Gerçek İntegraller:** $\int_{-\infty}^\infty \frac{dx}{1+x^2} = \pi$ gibi hesaplamalar.
- **Argüman Prensibi:** $f$'nin sıfır ve kutup sayıları hakkında bilgi.
- **Rouché Teoremi:** İki fonksiyon arasındaki sıfır sayıları karşılaştırması.
- **Riemann Haritalama Teoremi:** Her basit bağlantılı bölge birim diske konform eşdeğerdir.


## Recommended Books


### Başlangıç Seviyesi

- **Brown & Churchill** — *Complex Variables and Applications*
  - Uygulamalı, mühendislik ve fizik perspektifi, bol örnek.
  - Zorluk: ★★☆☆☆ | Dil: İngilizce

- **Stein & Shakarchi** — *Complex Analysis* (Princeton Lectures II)
  - Güzel yazım, sezgi ve titizlik dengesi.
  - Zorluk: ★★★☆☆ | Dil: İngilizce

- **Needham** — *Visual Complex Analysis*
  - Eşsiz geometrik yaklaşım, görsel anlatım.
  - Zorluk: ★★★☆☆ | Dil: İngilizce

### İleri Seviye

- **Ahlfors** — *Complex Analysis*
  - Klasik referans, sıkı ve kapsamlı.
  - Zorluk: ★★★★☆ | Dil: İngilizce

- **Rudin** — *Real and Complex Analysis*
  - Gerçel ve karmaşık analizin birleşik sunumu.
  - Zorluk: ★★★★★ | Dil: İngilizce


## Web Resources


### İnteraktif Kaynaklar

- [Complex Analysis — mathlets.org](https://mathlets.org/) — MIT interaktif araçlar
- [Visual Complex Analysis — Online](https://visual.icse.us.edu.pl/) — Görsel karmaşık analiz
- [Complex Function Explorer](https://people.math.harvard.edu/~knill/teaching/math213_2017/index.html)

### Problem Setleri

- [MIT 18.04 — Complex Variables](https://ocw.mit.edu/courses/18-04-complex-variables-with-applications-spring-2018/)
- [Complex Analysis — Khan Academy](https://www.khanacademy.org/) — Temel konular


## Video Lectures


### Üniversite Dersleri

- [MIT 18.04 — Complex Variables](https://ocw.mit.edu/courses/18-04-complex-variables-with-applications-spring-2018/) — Tam ders materyali
- [NPTEL — Complex Analysis](https://www.youtube.com/results?search_query=NPTEL+complex+analysis) — Hindistan'ın açık ders sistemi

### YouTube Kanalları

- [3Blue1Brown — Visualizing Complex Analysis](https://www.youtube.com/watch?v=5PcpBw5Hbwo) — Görsel sezgi
- [The Bright Side of Mathematics — Complex Analysis](https://www.youtube.com/@brightsideofmaths) — Karmaşık analiz serisi
- [Dr. Peyam — Complex Analysis](https://www.youtube.com/@drpeyam) — Karmaşık analiz problemleri


---

[← Commutative Algebra]({{ '/commutative-algebra/' | relative_url }}) | [Ana Sayfa]({{ '/' | relative_url }}) | [Differential Geometry →]({{ '/differential-geometry/' | relative_url }})
