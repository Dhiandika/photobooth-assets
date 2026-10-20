# 📸 Photobooth Assets Repository

Repositori penyimpanan aset multimedia statis (CDN-hosted) untuk ekosistem **Kaze Photobooth**. Aset ini disajikan langsung ke Kiosk App dan Dashboard melalui jsDelivr / GitHub Raw CDN.

---

## 🗂️ Struktur Direktori

Semua aset diatur secara modular dan terpisah berdasarkan jenis dan fungsinya:

```text
photobooth-assets/
├── branding/                      # Aset identitas & tampilan tenant/kiosk
│   ├── announcements/             # Banner / poster pengumuman fullscreen kiosk
│   ├── backgrounds/               # Wallpaper / background layar start & selection
│   ├── logos/                     # Logo tenant / watermark brand
│   ├── packages/                  # Gambar visual paket photobooth
│   ├── screensavers/              # Video / gambar screensaver animasi idle
│   └── watermarks/                # Watermark transparan untuk foto hasil
│
├── filters/                       # Aset grading warna kamera
│   ├── luts/                      # File tabel warna 3DLUT (.cube)
│   └── previews/                  # Gambar thumbnail perbandingan sebelum & sesudah filter
│
├── frames/                        # Template bingkai foto cetak
│   ├── side_b/                    # Template strip sisi belakang (duplex / strip B)
│   ├── templates/                 # Template overlay frame utama (.webp / .png)
│   └── thumbnails/                # Thumbnail mini untuk layar pemilihan frame
│
├── icons/                         # Ikon antarmuka & navigasi
│   ├── categories/                # Cover / ikon square 1:1 untuk kategori frame
│   └── ui/                        # Ikon navigasi / kontrol UI kiosk
│
├── letters/                       # Aset font khusus / tipografi cetak
│
├── payments/                      # Aset transaksi
│   └── qris/                      # Gambar kode QRIS statis / gateway pembayaran
│
└── stickers/                      # Aset dekorasi foto interaktif
    ├── animated/                  # Stiker bergerak format GIF (.gif)
    └── static/                    # Stiker ilustrasi diam format PNG (.png / .webp)
```

---

## 🌐 Format URL CDN (jsDelivr)

Untuk performa tinggi dan caching global, gunakan format URL CDN berikut:

```text
https://cdn.jsdelivr.net/gh/<owner>/photobooth-assets@main/<folder>/<nama_file>
```

### Contoh URL:
- **Frame Template**:
  `https://cdn.jsdelivr.net/gh/Dhiandika/photobooth-assets@main/frames/templates/1.webp`
- **Icon Kategori**:
  `https://cdn.jsdelivr.net/gh/Dhiandika/photobooth-assets@main/icons/categories/idulfitri.jpg`
- **LUT Filter**:
  `https://cdn.jsdelivr.net/gh/Dhiandika/photobooth-assets@main/filters/luts/CLassicFilm01.cube`
- **Stiker Bergerak**:
  `https://cdn.jsdelivr.net/gh/Dhiandika/photobooth-assets@main/stickers/animated/gura-gwar-gura.gif`

---

## 🏷️ Standar Penamaan File Baru

Saat mengunggah melalui Dashboard Kaze, nama file otomatis diformat dengan format:

```text
{prefix}_{slug}_{YYYYMMDD}_{hash6}.{ext}
```

- **Prefix yang digunakan:**
  - `frame_` : Template bingkai
  - `thumb_` : Thumbnail preview
  - `sideb_` : Bingkai sisi B
  - `icon_`  : Ikon kategori
  - `stk_`   : Stiker ilustrasi
  - `lut_`   : File LUT color table
  - `logo_`  : Logo tenant
  - `wm_`    : Watermark cetak
  - `qris_`  : QRIS pembayaran
  - `bg_`    : Background layar
  - `scrs_`  : Screensaver kiosk
