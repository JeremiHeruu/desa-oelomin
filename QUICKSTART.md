# 🚀 QUICK START GUIDE

## Instalasi dalam 3 Langkah

### 1️⃣ Upload ke Hosting
```
1. Download folder website-terpisah
2. Buka cPanel > File Manager
3. Upload semua file & folder ke public_html/
4. Done! ✅
```

### 2️⃣ Edit Konten
```
Edit file: index.html

Ganti:
- Nama desa (Ctrl+F: "Oelomin")
- Statistik (cari: data-target="")
- Kontak (cari: info-value)
```

### 3️⃣ Ganti Warna (Opsional)
```
Edit file: assets/css/style.css

Cari baris ini (sekitar baris 21-27):
:root {
    --primary-green: #2d5016;    /* Ganti warna */
    --accent-gold: #d4a574;      /* Ganti warna */
}
```

---

## 🎨 Preset Warna

Copy-paste salah satu ke `style.css`:

**Hijau (Default):**
```css
--primary-green: #2d5016;
--primary-green-light: #4a7c2c;
--accent-gold: #d4a574;
```

**Biru:**
```css
--primary-green: #1e3a8a;
--primary-green-light: #3b82f6;
--accent-gold: #fbbf24;
```

**Cokelat:**
```css
--primary-green: #78350f;
--primary-green-light: #92400e;
--accent-gold: #f59e0b;
```

---

## 📸 Tambah Gambar

1. Upload gambar ke: `assets/images/`
2. Edit `index.html`, cari bagian yang ingin diberi gambar
3. Tambahkan `style="background-image: url('assets/images/nama-file.jpg');"`

**Contoh:**
```html
<!-- Hero Background -->
<div class="hero-background" 
     style="background-image: url('assets/images/hero-bg.jpg');"></div>

<!-- Profile Image -->
<div class="profile-image" 
     style="background-image: url('assets/images/profile.jpg');"></div>

<!-- News Image -->
<div class="news-image" 
     style="background-image: url('assets/images/news/berita-1.jpg');"></div>
```

**Tips:**
- Compress gambar dulu di https://tinypng.com
- Hero: 1920x1080px, max 200KB
- News: 800x600px, max 100KB

---

## ✅ Checklist

- [ ] Upload semua file ke hosting
- [ ] Ganti nama desa
- [ ] Update statistik
- [ ] Update kontak (alamat, telepon, email)
- [ ] Upload & set gambar hero
- [ ] Upload & set gambar profile
- [ ] Test di mobile & desktop
- [ ] Aktifkan HTTPS/SSL

---

## 🆘 Troubleshooting

**CSS tidak muncul?**
- Cek file `style.css` ada di `assets/css/`
- Clear cache browser (Ctrl+Shift+R)

**JavaScript tidak jalan?**
- Cek file `script.js` ada di `assets/js/`
- Buka Console (F12) untuk cek error

**Gambar tidak muncul?**
- Cek path gambar (case-sensitive!)
- Pastikan file gambar sudah diupload

---

## 📚 Dokumentasi Lengkap

Baca **README.md** untuk panduan detail.

---

**Selamat! Website desa Anda siap! 🎉**
