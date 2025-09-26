# Laporan Praktikum HTML dan CSS

## Identitas
**Nama:** Ni Made Dina Ayu Purnami  
**NIM:** 42430004  
**Mata Kuliah:** Konfigurasi dan Administrasi Basis Data (Praktikum Semantik HTML dan CSS)  
**Dosen Pengampu:** Ir. Gede Humaswara Prathama, S.T., M.T.  
**Universitas Pendidikan Nasional – Fakultas Teknik dan Informatika – Program Studi Teknologi Informasi**  
**Tahun:** 2025  

---

## 1. Tujuan
- Mampu membuat struktur halaman web dengan menggunakan Semantik HTML dan CSS.  
- Mampu menerapkan elemen dari Semantik HTML dan CSS.  
- Membuat halaman website yang rapi, mudah digunakan, dan terstruktur.  

---

## 2. Pendahuluan
Perkembangan teknologi informasi saat ini membuat banyak bermunculan media digital sebagai sarana komunikasi, promosi, dan penyampaian informasi. Salah satunya adalah website, yang tidak hanya berperan sebagai media informasi, tetapi juga menjadi tempat untuk mengekspresikan ide, minat, dan budaya.  

Memiliki website portofolio pribadi penting karena dapat menunjukkan identitas sekaligus profesionalitas seseorang secara lebih terstruktur. Melalui portofolio, karya, pengalaman, dan pencapaian dapat terdokumentasi dengan baik sehingga meningkatkan kredibilitas di mata orang lain. Selain itu, portofolio berbasis website mudah diakses dan dibagikan hanya dengan satu tautan, sehingga sangat membantu ketika melamar pekerjaan, mendaftar beasiswa, atau mengikuti kegiatan tertentu. Lebih dari itu, portofolio juga menjadi wadah untuk mengekspresikan kreativitas, minat, serta ciri khas pribadi yang membedakan dari orang lain.  

---

## 3. Pembahasan

### Penjelasan Kode **index.html**

1. `<!DOCTYPE html>`  
   Memberitahu browser bahwa dokumen ini adalah HTML5.

2. `<html lang="en">`  
   Tag utama pembungkus semua isi website. `lang="en"` berarti bahasa utama halaman adalah English.

3. `<head>` … `</head>`  
   Bagian kepala dokumen, berisi metadata, judul, link CSS, dll.

4. `<meta charset="UTF-8">`  
   Mengatur encoding karakter (UTF-8).

5. `<meta name="viewport" content="width=device-width, initial-scale=1.0">`  
   Membuat tampilan responsif pada berbagai perangkat.

6. `<title>`  
   Menentukan judul website yang muncul di tab browser.

7. `<header class="portfolio-slide"> … </header>`  
   Bagian header untuk menampilkan identitas awal.

8. `<nav class="top-bar"> … </nav>`  
   Wadah navigasi di bagian atas.

9. `<ul> … </ul>` dan `<li class="nav-item"> … </li>`  
   Daftar item navigasi, berisi nama, judul, dan peran pembuat portofolio.

10. `<section class="hero" id="utama"> … </section>`  
    Hero section yang menampilkan informasi utama.  
    - `<div class="title"> … </div>` → wadah judul dan tautan sosial.  
    - `<h1>` dengan `<span class="creative">Creative</span>` dan `<span class="portfolio">PORTFOLIO</span>` → membentuk judul utama.  
    - `<a class="social-link">Instagram/WhatsApp</a>` → tautan ke media sosial.  
    - `<br>` → pindah baris.  

11. `<div class="model-photo"> … </div>`  
    Menampilkan foto profil/gambar utama.  
    - `<img src="model.jpg" alt="Foto Saya" data-role="hero-image">`  
      - `src` = lokasi gambar.  
      - `alt` = teks alternatif.  
      - `data-role` = atribut khusus.  

12. `<footer class="footer"> … </footer>`  
    Bagian kaki halaman berisi informasi kontak (WhatsApp).  

13. `</body>` dan `</html>`  
    Menutup struktur HTML.  

---

### Penjelasan Kode **style.css**

1. **Import Font**  
   ```css
   @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Playfair+Display:ital,wght@1,600&display=swap');
   ```
   Mengimpor font Montserrat dan Playfair Display dari Google Fonts.

2. **Selektor Elemen Global**  
   ```css
   body { margin:0; padding:0; font-family:'Montserrat',sans-serif; background:#f5f5f5; }
   header { padding:30px 60px; }
   ```
   Mengatur tampilan dasar halaman.

3. **Selektor Kelas (Class Selector)**  
   - `.nav-item` → ukuran kecil, warna abu, bobot normal.  
   - `.portfolio` → teks besar, tebal, berwarna pink.  
   - `.creative` → teks miring, Times New Roman, ukuran sedang.  

4. **Selektor ID**  
   - `#utama` → flexbox layout, dengan padding dan jarak antar elemen.  

5. **Selektor Atribut**  
   - `img[data-role="hero-image"]` → gambar dengan batas melengkung, bayangan, dan lebar maksimum 300px.  

6. **Pseudo-class Selector**  
   - `.social-link:hover` → saat di-hover berubah warna biru dan bergaris bawah.  

7. **Pseudo-element Selector**  
   - `.footer-text::first-line` → baris pertama footer ditebalkan.  

8. **Tambahan Layout**  
   - `.top-bar ul` → daftar navigasi horizontal tanpa bullet.  
   - `.model-photo` → gambar rata tengah.  
   - `.footer` → posisi absolute di bawah dengan flexbox.  

---

## 4. Kesimpulan
Dalam praktikum ini berhasil dibuat struktur halaman web menggunakan HTML semantik dan CSS. Elemen-elemen HTML seperti header, section, dan footer dapat diatur tampilannya melalui CSS menggunakan berbagai selektor (class, id, atribut, pseudo-class, dan pseudo-element). Hasilnya, website portofolio menjadi rapi, terstruktur, mudah digunakan, serta mampu menampilkan identitas dan karya pemilik secara profesional.

