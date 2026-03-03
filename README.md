# 📁 STRUKTUR WEBSITE DESA - FILE TERPISAH

## 📂 Struktur Folder

```
website-desa/
│
├── index.html                  # File HTML utama
│
├── assets/                     # Folder aset website
│   ├── css/                    # Folder CSS
│   │   └── style.css          # File CSS utama
│   │
│   ├── js/                     # Folder JavaScript
│   │   └── script.js          # File JavaScript utama
│   │
│   └── images/                 # Folder gambar
│       ├── hero-bg.jpg        # Gambar background hero
│       ├── logo.png           # Logo desa
│       ├── favicon.png        # Favicon
│       └── gallery/           # Folder galeri
│
└── README.md                   # Dokumentasi ini
```

---

## 🚀 Cara Instalasi

### Metode 1: Upload ke Hosting

1. **Download semua file dan folder**
2. **Upload ke hosting** melalui cPanel File Manager atau FTP
3. **Upload ke folder** `public_html/`
4. **Akses website** via `https://namadomain.com`

### Metode 2: Local Development

1. **Letakkan folder** di server lokal (XAMPP/WAMP/MAMP)
2. **Akses via browser**: `http://localhost/website-desa/`

---

## 📝 Penjelasan File

### 1. index.html
File HTML utama yang berisi struktur konten website:
- Navigation menu
- Hero section
- Statistics section
- Profile section
- Government section
- Services section
- News section
- Potential section
- Gallery section
- Contact section
- Footer

**Link ke file eksternal:**
```html
<!-- CSS -->
<link rel="stylesheet" href="assets/css/style.css">

<!-- JavaScript -->
<script src="assets/js/script.js"></script>
```

### 2. assets/css/style.css
File CSS yang berisi semua styling:
- CSS Variables (warna, font, spacing)
- Reset & base styles
- Typography
- Navigation styling
- Hero section styling
- Card layouts
- Responsive design
- Animations

**Cara mengubah warna tema:**
Edit bagian `:root` di file `style.css`:
```css
:root {
    --primary-green: #2d5016;      /* Warna utama */
    --accent-gold: #d4a574;        /* Warna aksen */
    --bg-cream: #faf8f4;           /* Background */
}
```

### 3. assets/js/script.js
File JavaScript yang berisi fungsi interaktif:
- Mobile menu toggle
- Navbar scroll effect
- Active nav link highlighting
- Smooth scrolling
- Fade-in animations
- Counter animations
- Footer year auto-update

**Tidak perlu diubah** kecuali ingin menambah fitur baru.

---

## 🎨 Kustomisasi

### Mengganti Teks Konten

Edit file `index.html`:

1. **Nama Desa:**
```html
<!-- Cari dan ganti -->
<span>Desa Oelomin</span>
```

2. **Statistik:**
```html
<!-- Edit atribut data-target -->
<div class="stat-number" data-target="5420">0</div>
```

3. **Informasi Kontak:**
```html
<!-- Edit di section kontak -->
<span class="info-value">Alamat Anda</span>
```

### Mengganti Warna

Edit file `assets/css/style.css`:

**Tema Biru:**
```css
:root {
    --primary-green: #1e3a8a;
    --primary-green-light: #3b82f6;
    --accent-gold: #fbbf24;
}
```

**Tema Cokelat:**
```css
:root {
    --primary-green: #78350f;
    --primary-green-light: #92400e;
    --accent-gold: #f59e0b;
}
```

### Menambahkan Gambar

1. Upload gambar ke `assets/images/`
2. Edit `index.html`:

**Hero background:**
```html
<div class="hero-background" style="background-image: url('assets/images/hero-bg.jpg');"></div>
```

**Profile image:**
```html
<div class="profile-image" style="background-image: url('assets/images/profile.jpg');"></div>
```

**News card:**
```html
<div class="news-image" style="background-image: url('assets/images/news-1.jpg');"></div>
```

---

## 📱 Responsive Design

Website sudah **100% responsif** untuk:
- Desktop (>1200px)
- Tablet (768px - 1199px)
- Mobile (<767px)

Breakpoints ada di `style.css` bagian `@media`:
```css
@media (max-width: 768px) {
    /* Mobile styles */
}
```

---

## ⚡ Optimasi Kecepatan

### 1. Kompresi Gambar
Gunakan tools:
- TinyPNG: https://tinypng.com
- ImageOptim
- Squoosh: https://squoosh.app

**Ukuran yang disarankan:**
- Hero: 1920x1080px, max 200KB
- Thumbnail: 400x300px, max 50KB
- Icon: 100x100px, max 20KB

### 2. Minifikasi (Production)

**CSS:**
```bash
# Online: https://cssminifier.com
# Atau install tool:
npm install -g csso-cli
csso style.css -o style.min.css
```

**JavaScript:**
```bash
# Online: https://javascript-minifier.com
# Atau install tool:
npm install -g uglify-js
uglifyjs script.js -o script.min.js -c -m
```

Kemudian update link di `index.html`:
```html
<link rel="stylesheet" href="assets/css/style.min.css">
<script src="assets/js/script.min.js"></script>
```

### 3. Browser Caching

Buat file `.htaccess` di root folder:
```apache
<IfModule mod_expires.c>
    ExpiresActive On
    ExpiresByType text/css "access plus 1 month"
    ExpiresByType application/javascript "access plus 1 month"
    ExpiresByType image/jpeg "access plus 1 year"
    ExpiresByType image/png "access plus 1 year"
</IfModule>
```

---

## 🔧 Debugging

### CSS tidak muncul?
1. Cek path di `index.html`: `href="assets/css/style.css"`
2. Pastikan file ada di folder yang benar
3. Clear browser cache (Ctrl+Shift+R)

### JavaScript tidak berfungsi?
1. Buka Developer Tools (F12)
2. Cek tab Console untuk error
3. Pastikan path script benar: `src="assets/js/script.js"`

### Gambar tidak muncul?
1. Cek path gambar (case-sensitive!)
2. Pastikan file gambar ada
3. Cek file permission (644)

---

## 📋 Checklist Deployment

- [ ] Ganti nama desa di semua tempat
- [ ] Update statistik (jumlah penduduk, dll)
- [ ] Update informasi kontak
- [ ] Tambahkan gambar hero, profile, news
- [ ] Ganti warna tema (opsional)
- [ ] Test di desktop & mobile
- [ ] Kompresi semua gambar
- [ ] Minify CSS & JS untuk production
- [ ] Upload ke hosting
- [ ] Test kecepatan (Google PageSpeed)
- [ ] Setup SSL (HTTPS)

---

## 🎯 Fitur Tambahan (Opsional)

### 1. Google Analytics
Tambahkan sebelum `</head>`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

### 2. Google Maps
Di section kontak, ganti emoji peta:
```html
<iframe 
    src="https://www.google.com/maps/embed?pb=YOUR_EMBED_CODE"
    width="100%" 
    height="500" 
    style="border:0; border-radius:20px;" 
    allowfullscreen="" 
    loading="lazy">
</iframe>
```

### 3. WhatsApp Button
Tambahkan di footer atau floating:
```html
<a href="https://wa.me/6281234567890" class="whatsapp-float" target="_blank">
    <i class="fa fa-whatsapp"></i>
</a>
```

---

## 📞 Support

### Dokumentasi Lengkap
- HTML: https://developer.mozilla.org/en-US/docs/Web/HTML
- CSS: https://developer.mozilla.org/en-US/docs/Web/CSS
- JavaScript: https://developer.mozilla.org/en-US/docs/Web/JavaScript

### Tools
- Validator HTML: https://validator.w3.org
- Validator CSS: https://jigsaw.w3.org/css-validator/
- PageSpeed: https://pagespeed.web.dev

---

## ✅ Keuntungan Struktur File Terpisah

1. **Mudah Dimaintain** - Edit CSS/JS tanpa buka HTML
2. **Cache Browser** - Loading lebih cepat di visit kedua
3. **Reusability** - Satu CSS/JS bisa dipakai banyak halaman
4. **Collaboration** - Tim bisa kerja parallel (HTML, CSS, JS)
5. **Production Ready** - Mudah di-minify dan optimize
6. **Version Control** - Lebih mudah track changes

---

## 📦 File Size

```
index.html         ~25 KB
style.css          ~35 KB
script.js          ~4 KB
--------------------------
Total (tanpa gambar) ~64 KB
```

**Dengan gambar (compressed):**
- Hero background: ~200 KB
- Profile image: ~100 KB
- 3 News images: ~150 KB
- 6 Gallery images: ~300 KB
- **Total: ~814 KB** ✅ Sangat ringan!

---

## 🌟 Best Practices

1. **Selalu backup** file sebelum edit
2. **Test di berbagai browser** (Chrome, Firefox, Safari, Edge)
3. **Optimize gambar** sebelum upload
4. **Gunakan HTTPS** untuk keamanan
5. **Update konten** secara rutin
6. **Monitor performance** dengan PageSpeed Insights

---

**Terakhir diupdate: 4 Februari 2026**

Untuk pertanyaan lebih lanjut, silakan buka dokumentasi lengkap atau hubungi developer.

Happy Coding! 🚀
