# 📸 Folder Gambar

Letakkan semua gambar website di folder ini.

## Struktur yang Disarankan

```
images/
├── hero-bg.jpg           # Background hero section (1920x1080px)
├── logo.png              # Logo desa (transparent PNG)
├── favicon.png           # Favicon (32x32px atau 64x64px)
├── profile/              # Gambar profil desa
│   └── desa-view.jpg
├── news/                 # Gambar berita
│   ├── news-1.jpg
│   ├── news-2.jpg
│   └── news-3.jpg
└── gallery/              # Galeri foto
    ├── kegiatan-1.jpg
    ├── kegiatan-2.jpg
    └── ...
```

## Format Gambar yang Disarankan

### Format File
- **JPEG/JPG** - Untuk foto (lebih kecil file size)
- **PNG** - Untuk gambar dengan transparansi (logo, icon)
- **WebP** - Format modern, ukuran kecil (jika browser support)

### Ukuran File
- **Hero Background**: Max 200 KB
- **News Thumbnail**: Max 50 KB
- **Gallery**: Max 100 KB per foto
- **Logo/Icon**: Max 20 KB

## Tools Kompresi Gambar

1. **TinyPNG** - https://tinypng.com
2. **Squoosh** - https://squoosh.app
3. **ImageOptim** (Mac)
4. **RIOT** (Windows)
5. **Optimizilla** - https://imagecompressor.com

## Cara Menggunakan Gambar

### 1. Background Image (CSS)
```css
.hero-background {
    background-image: url('../images/hero-bg.jpg');
}
```

### 2. HTML Image Tag
```html
<img src="assets/images/logo.png" alt="Logo Desa Oelomin">
```

### 3. Inline Style
```html
<div style="background-image: url('assets/images/news/news-1.jpg');"></div>
```

## Tips Optimasi

1. **Resize** gambar sebelum upload (jangan upload foto 5MB!)
2. **Compress** dengan tools di atas
3. **Use WebP** untuk browser modern
4. **Lazy Loading** untuk gambar di bawah fold
5. **Alt Text** selalu isi untuk SEO

## Konvensi Penamaan File

- Gunakan huruf kecil semua
- Pisahkan kata dengan dash (-)
- Hindari spasi dan karakter khusus
- Deskriptif tapi singkat

**Contoh:**
✅ `hero-background.jpg`
✅ `news-pembangunan-jalan.jpg`
✅ `galeri-posyandu-2024.jpg`

❌ `Hero Background.jpg`
❌ `IMG_1234.jpg`
❌ `foto kegiatan (copy).jpg`

---

**Note:** File ini (README.md) hanya untuk dokumentasi. Anda bisa menghapusnya setelah memahami strukturnya.
