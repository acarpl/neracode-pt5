# neracode-pt5

### **Materi Flexbox dan Grid dalam CSS**

#### **1. Flexbox (Flexible Box)**
- **Konsep Utama**: Flexbox digunakan untuk membuat tata letak yang fleksibel dan responsif.
- **Cara Kerja**: Elemen dalam flexbox diatur dalam satu dimensi, baik itu horizontal (row) atau vertikal (column).

##### **Properti Utama Flexbox:**
1. **display: flex** – Mengaktifkan flexbox pada elemen induk.
2. **flex-direction** – Menentukan arah elemen fleksibel (row, column, row-reverse, column-reverse).
3. **justify-content** – Mengatur penempatan elemen secara horizontal (start, center, space-between, space-around).
4. **align-items** – Menentukan perataan elemen secara vertikal (stretch, center, baseline, start, end).
5. **flex-wrap** – Membuat elemen wrap atau membungkus jika melebihi lebar kontainer (nowrap, wrap).
6. **flex-grow, flex-shrink, flex-basis** – Mengatur ukuran relatif elemen di dalam flexbox.

##### **Studi Kasus Flexbox (Portofolio Rasya Falqi Gani):**
Misalnya, kita ingin membuat layout untuk header portofolio Rasya yang terdiri dari logo, navigasi, dan tombol kontak:
```css
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```
- Logo berada di kiri, navigasi di tengah, dan tombol kontak di kanan.

---

#### **2. CSS Grid**
- **Konsep Utama**: CSS Grid digunakan untuk membuat layout dua dimensi (baris dan kolom).
- **Cara Kerja**: Elemen dapat ditempatkan dalam posisi spesifik pada grid, memungkinkan kontrol yang lebih besar terhadap tata letak.

##### **Properti Utama Grid:**
1. **display: grid** – Mengaktifkan grid pada elemen induk.
2. **grid-template-columns** & **grid-template-rows** – Menentukan jumlah kolom dan baris.
3. **grid-gap** – Mengatur jarak antara baris dan kolom.
4. **grid-area** – Mengatur area tertentu dalam grid.
5. **grid-auto-flow** – Mengatur bagaimana elemen diisi dalam grid (row, column, dense).

##### **Studi Kasus Grid (Portofolio Rasya Falqi Gani):**
Misalnya, kita ingin membuat layout galeri portofolio dengan gambar-gambar proyek:
```css
.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 10px;
}
```
- Layout ini membagi galeri menjadi tiga kolom yang responsif dengan jarak antar elemen.

---

### **3. Figma: Desain Prototipe UI/UX**

- **Penggunaan Figma**: Figma adalah alat desain antarmuka yang digunakan untuk membuat prototipe interaktif dan mockup desain web atau aplikasi.
  
##### **Fitur Utama Figma:**
1. **Frames** – Menentukan area kerja, seperti layar atau komponen.
2. **Auto Layout** – Mengatur elemen otomatis seperti Flexbox dalam CSS.
3. **Components** – Membuat elemen yang dapat digunakan kembali (misalnya, tombol atau header).
4. **Prototyping** – Membuat interaksi antar layar (misalnya, klik tombol menuju halaman lain).

##### **Studi Kasus Figma (Portofolio Rasya Falqi Gani):**
Di Figma, Rasya dapat mendesain layout portofolio seperti ini:
1. **Frame**: Buat frame untuk halaman utama dengan header, konten, dan footer.
2. **Auto Layout**: Gunakan auto layout pada navigasi di header untuk membuatnya responsif dan fleksibel.
3. **Component**: Buat komponen seperti tombol "Kontak" yang bisa digunakan berulang di seluruh halaman.

##### **Tampilan Mockup di Figma:**
- **Header**: Logo di kiri, navigasi di tengah, dan tombol di kanan (menggunakan auto layout).
- **Section Portfolio**: Menggunakan grid untuk menampilkan proyek Rasya dengan gambar-gambar.

---

### **Tugas untuk Siswa:**
1. **Flexbox Task**: Buat header portofolio dengan logo, navigasi, dan tombol menggunakan flexbox.
2. **Grid Task**: Buat galeri proyek Rasya menggunakan grid dengan tiga kolom.
3. **Figma Task**: Desain layout halaman utama portofolio Rasya di Figma dengan auto layout.

Berikut adalah kode lengkap dan penjelasan untuk tugas siswa mengenai Flexbox, Grid, dan penggunaan Figma dengan HTML dan CSS:

---

### **Tugas Flexbox: Membuat Header Portofolio**

#### **HTML**:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio Rasya Falqi Gani</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header class="header">
        <div class="logo">
            <h1>Rasya Falqi Gani</h1>
        </div>
        <nav class="nav">
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#portfolio">Portfolio</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
        <div class="contact-btn">
            <a href="#contact" class="btn">Kontak</a>
        </div>
    </header>
</body>
</html>
```

#### **CSS**:
```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
}

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    background-color: #333;
    color: white;
}

.logo h1 {
    font-size: 24px;
}

.nav ul {
    display: flex;
    list-style: none;
}

.nav ul li {
    margin-left: 20px;
}

.nav ul li a {
    text-decoration: none;
    color: white;
}

.contact-btn .btn {
    padding: 10px 20px;
    background-color: #ff6347;
    color: white;
    text-decoration: none;
    border-radius: 5px;
}
```

#### **Penjelasan**:
- **HTML Structure**: Terdapat tiga bagian dalam header: logo, navigasi, dan tombol kontak. Elemen-elemen ini akan diatur dengan menggunakan Flexbox.
- **Flexbox**: Pada elemen `.header`, properti `display: flex` digunakan untuk membuat elemen di dalamnya fleksibel, `justify-content: space-between` mengatur agar logo, navigasi, dan tombol kontak terletak di posisi yang berjauhan secara horizontal, sedangkan `align-items: center` mengatur semua elemen agar berada di tengah secara vertikal.
  
---

### **Tugas Grid: Membuat Galeri Portofolio**

#### **HTML**:
```html
<section class="portfolio">
    <h2>My Projects</h2>
    <div class="gallery">
        <div class="project">Project 1</div>
        <div class="project">Project 2</div>
        <div class="project">Project 3</div>
        <div class="project">Project 4</div>
        <div class="project">Project 5</div>
        <div class="project">Project 6</div>
    </div>
</section>
```

#### **CSS**:
```css
.portfolio {
    padding: 50px;
    text-align: center;
}

.portfolio h2 {
    margin-bottom: 20px;
}

.gallery {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 20px;
}

.project {
    padding: 40px;
    background-color: #f4f4f4;
    border: 1px solid #ccc;
    text-align: center;
}
```

#### **Penjelasan**:
- **HTML Structure**: Galeri ini terdiri dari beberapa item proyek yang diatur dalam elemen `<div>` dengan class `.project`.
- **CSS Grid**: Elemen `.gallery` menggunakan `display: grid` untuk mengaktifkan tata letak grid. Properti `grid-template-columns: repeat(3, 1fr)` membuat tiga kolom dengan ukuran yang sama, sedangkan `grid-gap: 20px` memberikan jarak antar kolom dan baris.
  
---

### **Tugas Figma: Desain Layout Halaman Utama**

#### **Langkah-Langkah di Figma**:
1. **Membuat Frame**:
   - Buat frame baru untuk halaman utama dengan ukuran 1440x1024 px.
   - Bagian frame ini akan terdiri dari header, section portfolio, dan footer.

2. **Membuat Header**:
   - Tambahkan logo di sebelah kiri dan gunakan fitur **Auto Layout** untuk menata navigasi di tengah dan tombol di sebelah kanan.
   - Atur jarak antar elemen dengan menggunakan padding dan margin.

3. **Membuat Komponen Galeri**:
   - Buat elemen untuk tiap proyek di galeri menggunakan **Repeat Grid** atau **Auto Layout** agar setiap item berukuran sama dan teratur.
   
4. **Membuat Tombol Kontak**:
   - Buat tombol di bagian header dan jadikan sebagai **Component**, sehingga bisa digunakan berulang di berbagai halaman.

#### **Hasil Akhir**:
- **Header** dengan layout yang rapi dan responsif.
- **Galeri Proyek** dengan tampilan yang bersih dan terorganisir menggunakan grid.

---

Ini adalah contoh kode lengkap dan penjelasan untuk tugas siswa dalam mengatur layout menggunakan Flexbox dan Grid di CSS serta penggunaan Figma dalam studi kasus portofolio Rasya Falqi Gani.

---
**SEDIKIT QNA** 

"Kalau kita bicara tentang komputer, menurut kamu, apa sih bagian yang paling penting dari sebuah komputer? Bisa ceritain?"
"Kamu pernah dengar istilah 'hardware' dan 'software'? Apa yang terlintas di pikiran kamu tentang dua hal ini?"
"Nah, kalau kamu lagi pakai komputer, apa langkah pertama yang kamu lakukan untuk menyalakannya? Ada nggak tips khusus supaya komputer nggak cepat rusak?"
"Menurut kamu, kenapa sistem operasi itu penting banget buat komputer? Apa yang bakal terjadi kalau nggak ada OS?"
"Boleh cerita, alat apa aja yang pernah kamu pakai untuk menginput data di komputer? Dan menurut kamu, apa output yang paling sering kamu lihat di komputer kamu?"
"Kalau denger kata 'coding', apa sih yang terlintas di pikiran kamu? Apa menurut kamu coding itu sulit atau justru menyenangkan?"
"Kamu pernah coba nulis kode? Nah, setelah kamu menulis kode, apa sih yang terjadi di balik layar komputer?"
"Pernah dengar bahasa pemrograman kayak Python, Java, atau C++? Kalau iya, bahasa apa yang menurut kamu paling menarik, dan kenapa?"
"Gimana menurut kamu komputer bisa paham apa yang kita tulis dalam kode dan akhirnya melakukan perintah itu?"
"Saat kamu berhasil menyelesaikan satu proyek coding kecil, gimana rasanya? Apa yang paling kamu banggakan?"
"Kalau kamu kasih input ke komputer, apa yang terjadi di dalamnya sampai akhirnya dia ngasih output? Bisa ceritain dengan versi kamu sendiri?"
"Apa kamu tahu kenapa CPU sering disebut sebagai otaknya komputer? Menurut kamu, apa yang bikin CPU begitu penting?"
"Bayangin data yang kita simpan di komputer, gimana ya caranya komputer bisa ngambil dan menyimpan data itu kapan pun kita mau?"
"Kadang kita jalankan banyak program sekaligus di komputer, menurut kamu gimana caranya komputer bisa multitasking kayak gitu?"
"Dari semua yang kamu pelajari tentang komputer dan coding, apa sih yang menurut kamu paling menarik atau seru?"
"Apa tantangan terbesar yang kamu rasain waktu belajar tentang komputer? Gimana kamu menghadapi atau mengatasi hal itu?"
"Kalau kamu diberi kesempatan untuk belajar lebih dalam tentang komputer atau coding, apa sih yang paling ingin kamu eksplor?"
"Waktu berinteraksi dengan teknologi, apakah kamu merasa nyaman atau malah kadang bingung? Kenapa bisa begitu?"
"Menurut kamu, apa langkah-langkah yang bisa kamu ambil untuk lebih paham lagi soal komputer? Ada hal yang ingin kamu lakukan lebih baik?"
ORANG PINTAR ADALAH ORANG YANG PENASARAN - DENGAN MEMNACINGNYA MENGGUNAKAN PERTANYAAN, MENYELIPKAN OBROLAN PERTANYAAN DISAAT ADA WAKTU KOSONG ATAU AKWARD. MEMBUKA PEMIKIRAN PENASARAN DALAM DUNIA IT - MEMBUKA CAKRAWALA DI BIDANG IT MERUPAKAN SALAH SATU HAL YANG PENTING KARENA DUNIA IT MEMILIKI LONG TERM DIMANA SELALU BERKEMBANG DI SETIAP MASA - LEARN TILL WE DIE NEVER STOP AND NEVER SURRENDER

---

Semoga materi ini bisa membantu dalam belajar!
