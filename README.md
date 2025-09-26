# cvnayge
# Praktikum Pemrograman Website — Curriculum Vitae (CV) Online  
**Semantic HTML & CSS**  

**Penulis:** Nayge Audrey Jemahi  
**NIM:** 42430024  
**Program Studi:** Teknologi Informasi, Fakultas Teknik dan Informatika — Universitas Pendidikan Nasional  
**Tahun:** 2025

---

## Deskripsi singkat
Repositori ini berisi laporan praktikum dan contoh implementasi sederhana sebuah **Website CV (Curriculum Vitae)** yang dibangun menggunakan **Semantic HTML5** dan **CSS**. Tujuan praktikum adalah menerapkan elemen-elemen semantik (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`) serta praktik CSS dasar untuk menghasilkan halaman CV yang rapi, responsif, dan mudah diakses.

Konten README ini merangkum konsep, struktur, dan panduan singkat menjalankan proyek berdasarkan materi praktikum.

---

## Fitur
- Struktur HTML semantik sesuai HTML5  
- Navigasi sederhana (navbar) dengan anchor ke section (`#about`, `#biodata`, `#gallery`, `#contact`)  
- Hero section dengan teks overlay pada gambar  
- Section `Tentang Saya`, `Biodata`, dan `Gallery`  
- Styling dasar untuk layout, tipografi, dan responsivitas menggunakan CSS  
- Footer berisi kontak dan hak cipta

---

## Struktur file (contoh)
```
/project-root
│
├─ index.html          # Halaman utama (CV)
├─ style.css           # Styling CSS
├─ assets/
│   ├─ hero.jpg        # Gambar hero / foto utama
│   ├─ foto1.jpg
│   └─ foto2.jpg
└─ Praktikum PEMROGRAMAN WEBSITE TGL 26 sept.pdf   # Laporan praktikum (sumber materi)
```

---

## Contoh potongan `index.html`
```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Curriculum Vitae — Nayge Audrey</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1>Nayge Audrey</h1>
    <nav>
      <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#biodata">Biodata</a></li>
        <li><a href="#gallery">Gallery</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section class="hero">
    <img src="assets/hero.jpg" alt="Foto Hero" />
    <div class="hero-text">Welcome To Nayge's Page</div>
  </section>

  <main>
    <section id="about">
      <h2>Tentang Saya</h2>
      <article>
        <p>Halo, saya Nayge. Saya seorang mahasiswi Teknologi Informasi yang menyukai traveling dan belajar teknologi serta desain.</p>
      </article>
    </section>

    <section id="biodata">
      <h2>Biodata Diri</h2>
      <article>
        <p><b>Nama:</b> Nayge Audrey Jemahi</p>
        <p><b>NIM:</b> 42430024</p>
        <!-- dst. -->
      </article>
    </section>

    <section id="gallery">
      <h2>Gallery</h2>
      <div class="gallery">
        <img src="assets/foto1.jpg" alt="foto 1"/>
        <img src="assets/foto2.jpg" alt="foto 2"/>
      </div>
    </section>
  </main>

  <footer id="contact">
    <p>©️ 2025 Nayge Audrey | Contact: nayge.audrey@gmail.com</p>
  </footer>
</body>
</html>
```

---

## Contoh gaya dasar `style.css`
Ringkasan titik-titik gaya yang digunakan dalam praktikum:
- Reset margin default (`body { margin: 0; }`)  
- Font-family: `Georgia, serif` (atau alternatif)  
- Background halaman: `#f8f6f7` / warna netral lembut  
- Header putih dengan border-bottom tipis (`border-bottom: 1px solid #ddd`)  
- Navbar: `display: flex; justify-content: center; gap: 1.5rem; list-style: none;`  
- Hero image: `width: 100%; display: block; filter: brightness(70%); position: relative;`  
- Hero text: `position: absolute; transform: translate(-50%, -50%); top: 50%; left: 50%; color: white;`  
- Section: `max-width: 800px; margin: auto; line-height: 1.6; text-align: center;`  
- Gallery: `display: flex; justify-content: center; gap: 1rem; flex-wrap: wrap;`  
- Footer: `background: #d4b8be; color: #fff; padding: 1rem; text-align: center;`

---

## Cara menjalankan (lokal)
1. Pastikan struktur file seperti contoh di atas.  
2. Buka `index.html` di peramban (browser) — cukup double-click atau buka lewat `File → Open`.  
3. Untuk pengalaman pengembangan, jalankan live server (opsional) seperti ekstensi Live Server pada VS Code.

---

## Tips pengembangan & aksesibilitas
- Selalu isi atribut `alt` pada gambar.  
- Gunakan heading (`h1`..`h6`) berurutan untuk struktur dokumen yang jelas.  
- Pastikan kontras warna teks terhadap latar cukup tinggi untuk keterbacaan.  
- Gunakan `meta viewport` agar tampilan responsif di perangkat mobile.  
- Pertimbangkan menggunakan `aria-*` attributes apabila menambahkan komponen interaktif.

---

## Kontribusi
Jika ingin menambah fitur (mis. bagian pengalaman kerja, portofolio proyek, atau memodernkan layout dengan CSS Grid/Flexbox lebih lanjut), silakan:
1. Fork repository (jika disimpan di GitHub).  
2. Buat branch fitur: `git checkout -b fitur/nama-fitur`.  
3. Commit perubahan dan buka pull request.

---

## Penulis & Referensi
Laporan praktikum dan isi README ini merujuk pada dokumen praktikum: **Praktikum PEMROGRAMAN WEBSITE TGL 26 sept.pdf**.

---

## Lisensi
Silakan tambahkan lisensi sesuai keinginan (mis. MIT, CC-BY) — jika tidak ada, proyek diasumsikan sebagai milik penulis.
