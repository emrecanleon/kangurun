# KanguRun

Tek dosyalık, bağımlılıksız HTML5 Canvas koşu oyunu (kanguru). Açık/koyu tema (sistem temasına otomatik uyum), dikey ve yatay çalışır; 10 dil destekler (TR, EN, ES, FR, DE, IT, PT-BR, AR, RU, ZH). PWA olarak telefona yüklenebilir ve çevrimdışı oynanır.

## Yapı

```
index.html
manifest.webmanifest
sw.js
_headers
netlify.toml
.nojekyll
LICENSE
README.md
icons/
  icon-192.png
  icon-512.png
  apple-touch-icon.png
```

## Kurulum

**GitHub Pages:** Dosyaları repo köküne yükle → Settings → Pages → Branch: `main` / `(root)`.

**Cloudflare Pages:** Repoyu bağla → Framework preset: `None`, Build command: boş, Output directory: `/`.

**Netlify:** Repoyu bağla; `netlify.toml` otomatik okunur.

**Yerelde test:** `python3 -m http.server 8000` → http://localhost:8000 (service worker için `https` veya `localhost` gerekir).

## Telefona yükleme

- **Android / Chrome:** Menü → "Ana ekrana ekle" / "Uygulamayı yükle".
- **iOS / Safari:** Paylaş → "Ana Ekrana Ekle".

## Güncelleme

Değişiklik yaptığında `sw.js` içindeki `VERSION` değerini artır; eski önbellek otomatik silinir.

## Lisans

MIT © 2026 A. Emre Canaslan
