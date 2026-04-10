# Math Resources Hub

Lisans öğrencileri için kapsamlı matematik kaynakları merkezi. Her konu **doğrudan görünür başlık + liste** düzeniyle sunulmuştur.

🌐 **GitHub Pages Site:** https://mehmetyurtsever-math.github.io/math-resources-hub/

## Konular

| Konu | Açıklama |
|------|----------|
| [Analysis](./analysis/) | Limitler, türev, integral, metrik uzaylar |
| [Linear Algebra](./linear-algebra/) | Vektör uzayları, matrisler, özdeğerler |
| [Abstract Algebra](./abstract-algebra/) | Gruplar, halkalar, cisimler |
| [Group Theory](./group-theory/) | Grup aksiyomları, Sylow teoremleri, simetri |
| [Logic and Proofs](./logic-and-proofs/) | Önerme mantığı, küme teorisi, ispat teknikleri |
| [Galois Theory](./galois-theory/) | Cisim uzantıları, Galois grubu, çözülebilirlik |
| [Commutative Algebra](./commutative-algebra/) | Halkalar, idealler, Noetherian yapılar |
| [Complex Analysis](./complex-analysis/) | Karmaşık fonksiyonlar, Cauchy teoremi, rezidüler |
| [Differential Geometry](./differential-geometry/) | Eğriler, yüzeyler, manifoldlar, eğrilik |

## Proje Yapısı

```
math-resources-hub/
├── _config.yml              # Jekyll yapılandırması
├── _layouts/
│   └── default.html         # Navigasyon + footer içeren şablon
├── assets/
│   └── style.css            # Tema ve responsive CSS
├── index.md                 # Ana sayfa (9 konu kartı)
├── analysis/index.md        # Analiz sayfası (detaylı içerik)
├── linear-algebra/index.md  # Doğrusal cebir sayfası
├── abstract-algebra/index.md
├── group-theory/index.md
├── logic-and-proofs/index.md
├── galois-theory/index.md
├── commutative-algebra/index.md
├── complex-analysis/index.md
└── differential-geometry/index.md
```

## Bölüm Yapısı

Her konu sayfasında dört görünür bölüm bulunmaktadır:

- **📖 Ders Notları** — Tanımlar, teoremler, ispatlar, örnekler
- **📚 Kitap Önerileri** — Başlangıç ve ileri seviye kitaplar
- **🌐 Web Siteleri ve Kaynaklar** — Online araçlar ve problem setleri
- **🎬 Video Dersler** — Üniversite dersleri ve YouTube kanalları

Bu bölümler doğrudan başlıklar altında listelenir; içerik gizlenmez.

## Katkıda Bulunma

Yeni içerik veya konu eklemek için:

1. İlgili konu klasörüne gidin (ör. `analysis/`)
2. `index.md` dosyasını düzenleyin
3. Şu yapıyı koruyun:

```html
## 📖 Ders Notları

### Başlık
- İçerik
```

4. Pull Request açın

## GitHub Pages Kurulumu

1. **Settings → Pages**
2. Source: `Deploy from a branch`
3. Branch: `main`, Folder: `/ (root)`
4. **Save** — ~2 dk sonra site yayında
