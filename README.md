# Rapih — Web Landing Page Statis

Halaman web statis mandiri (*zero-dependency standalone landing page*) untuk mempublikasikan dan mendistribusikan aplikasi **Rapih Windows** serta pendaftaran daftar tunggu (*waitlist*) sebelum platform cloud dinamis siap di-deploy secara penuh.

## Struktur Berkas
```
static-landing/
├── index.html                  # Halaman utama responsif (HTML5 + Tailwind CSS)
├── favicon.svg                 # Ikon situs
├── images/
│   └── rapih-app-preview.png   # Tangkapan layar antarmuka desktop Rapih
└── README.md
```

## Fitur Utama Halaman Statis:
1. **Hero & Screenshot Showcase:** Menampilkan antarmuka asli Rapih dalam bingkai window desktop modern.
2. **Interactive Text Formatter Simulator:** Pengunjung dapat mengetik dialog sastra berantakan dan melihat simulasi otomatisasi tanda petik, elipsis, dan alinea narasi langsung di browser tanpa perlu server.
3. **Tabel Perbandingan:** Membandingkan Rapih vs Pengolah Kata umum (MS Word / Google Docs).
4. **Download Section v1.0.0:** Tautan langsung unduh berkas aplikasi desktop Windows via Google Drive resmi.
5. **Teaser & Form Waitlist Rapih Cloud:** Mengumpulkan nama dan email calon pengguna beta tester (disimpan ke `localStorage` browser dan siap dihubungkan ke webhook / Google Sheets / Formspree / Mailchimp).
6. **FAQ Interaktif:** Accordion tanya-jawab seputar privasi 100% hak cipta, offline-first, dan ekspor EPUB/DOCX.

## Cara Deploy Web Statis Ini:

### 1. Cloudflare Pages / Netlify / Vercel
- Hubungkan repositori atau cukup *drag & drop* seluruh folder `static-landing` ke dasbor Cloudflare Pages atau Netlify.
- **Build command:** Kosongkan (tidak butuh build step).
- **Publish directory:** `.` atau `static-landing`.

### 2. GitHub Pages
- Aktifkan GitHub Pages pada pengaturan repositori.
- Pilih branch atau jadikan folder `static-landing` sebagai sumber publikasi.

### 3. Hosting Konvensional (cPanel / Apache / Nginx / VPS)
- Unggah seluruh isi folder `static-landing` ke dalam direktori `public_html` atau `/var/www/html`.
- Web langsung aktif secara instan dan dapat diakses dengan performa tinggi.
