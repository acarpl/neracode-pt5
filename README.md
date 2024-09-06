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

---

Semoga materi ini bisa membantu dalam mengajar!
