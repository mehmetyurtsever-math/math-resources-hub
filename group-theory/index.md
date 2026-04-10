---
layout: default
title: Group Theory (Grup Teorisi)
---

# ◈ Group Theory (Grup Teorisi)

Simetriyi matematiksel olarak kodlayan cebirsel yapılar. Kristalografi'den kuantum mekaniğine kadar geniş uygulama alanı.

---

<details>
<summary>📖 Ders Notları</summary>
<div class="details-body">

### Temel Kavramlar

#### Gruplar ve Simetri
- **Simetri Grubu:** Bir nesnenin simetri dönüşümlerinin oluşturduğu grup.
- **Dihedral Grup $D_n$:** Düzgün $n$-genin simetrileri; $2n$ eleman.
- **Simetrik Grup $S_n$:** $n$ elemanın tüm permütasyonları; $|S_n| = n!$.
- **Devirli Gruplar:** Her $g \in G$ için $\langle g \rangle$ alt grubu; $\mathbb{Z}_n \cong \mathbb{Z}/n\mathbb{Z}$.

#### Alt Gruplar ve Bölüm Grupları
- **Lagrange Teoremi:** $H \leq G$ ise $|H| \mid |G|$.
- **Koset:** $gH = \{gh \mid h \in H\}$ sol, $Hg$ sağ koset.
- **Normal Alt Grup:** $gNg^{-1} = N,\ \forall g \in G$.
- **Bölüm Grubu:** $G/N$ — kosetlerin grubu.

#### Grup Homomorfizmaları
- **Tanım:** $\phi: G \to H$, $\phi(ab) = \phi(a)\phi(b)$.
- **Birinci İzomorfizm Teoremi:** $G/\ker\phi \cong \text{im}\,\phi$.
- **Otomorfizmalar:** $\text{Aut}(G)$ — bir grubun kendisine olan izomorfizmleri.

#### Sylow Teoremleri
- **Sylow $p$-altgrubu:** Maksimal $p$-kuvveti mertebeli alt grup.
- **Sylow I:** $|G| = p^a m$ ($p \nmid m$) ise mertebesi $p^a$ olan alt grup vardır.
- **Sylow II & III:** Sylow alt gruplarının konjugasyon altında geçişkenliği ve sayısı.
- **Uygulama:** Belirli mertebedeki grupların basit olmadığını kanıtlama.

### Örnekler ve Alıştırmalar

- $\mathbb{Z}_4$, $\mathbb{Z}_2 \times \mathbb{Z}_2$, $S_3$, $D_4$, $Q_8$ (Quaternion grubu) incelemesi.
- Alıştırma: Mertebesi 6 olan grupların $\mathbb{Z}_6$ veya $S_3$'e izomorf olduğunu kanıtlayın.
- Alıştırma: Mertebesi 15 olan her grubun devirli olduğunu gösterin.

</div>
</details>

<details>
<summary>📚 Kitap Önerileri</summary>
<div class="details-body">

### Başlangıç Seviyesi

- **Joseph Gallian** — *Contemporary Abstract Algebra*
  - Bol örnek ve uygulama, başlangıç için ideal.
  - Zorluk: ★★☆☆☆ | Dil: İngilizce

- **Dummit & Foote** — *Abstract Algebra* (Grup teorisi bölümleri)
  - Kapsamlı ve standart referans.
  - Zorluk: ★★★☆☆ | Dil: İngilizce

### İleri Seviye

- **Aschbacher** — *Finite Group Theory*
  - Sonlu grup teorisinin ileri düzey işlenmesi.
  - Zorluk: ★★★★★ | Dil: İngilizce

- **Robinson** — *A Course in the Theory of Groups*
  - Sonsuz grup teorisi dahil geniş kapsam.
  - Zorluk: ★★★★☆ | Dil: İngilizce

- **Serre** — *Linear Representations of Finite Groups*
  - Grup temsil teorisi, karakter teorisi.
  - Zorluk: ★★★★☆ | Dil: İngilizce

</div>
</details>

<details>
<summary>🌐 Web Siteleri ve Kaynaklar</summary>
<div class="details-body">

### İnteraktif Kaynaklar

- [Group Explorer](https://nathancarter.github.io/group-explorer/) — Grupları görsel keşfet
- [Visual Group Theory](https://www.youtube.com/playlist?list=PLwV-9DG53NDxU337smpTwm6sef4x-SCLv) — Görsel anlatım
- [Algebra — Keith Conrad](https://kconrad.math.uconn.edu/blurbs/) — Detaylı ekspozitif notlar

### Problem Setleri

- [Qualifying Exam Problems — Groups](https://math.stackexchange.com/questions/tagged/group-theory) — StackExchange arşivi
- [MIT OCW — Group Theory Problems](https://ocw.mit.edu/courses/18-703-modern-algebra-spring-2013/pages/assignments/)

</div>
</details>

<details>
<summary>🎬 Video Dersler</summary>
<div class="details-body">

### Üniversite Dersleri

- [MIT 18.703](https://ocw.mit.edu/courses/18-703-modern-algebra-spring-2013/) — Tam ders materyali
- [Oxford — Group Theory](https://www.youtube.com/results?search_query=oxford+group+theory+lecture) — Oxford ders serileri

### YouTube Kanalları

- [Socratica — Group Theory](https://www.youtube.com/playlist?list=PLi01XoE8jYoi3SgnnGorR_XOW3IcK-TP6) — Temel kavramlar
- [Richard Borcherds — Group Theory](https://www.youtube.com/@RichardBorcherds) — İleri grup teorisi
- [Visual Group Theory — MAST 613](https://www.youtube.com/playlist?list=PLwV-9DG53NDxU337smpTwm6sef4x-SCLv) — Görsel yaklaşım

</div>
</details>

---

[← Abstract Algebra]({{ '/abstract-algebra/' | relative_url }}) | [Ana Sayfa]({{ '/' | relative_url }}) | [Logic & Proofs →]({{ '/logic-and-proofs/' | relative_url }})
