# 📸 Photobooth Assets Repository

Repositori penyimpanan aset multimedia statis (CDN-hosted) untuk ekosistem **Kaze Photobooth**.
Disajikan langsung ke Kiosk App dan Dashboard melalui jsDelivr / GitHub Raw CDN.

---

## 🗂️ Struktur Direktori & Penamaan Bersih

Seluruh aset telah distandardisasi dengan penamaan semantik tanpa timestamp berantakan:

```text
photobooth-assets/
├── branding/                      # Aset identitas & tampilan tenant/kiosk
│   ├── announcements/             # Banner / video pengumuman fullscreen (announcement_*.mp4)
│   ├── backgrounds/               # Wallpaper / background layar start & selection
│   ├── logos/                     # Logo tenant / watermark brand (logo_kaze_main.png)
│   ├── packages/                  # Gambar visual paket photobooth
│   ├── screensavers/              # Video / gambar screensaver animasi idle
│   └── watermarks/                # Watermark transparan untuk foto hasil (wm_kaze_default.png)
│
├── filters/                       # Aset grading warna kamera
│   ├── luts/                      # Tabel warna 3DLUT (.cube) (lut_drip_04.cube, lut_flex_02.cube, dll)
│   └── previews/                  # Thumbnail preview filter (thumb_drip_04.jpg, dll)
│
├── frames/                        # Template bingkai foto cetak
│   ├── side_b/                    # Template strip sisi belakang / duplex (sideb_gito_vintage.webp, dll)
│   ├── templates/                 # Template overlay frame utama (frame_gito_vintage_4r.webp, dll)
│   └── thumbnails/                # Thumbnail mini kartu frame (thumb_gito_vintage.jpg, dll)
│
├── icons/                         # Ikon antarmuka & navigasi
│   ├── categories/                # Cover square 1:1 kategori (icon_cat_idulfitri.jpg, icon_cat_valentine.jpg, dll)
│   └── ui/                        # Ikon kontrol UI kiosk
│
├── payments/                      # Aset transaksi
│   └── qris/                      # Kode QRIS pembayaran (qris_kaze_primary.jpg)
│
└── stickers/                      # Aset dekorasi foto interaktif
    ├── animated/                  # Stiker bergerak GIF (stk_cat_dance.gif, stk_gura_wave.gif, stk_maxwell_spin.gif, dll)
    └── static/                    # Stiker ilustrasi PNG (stk_cat_meme_08.png, stk_cat_cute_01.png, dll)
```

---

## 🌐 Format URL CDN (jsDelivr)

```text
https://cdn.jsdelivr.net/gh/Dhiandika/photobooth-assets@main/<folder>/<nama_file>
```

### Contoh URL Siap Pakai:
- **Frame Utama**:  
  `https://cdn.jsdelivr.net/gh/Dhiandika/photobooth-assets@main/frames/templates/frame_mu_aesthetic_4r.webp`
- **Side B Duplex**:  
  `https://cdn.jsdelivr.net/gh/Dhiandika/photobooth-assets@main/frames/side_b/sideb_gito_vintage.webp`
- **Cover Kategori**:  
  `https://cdn.jsdelivr.net/gh/Dhiandika/photobooth-assets@main/icons/categories/icon_cat_valentine.jpg`
- **LUT 3D Table**:  
  `https://cdn.jsdelivr.net/gh/Dhiandika/photobooth-assets@main/filters/luts/lut_drip_04.cube`
- **Stiker Bergerak**:  
  `https://cdn.jsdelivr.net/gh/Dhiandika/photobooth-assets@main/stickers/animated/stk_maxwell_spin.gif`
- **Stiker PNG**:  
  `https://cdn.jsdelivr.net/gh/Dhiandika/photobooth-assets@main/stickers/static/stk_cat_meme_08.png`
- **Logo Brand**:  
  `https://cdn.jsdelivr.net/gh/Dhiandika/photobooth-assets@main/branding/logos/logo_kaze_main.png`
- **QRIS Pembayaran**:  
  `https://cdn.jsdelivr.net/gh/Dhiandika/photobooth-assets@main/payments/qris/qris_kaze_primary.jpg`
