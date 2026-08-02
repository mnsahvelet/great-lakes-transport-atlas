# GitHub'a yükleme ve canlı link oluşturma (adım adım)

Bu klasör (`great-lakes-transport-atlas`) GitHub'a yüklenmeye hazır. Git bilmene
gerek yok — aşağıdaki yol tamamen tarayıcı üzerinden.

## 1. GitHub hesabı ve repo

1. https://github.com adresine gir, hesabın yoksa ücretsiz aç.
2. Sağ üstte **+ → New repository**.
3. **Repository name:** `great-lakes-transport-atlas`
4. Şimdilik **Private** seç (paper submit olana kadar gizli kalsın).
5. "Add a README" gibi kutuları **işaretleme** (bizde zaten var).
6. **Create repository**.

## 2. Dosyaları yükle

1. Yeni repo sayfasında **Add file → Upload files**.
2. Bu klasörün İÇİNDEKİ tüm dosyaları sürükle-bırak:
   `index.html`, `.nojekyll`, `robots.txt`, `README.md`, `LICENSE`, `CITATION.cff`
   - ÖNEMLİ: `great-lakes-transport-atlas` klasörünün kendisini değil, İÇİNDEKİ
     dosyaları yükle. `index.html` repo'nun kök dizininde olmalı.
   - `.nojekyll` görünmüyorsa: Windows'ta gizli dosya olabilir; File Explorer'da
     "Hidden items" görünürlüğünü aç veya sürükle-bırak listesine dahil et.
3. Aşağıda **Commit changes**.

> Not: `index.html` 24 MB. GitHub tek dosya sınırı 100 MB olduğu için sorun yok.
> Tarayıcı yüklemesi birkaç dakika sürebilir.

## 3. GitHub Pages'i açma (canlı link)

> Bunu SADECE danışmanına link göstereceğin / submit edeceğin zaman yap.
> Açtığın an sayfa link'i bilenlere açık olur (ama arama motorlarına kapalı).

1. Repo'da **Settings → Pages**.
2. **Source:** "Deploy from a branch".
3. **Branch:** `main`  •  **Folder:** `/ (root)` → **Save**.
4. 1-2 dakika bekle, sayfayı yenile. Yeşil kutuda link çıkar:
   `https://KULLANICI-ADIN.github.io/great-lakes-transport-atlas/`
5. Bu link'i danışmanına gönder. Direkt haritayı açar.

## 4. Paper'da nasıl referans verilir

Draft aşamasında (submit öncesi) metne şunu koyabilirsin:

> An interactive visualization of shoreline-scale potential longshore transport
> is available at: https://KULLANICI-ADIN.github.io/great-lakes-transport-atlas/

Submit / kabul aşamasında Zenodo DOI eklemek için:

> The archived, citable version of the interactive atlas and source code is
> available at: https://doi.org/XX.XXXX/zenodo.XXXXXXX

## 5. Kabul sonrası: kalıcı DOI (Zenodo)

1. https://zenodo.org → GitHub ile giriş yap.
2. **Settings → GitHub** → repo'yu ON yap.
3. GitHub'da **Releases → Create a new release** (örn. `v1.0`).
4. Zenodo otomatik arşivler ve kalıcı bir DOI verir.
5. DOI'yi paper'ın "Data Availability" bölümüne koy.

## Gizlilik notu

- `robots.txt` ve HTML içindeki `noindex` etiketi sayesinde Google vb. sayfayı
  dizine EKLEMEZ. Yani link'i bilmeyen kimse bulamaz.
- Yine de Pages açıkken sayfa teknik olarak herkese açıktır. Tam gizlilik
  gerekiyorsa Pages'i submit anına kadar KAPALI tut; repo'yu private bırak.
- Double-blind hakemlik varsa: submit ederken repo'da adını geçici olarak
  gizlemek isteyebilirsin (README/CITATION içindeki isim). Hatırlat, yardımcı
  olurum.

## Dosya adı değişikliği

Orijinal harita dosyanın adı
`Interactive_Great_Lakes_vanRijn_Transport_5Lakes_WHITE_ARROWS_TIMESERIES.html`
idi; ziyaretçinin dosya adı yazmadan direkt açabilmesi için `index.html` olarak
kopyalandı. İçerik birebir aynı, sadece head kısmına `noindex` etiketi ve bir
başlık eklendi.
