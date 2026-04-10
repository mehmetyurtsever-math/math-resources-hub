---
layout: default
title: Linear Algebra (Doğrusal Cebir)
---

# ⊕ Linear Algebra (Doğrusal Cebir)

Vektörler, matrisler, doğrusal dönüşümler ve vektör uzaylarını inceleyen temel matematik dalı. Mühendislik, fizik, bilgisayar bilimi ve ekonominin vazgeçilmez aracı.

---

## 📖 Ders Notları


### Temel Kavramlar

#### Vektörler ve Vektör Uzayları
- **Vektör Uzayı:** $(V, +, \cdot)$ — toplama ve skalar çarpma aksiyomlarını sağlayan yapı.
- **Alt Uzay:** $W \subseteq V$ alt uzay $\iff$ $\mathbf{0} \in W$, toplama ve skalar çarpma altında kapalı.
- **Doğrusal Bağımsızlık:** $v_1, \ldots, v_n$ bağımsız $\iff$ $c_1 v_1 + \cdots + c_n v_n = 0 \Rightarrow c_i = 0$.
- **Baz ve Boyut:** $\dim(V)$, bazın eleman sayısı. Sonlu boyutlu uzaylarda her baz aynı sayıda eleman içerir.
- **Germe (Span):** $\text{span}\{v_1,\ldots,v_k\} = \{c_1 v_1 + \cdots + c_k v_k \mid c_i \in F\}$.

#### Matrisler
- **Matris İşlemleri:** Toplama, skalar çarpma, matris çarpımı $(AB)_{ij} = \sum_k A_{ik}B_{kj}$.
- **Determinant:** $\det(A)$, permütasyon formülü, kofaktör açılımı, Cramer kuralı.
- **İz (Trace):** $\text{tr}(A) = \sum_i A_{ii}$. Özdeğerlerin toplamına eşit.
- **Matris Tersi:** $A^{-1}$ var $\iff$ $\det(A) \neq 0$.

#### Doğrusal Dönüşümler
- **Tanım:** $T: V \to W$ doğrusal $\iff$ $T(u+v) = T(u)+T(v)$ ve $T(cv) = cT(v)$.
- **Çekirdek (Kernel):** $\ker(T) = \{v \in V \mid T(v) = 0\}$ — bir alt uzay.
- **Görüntü (Image):** $\text{im}(T) = \{T(v) \mid v \in V\}$ — bir alt uzay.
- **Boyut Teoremi (Rank-Nullity):** $\dim(V) = \dim(\ker T) + \dim(\text{im}\, T)$.

#### Özdeğer ve Özvektörler
- **Tanım:** $Av = \lambda v$, $v \neq 0$. $\lambda$: özdeğer, $v$: özvektör.
- **Karakteristik Polinom:** $p(\lambda) = \det(\lambda I - A)$. Özdeğerler bu polinomun kökleridir.
- **Köşegenleştirme:** $A = PDP^{-1}$ — $D$ köşegen, $P$ özvektörlerden oluşan matris.
- **Spektral Teorem:** Simetrik (gerçel) veya Hermityan (karmaşık) matrisler ortonormal bir özvektör bazına sahiptir.

#### İç Çarpım Uzayları
- **İç Çarpım:** $\langle u, v \rangle$ — pozitif tanımlı, simetrik (veya Hermityan), doğrusal.
- **Norm:** $\|v\| = \sqrt{\langle v, v \rangle}$.
- **Cauchy-Schwarz Eşitsizliği:** $|\langle u, v \rangle| \leq \|u\| \cdot \|v\|$.
- **Gram-Schmidt:** Doğrusal bağımsız vektörlerden ortonormal baz elde etme algoritması.
- **QR Ayrışımı:** $A = QR$; $Q$ ortogonal, $R$ üst üçgen.

### İleri Konular

- **Jordan Kanonik Formu:** Her matrisin üst üçgen kanonik formu.
- **Tekil Değer Ayrışımı (SVD):** $A = U\Sigma V^T$ — veri sıkıştırma, PCA temeli.
- **LU Ayrışımı:** Doğrusal sistemlerin etkin çözümü.
- **Pozitif Tanımlı Matrisler:** $x^TAx > 0,\ \forall x \neq 0$.


## 📚 Kitap Önerileri


### Başlangıç Seviyesi

- **Gilbert Strang** — *Introduction to Linear Algebra* (5. baskı)
  - MIT'nin standart ders kitabı. Sezgisel, uygulamalı, görsel.
  - Zorluk: ★★☆☆☆ | Dil: İngilizce

- **Sheldon Axler** — *Linear Algebra Done Right*
  - Determinant-free yaklaşım, soyut vektör uzayları. Sıkı teorik temel.
  - Zorluk: ★★★☆☆ | Dil: İngilizce

- **David Lay** — *Linear Algebra and Its Applications*
  - Uygulama odaklı, bol örnek ve grafik.
  - Zorluk: ★★☆☆☆ | Dil: İngilizce

### İleri Seviye

- **Hoffman & Kunze** — *Linear Algebra*
  - Klasik ve kapsamlı referans, soyut cebir bağlantısı güçlü.
  - Zorluk: ★★★★☆ | Dil: İngilizce

- **Roman** — *Advanced Linear Algebra*
  - Modüler yaklaşım, bilinear formlar, tensörler.
  - Zorluk: ★★★★★ | Dil: İngilizce

- **Horn & Johnson** — *Matrix Analysis*
  - Matris teorisi ve uygulamalar, araştırma seviyesi.
  - Zorluk: ★★★★★ | Dil: İngilizce

### Türkçe Kaynaklar

- **Ömer Köküsarı** — *Lineer Cebir* — Türkçe üniversite ders kitabı.
- **Mustafa Balcı** — *Lineer Cebir* — Temel kavramlar, alıştırmalar.


## 🌐 Web Siteleri ve Kaynaklar


### İnteraktif Kaynaklar

- [Immersive Linear Algebra](https://immersivemath.com/ila/) — Tamamen interaktif, online kitap
- [3Blue1Brown — Essence of Linear Algebra](https://www.3blue1brown.com/topics/linear-algebra) — Görsel sezgi serisi
- [Khan Academy — Linear Algebra](https://www.khanacademy.org/math/linear-algebra) — Temel alıştırmalar
- [MIT OpenCourseWare 18.06](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/) — Gilbert Strang dersleri

### Hesaplamalı Araçlar

- [Wolfram Alpha — Matrix Calculator](https://www.wolframalpha.com/) — Matris hesaplama
- [MATLAB Online](https://matlab.mathworks.com/) — Sayısal hesaplama
- [NumPy Documentation](https://numpy.org/doc/) — Python ile doğrusal cebir

### Problem Setleri

- [MIT 18.06 Problem Sets](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/pages/assignments/) — Strang'in ödev soruları
- [Linear Algebra Done Right — Exercises](https://linear.axler.net/) — Axler'ın problem setleri


## 🎬 Video Dersler


### Üniversite Dersleri

- [MIT 18.06 — Linear Algebra (Gilbert Strang)](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/video_galleries/video-lectures/) — En ünlü doğrusal cebir ders serisi
- [MIT 18.065 — Matrix Methods in Data Analysis](https://ocw.mit.edu/courses/18-065-matrix-methods-in-data-analysis-signal-processing-and-machine-learning-spring-2018/) — SVD, PCA, makine öğrenmesi bağlantıları

### YouTube Kanalları

- [3Blue1Brown — Essence of Linear Algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab) — 15 bölümlük geometrik sezgi serisi
- [Professor Leonard](https://www.youtube.com/@ProfessorLeonard) — Doğrusal cebir dersleri, adım adım çözümler
- [Trefor Bazett](https://www.youtube.com/@DrTreforBazett) — Görsel ve açıklayıcı anlatım
- [MathTheBeautiful](https://www.youtube.com/@MathTheBeautiful) — Pavel Grinfeld, geometrik yaklaşım

### Türkçe Video Kaynaklar

- [Ahmet Yıldırım — Lineer Cebir](https://www.youtube.com/) — Türk üniversitelerinde kullanılan ders serisi


---

[← Analysis]({{ '/analysis/' | relative_url }}) | [Ana Sayfa]({{ '/' | relative_url }}) | [Abstract Algebra →]({{ '/abstract-algebra/' | relative_url }})
