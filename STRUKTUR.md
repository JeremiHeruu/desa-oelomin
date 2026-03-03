# 📦 STRUKTUR LENGKAP WEBSITE DESA

```
website-terpisah/
│
├── 📄 index.html                    # Halaman utama website
│
├── 📂 assets/                       # Folder aset website
│   │
│   ├── 📂 css/                      # Folder CSS
│   │   └── 📄 style.css            # File CSS utama (21 KB)
│   │
│   ├── 📂 js/                       # Folder JavaScript
│   │   └── 📄 script.js            # File JavaScript utama (4 KB)
│   │
│   └── 📂 images/                   # Folder gambar
│       ├── 📄 README.md            # Panduan folder images
│       ├── 📷 hero-bg.jpg          # (Upload gambar Anda)
│       ├── 📷 logo.png             # (Upload gambar Anda)
│       ├── 📷 favicon.png          # (Upload gambar Anda)
│       ├── 📂 news/                # Subfolder gambar berita
│       ├── 📂 gallery/             # Subfolder galeri
│       └── 📂 profile/             # Subfolder profil desa
│
├── 📄 .htaccess                     # Konfigurasi server Apache
├── 📄 .gitignore                    # Git ignore file
│
├── 📚 README.md                     # Dokumentasi lengkap
├── 🚀 QUICKSTART.md                 # Panduan cepat
├── 📝 CHANGELOG.md                  # Log perubahan
├── 📋 TEMPLATE-BERITA.html          # Template tambah berita
└── 📜 LICENSE                       # Lisensi MIT

```

---

## 📊 Detail Ukuran File

| File/Folder | Ukuran | Keterangan |
|-------------|--------|------------|
| **index.html** | ~24 KB | Struktur HTML lengkap |
| **style.css** | ~21 KB | Semua styling website |
| **script.js** | ~4 KB | Fungsi interaktif |
| **Total Code** | **~49 KB** | Sangat ringan! |
| **.htaccess** | ~7.6 KB | Optimasi server |
| **Dokumentasi** | ~15 KB | README + guides |

**Total Website (tanpa gambar): ~72 KB** ✅

---

## 🎯 Fungsi Setiap File

### File Utama
- **index.html** → Konten website (yang dilihat user)
- **style.css** → Desain dan tampilan
- **script.js** → Interaktivitas (menu, animasi, dll)

### File Konfigurasi
- **.htaccess** → Optimasi kecepatan & keamanan server
- **.gitignore** → File yang tidak di-commit ke Git

### File Dokumentasi
- **README.md** → Panduan lengkap (baca ini dulu!)
- **QUICKSTART.md** → Panduan cepat untuk pemula
- **CHANGELOG.md** → Catatan perubahan versi
- **TEMPLATE-BERITA.html** → Copy-paste untuk tambah berita
- **LICENSE** → Lisensi penggunaan (MIT - bebas dipakai)

---

## 🚦 Urutan Baca Dokumentasi

```
1. QUICKSTART.md    ← Mulai di sini (instalasi 3 langkah)
2. README.md        ← Panduan lengkap kustomisasi
3. TEMPLATE-BERITA.html ← Cara tambah berita
4. CHANGELOG.md     ← Lihat fitur & update
```

---

## 📁 Folder yang Perlu Diisi

### 1. assets/images/
Upload gambar website Anda:
- Hero background (1920x1080px)
- Logo desa (PNG transparan)
- Favicon (32x32px)
- Foto profil desa
- Gambar berita (800x600px)
- Galeri kegiatan

**Wajib compress di**: https://tinypng.com

### 2. Tidak Ada Folder Lain
Semua sudah lengkap!

---

## 🔄 Workflow Edit

```
1. Edit konten       → index.html
2. Ganti warna/style → assets/css/style.css
3. Tambah fungsi JS  → assets/js/script.js
4. Upload gambar     → assets/images/
5. Save & upload     → Upload ke hosting
6. Test              → Buka di browser
```

---

## ✅ Checklist File

Pastikan semua file ada:

- [x] index.html
- [x] assets/css/style.css
- [x] assets/js/script.js
- [x] .htaccess
- [x] README.md
- [x] QUICKSTART.md
- [ ] assets/images/hero-bg.jpg (Upload Anda)
- [ ] assets/images/logo.png (Upload Anda)
- [ ] assets/images/favicon.png (Upload Anda)

---

## 💡 Tips Organisasi

### Backup
Selalu backup sebelum edit:
```
website-terpisah/
website-terpisah-backup-2026-02-04/
website-terpisah-backup-2026-02-10/
```

### Version Control
Gunakan Git untuk tracking changes:
```bash
git init
git add .
git commit -m "Initial commit"
```

### File Naming
- Lowercase semua
- Pisah dengan dash (-)
- Deskriptif tapi singkat

✅ `berita-pembangunan-jalan.html`
❌ `Berita Pembangunan Jalan.html`

---

## 🎨 Struktur CSS (dalam style.css)

```css
/* 1. CSS Variables (warna, font, spacing) */
/* 2. Reset & Base Styles */
/* 3. Typography (h1, h2, p) */
/* 4. Utility Classes (.container, .section) */
/* 5. Navigation */
/* 6. Hero Section */
/* 7. Stats Section */
/* 8. Profile Section */
/* 9. Government Section */
/* 10. Services Section */
/* 11. News Section */
/* 12. Gallery Section */
/* 13. Footer */
/* 14. Responsive Design (@media) */
/* 15. Animations */
```

Mudah dinavigasi dengan comment sections!

---

## 🔧 Struktur JavaScript (dalam script.js)

```javascript
// 1. Mobile menu toggle
// 2. Navbar scroll effect
// 3. Active nav highlighting
// 4. Smooth scroll
// 5. Fade-in animations (Intersection Observer)
// 6. Counter animations
// 7. Footer year auto-update
```

Semua terdokumentasi dengan jelas!

---

## 📱 Responsive Breakpoints

```css
Desktop:  > 1200px  → Full layout
Tablet:   768-1199px → Adjusted grid
Mobile:   < 768px   → Stacked layout, hamburger menu
```

---

## 🎯 File yang Wajib Diedit

```
1. index.html
   - Ganti nama desa
   - Update statistik
   - Edit kontak
   - Tambah berita

2. assets/css/style.css
   - (Opsional) Ganti warna tema

3. Upload gambar ke:
   - assets/images/
```

File lain **TIDAK** perlu diedit (kecuali advanced customization).

---

**Struktur ini dirancang:**
- ✅ Clean & organized
- ✅ Easy to navigate
- ✅ Well documented
- ✅ Production ready
- ✅ SEO friendly
- ✅ Performance optimized

**Happy coding! 🚀**
