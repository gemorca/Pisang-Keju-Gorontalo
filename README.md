<div align="center">

<img src="image/logo-pisang-keju.jpg" alt="Logo Pisang Keju Gorontalo" width="120">

# 🍌🧀 Pisang Keju Gorontalo

**Website pemesanan pisang keju premium khas Gorontalo.**
Renyah di luar, lembut di dalam, kejunya melimpah.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Responsive](https://img.shields.io/badge/Responsive-Mobile%20Friendly-FFC107?style=for-the-badge)

<img src="image/spg.png" alt="Pisang Keju Gorontalo" width="420">

</div>

---

## 📖 Tentang Proyek

**Pisang Keju Gorontalo** adalah landing page sekaligus sistem pemesanan sederhana untuk usaha pisang keju di Kota Gorontalo. Pelanggan dapat melihat menu, memilih topping, membayar melalui QRIS, lalu mengirim bukti pembayaran langsung ke admin lewat WhatsApp, semuanya tanpa backend dan tanpa instalasi.

Website ini murni *static site* (HTML, CSS, dan JavaScript), sehingga ringan, cepat, dan mudah di-hosting di mana saja.

## ✨ Fitur Utama

- **Desain responsif**: tampil rapi di ponsel, tablet, maupun desktop, lengkap dengan menu hamburger.
- **Katalog menu**: dua kategori produk (Pisang Goreng dan Pisang Nugget) dengan empat varian rasa.
- **Pemesanan via WhatsApp**: pesanan dan bukti pembayaran dikirim ke admin dengan pesan yang sudah terformat otomatis.
- **Pilihan topping**: pelanggan memilih satu topping tambahan (Keju, Oreo, Milo, atau Kacang) sebelum membayar.
- **Pembayaran QRIS**: QR code ditampilkan dalam modal dan bisa diunduh.
- **Deteksi jam operasional**: saat toko tutup, pesanan ditolak dan muncul pemberitahuan otomatis.
- **Salam otomatis**: pesan WhatsApp menyesuaikan sapaan Pagi, Sore, atau Malam sesuai waktu pemesanan.
- **Galeri produk**: slider gambar dengan tombol navigasi.
- **Testimoni pelanggan**: pengunjung dapat memberi ulasan dan rating bintang, tersimpan di browser lewat `localStorage`.
- **Animasi halus**: efek muncul saat *scroll* menggunakan AOS.
- **SEO dan Open Graph**: meta tag lengkap agar tautan tampil menarik saat dibagikan.

## 🍽️ Menu dan Harga

| Kategori | Varian | Harga |
|---|---|---|
| **Pisang Goreng** | Coklat, Tiramisu, Greentea, Palm Sugar | Rp 17.000 |
| **Pisang Nugget** | Coklat, Tiramisu, Greentea, Palm Sugar | Rp 15.000 |

**Topping tambahan:** Keju · Oreo · Milo · Kacang

## 🔄 Alur Pemesanan

```
Pilih menu → Pilih topping → Bayar via QRIS → Kirim bukti ke WhatsApp → Pesanan diproses
```

1. Pelanggan menekan tombol **Pesan via WhatsApp** pada menu pilihan.
2. Sistem mengecek jam operasional. Jika toko tutup, muncul pemberitahuan.
3. Pelanggan memilih satu topping tambahan.
4. Modal pembayaran menampilkan **QRIS** untuk dipindai atau diunduh.
5. Setelah membayar, pelanggan menekan **Kirim Bukti Pembayaran** dan WhatsApp terbuka dengan pesan siap kirim.

## 🗂️ Struktur Proyek

```
.
├── index.html          # Halaman utama
├── css/
│   └── style.css       # Seluruh gaya tampilan
├── js/
│   └── script.js       # Logika pemesanan, modal, galeri, dan testimoni
└── image/
    ├── logo-pisang-keju.jpg
    ├── spg.png
    ├── pisgor_tiramisu_oreo.jpg
    ├── pisnug_tiramisu_oreo.jpg
    └── qris-code.jpeg
```

## 🚀 Cara Menjalankan

Tidak perlu instalasi apa pun.

**Cara cepat:** unduh atau *clone* repositori ini, lalu buka `index.html` di browser.

```bash
git clone https://github.com/gemorca/pisang-keju-gorotanlo.git
cd pisang-keju-gorontalo
```

**Atau jalankan dengan server lokal:**

```bash
# Python
python -m http.server 8000

# Node.js
npx serve .
```

Lalu buka `http://localhost:8000`.

## ⚙️ Kustomisasi

| Yang ingin diubah | Lokasi |
|---|---|
| Nomor WhatsApp admin untuk pemesanan | variabel `number` di fungsi `sendProofWA()` pada `js/script.js` |
| Jam operasional toko | kondisi `hour >= 23 \|\| hour < 15` di fungsi `orderWA()` pada `js/script.js` |
| Harga dan nama menu | bagian `.product-grid` pada `index.html` |
| Pilihan topping | bagian `#toppingModal` pada `index.html` |
| Kode QRIS | ganti file `image/qris-code.jpeg` |
| Warna tema | variabel CSS `--primary`, `--primary-dark`, `--secondary`, dan `--light` di `css/style.css` |
| Testimoni bawaan | array `defaultTestimonials` pada `js/script.js` |

## 🛠️ Teknologi

- **HTML5**, **CSS3** (Flexbox dan Grid), dan **JavaScript** (Vanilla)
- [AOS (Animate On Scroll)](https://michalsnik.github.io/aos/) untuk animasi *scroll*
- [Font Awesome](https://fontawesome.com/) untuk ikon
- [Google Fonts (Poppins)](https://fonts.google.com/specimen/Poppins) untuk tipografi

## 🌐 Deploy

Karena berupa situs statis, proyek ini dapat langsung di-hosting gratis di:

- [GitHub Pages](https://pages.github.com/)
- [Netlify](https://www.netlify.com/)
- [Vercel](https://vercel.com/)
- [Cloudflare Pages](https://pages.cloudflare.com/)

## 📍 Kontak dan Lokasi

| | |
|---|---|
| 📱 **WhatsApp** | [0823-4690-1793](https://wa.me/6282346901793) |
| 📍 **Alamat** | Jl. Piola Isa, Dulomo Selatan, Kota Utara, Kota Gorontalo |
| 🕒 **Jam Operasional** | 15.00 – 22.00 WITA |
| 📸 **Instagram** | [@pisangkeju_gtlo](https://www.instagram.com/pisangkeju_gtlo) |
| 🎵 **TikTok** | [@pisangkeju.gtlo](https://www.tiktok.com/@pisangkeju.gtlo) |

## 👤 Kredit

Seluruh proyek ini, mulai dari desain, kode, hingga konten, dibuat sepenuhnya oleh:

**Moh. Agil S. Abdul**
[GitHub](https://github.com/gemorca) · [Instagram](https://instagram.com/mohammadagill)

> Pustaka pihak ketiga yang disebutkan di bagian Teknologi tetap menjadi milik masing-masing pembuatnya dan digunakan sesuai lisensi mereka.

## 📄 Lisensi

Hak Cipta © 2025 **Moh. Agil S. Abdul**. Seluruh hak dilindungi (*All Rights Reserved*).

Kode sumber, desain, gambar, dan logo dalam repositori ini dibuat dan dimiliki sepenuhnya oleh pemilik hak cipta. Anda bebas memakai, mengubah, dan membagikannya dengan tetap mencantumkan pemberitahuan hak cipta di atas.

---

<div align="center">

© 2025 Moh. Agil S. Abdul · Gorontalo, Indonesia.

</div>
