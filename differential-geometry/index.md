---
layout: default
title: Differential Geometry (Diferansiyel Geometri)
---

# 𝜅 Differential Geometry (Diferansiyel Geometri)

Calculus araçlarıyla eğriler, yüzeyler ve manifoldların geometrisini inceleyen matematik dalı. Genel görelilik teorisinin matematiksel dili.

---

<details>
<summary>📖 Ders Notları</summary>
<div class="details-body">

### Temel Kavramlar

#### Eğriler
- **Parametrik Eğri:** $\alpha: I \to \mathbb{R}^3$, $\alpha(t) = (x(t), y(t), z(t))$.
- **Birim Hız Eğrisi:** $|\alpha'(t)| = 1$ — yay uzunluğuyla parametreleme.
- **Eğrilik:** $\kappa(t) = |\alpha''(t)|$ — eğrinin nasıl büküldüğü.
- **Burulma:** $\tau(t)$ — eğrinin uzay içinde nasıl döndüğü.
- **Frenet-Serret Çerçevesi:** $\{T, N, B\}$ — teğet, normal, binormal.
- **Frenet-Serret Formülleri:** $T' = \kappa N$, $N' = -\kappa T + \tau B$, $B' = -\tau N$.

#### Yüzeyler
- **Düzenli Yüzey:** $\sigma: U \subseteq \mathbb{R}^2 \to \mathbb{R}^3$, $\text{rank}\, d\sigma_p = 2$.
- **Birinci Temel Form:** $I = E\,du^2 + 2F\,du\,dv + G\,dv^2$ — yüzey metriği.
- **Alan Hesabı:** $A = \iint_U \sqrt{EG - F^2}\,du\,dv$.
- **İkinci Temel Form:** $II = L\,du^2 + 2M\,du\,dv + N\,dv^2$ — eğriliği ölçer.
- **Ortalama Eğrilik:** $H = \dfrac{EN - 2FM + GL}{2(EG-F^2)}$.
- **Gaussian Eğrilik:** $K = \dfrac{LN - M^2}{EG - F^2}$.

#### Gauss-Bonnet Teoremi
- **Gauss'un Egregium Teoremi:** $K$ içsel büyüklüktür — yüzeyden bağımsız hesaplanır.
- **Gauss-Bonnet:** $\iint_M K\,dA + \oint_{\partial M} \kappa_g\,ds = 2\pi\chi(M)$.
- **Euler Karakteristiği:** $\chi(M) = V - E + F$ (köşe — kenar — yüz).

#### Manifoldlar
- **Pürüzsüz Manifold:** Yerel olarak $\mathbb{R}^n$'e benzeyen küme, açık örtü ile atlas.
- **Teğet Uzayı $T_pM$:** $p$ noktasındaki türevlenebilir yolların eşdeğerlik sınıfları.
- **Vektör Alanları ve Akışlar.**
- **Diferansiyel Formlar:** $1$-form, $2$-form, dış türev $d$.
- **Stokes Teoremi:** $\int_M d\omega = \int_{\partial M} \omega$.

### Bağlantı ve Eğrilik

- **Bağlantı (Connection):** Vektör alanlarının kovaryant türevi.
- **Riemann Metriği:** Her teğet uzayında iç çarpım.
- **Riemann Eğrilik Tensörü:** $R(X,Y)Z = \nabla_X\nabla_Y Z - \nabla_Y\nabla_X Z - \nabla_{[X,Y]}Z$.
- **Geodezikler:** Eğriliği sıfır olan eğriler — yüzeyde "düz çizgi" genellemesi.

</div>
</details>

<details>
<summary>📚 Kitap Önerileri</summary>
<div class="details-body">

### Başlangıç Seviyesi

- **do Carmo** — *Differential Geometry of Curves and Surfaces*
  - Klasik başlangıç kitabı, eğriler ve yüzeyler, mükemmel motivasyon.
  - Zorluk: ★★★☆☆ | Dil: İngilizce

- **Pressley** — *Elementary Differential Geometry*
  - Daha erişilebilir, bol görsel örnek.
  - Zorluk: ★★☆☆☆ | Dil: İngilizce

- **Millman & Parker** — *Elements of Differential Geometry*
  - Dengeli ve anlaşılır anlatım.
  - Zorluk: ★★★☆☆ | Dil: İngilizce

### İleri Seviye

- **do Carmo** — *Riemannian Geometry*
  - Manifoldlar, Riemann geometrisi, geodezikler.
  - Zorluk: ★★★★☆ | Dil: İngilizce

- **Lee** — *Introduction to Smooth Manifolds*
  - Kapsamlı ve modern referans, pürüzsüz manifoldlar.
  - Zorluk: ★★★★☆ | Dil: İngilizce

- **Spivak** — *A Comprehensive Introduction to Differential Geometry* (5 cilt)
  - Eşsiz kapsamlılık, tarihsel notlar.
  - Zorluk: ★★★★★ | Dil: İngilizce

</div>
</details>

<details>
<summary>🌐 Web Siteleri ve Kaynaklar</summary>
<div class="details-body">

### İnteraktif Kaynaklar

- [Differential Geometry — Visual](https://www.geogebra.org/m/differential-geometry) — GeoGebra görselleştirmeleri
- [MIT OCW — Differential Geometry](https://ocw.mit.edu/courses/18-950-differential-geometry-fall-2008/) — Ders notları
- [The Geometry Center](https://www.geom.uiuc.edu/) — İnteraktif geometri

### Problem Setleri

- [do Carmo — Solutions](https://math.stackexchange.com/questions/tagged/differential-geometry)
- [Qualifying Exam Problems — Geometry](https://math.stackexchange.com/questions/tagged/riemannian-geometry)

</div>
</details>

<details>
<summary>🎬 Video Dersler</summary>
<div class="details-body">

### Üniversite Dersleri

- [MIT 18.950 — Differential Geometry](https://ocw.mit.edu/courses/18-950-differential-geometry-fall-2008/) — Ders notları ve ödevler
- [NPTEL — Differential Geometry](https://www.youtube.com/results?search_query=NPTEL+differential+geometry) — Kapsamlı ders serisi

### YouTube Kanalları

- [Eigenchris — Tensor Calculus](https://www.youtube.com/@eigenchris) — Tensörler ve Riemann geometrisi
- [XylyXylyX — Differential Geometry](https://www.youtube.com/@XylyXylyX) — Manifoldlar ve formlar
- [Michael Penn](https://www.youtube.com/@michaelpennmath) — Diferansiyel geometri problemleri

</div>
</details>

---

[← Complex Analysis]({{ '/complex-analysis/' | relative_url }}) | [Ana Sayfa]({{ '/' | relative_url }})
