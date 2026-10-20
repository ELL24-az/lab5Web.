# Praktikum 5 — JavaScript Dasar dan Manipulasi HTML

## A. Deskripsi

Praktikum ini membahas dasar-dasar JavaScript dan penerapannya pada halaman web. Materi yang dipelajari meliputi output, input pengguna, variabel, operator, fungsi, percabangan, perulangan, manipulasi DOM, dan pembuatan kalkulator nilai mahasiswa.

## B. Struktur File

- `index.html` — halaman latihan JavaScript dasar.
- `script.js` — kode JavaScript untuk latihan dasar.
- `index2.html` — halaman mini project Kalkulator Nilai Mahasiswa.
- `script2.js` — fungsi perhitungan nilai akhir dan penentuan predikat.
- `README.md` — dokumentasi praktikum.

## C. Materi Praktikum

### 1. Menampilkan Output

Menampilkan teks Hello World pada halaman HTML dan Console menggunakan JavaScript.

### 2. Alert dan Prompt

Menggunakan `alert()` untuk menampilkan pesan dan `prompt()` untuk menerima input dari pengguna.

### 3. Operasi Aritmetika

Melakukan operasi penjumlahan, pengurangan, perkalian, pembagian, dan modulus.

### 4. Percabangan If-Else

Memeriksa nilai mahasiswa untuk menentukan apakah mahasiswa lulus atau belum lulus.

### 5. Percabangan Switch

Memilih keluaran berdasarkan angka yang dimasukkan pengguna.

### 6. Bilangan Genap dan Ganjil

Memeriksa jenis bilangan menggunakan operator modulus (`%`).

### 7. Mengubah Warna Latar

Mengubah warna latar halaman menggunakan JavaScript dan manipulasi DOM.

### 8. Menghitung Total Menu

Menghitung total harga makanan berdasarkan pilihan checkbox yang dicentang pengguna.

Menu yang tersedia:

- Ayam Goreng — Rp5.000
- Tempe — Rp500
- Telur Dadar — Rp2.500
- Es Teh — Rp3.000
- Mi Goreng — Rp6.000

## D. Mini Project: Kalkulator Nilai Mahasiswa

Mini project ini menghitung nilai akhir berdasarkan nilai Tugas, UTS, dan UAS dengan bobot:

- Tugas: 30%
- UTS: 30%
- UAS: 40%

### Ketentuan Predikat

- A: nilai minimal 85.
- B: nilai minimal 75.
- C: nilai minimal 60.
- D: nilai minimal 50.
- E: nilai di bawah 50.

Status kelulusan ditentukan berdasarkan nilai akhir. Nilai minimal 60 dinyatakan lulus, sedangkan nilai di bawah 60 dinyatakan belum lulus.

## E. Jawaban Pertanyaan

### 1. Apa fungsi JavaScript dalam pengembangan web?

JavaScript berfungsi membuat halaman web menjadi interaktif dan dinamis, misalnya menampilkan pesan, memproses input pengguna, dan mengubah tampilan halaman.

### 2. Apa perbedaan `var`, `let`, dan `const`?

- `var` digunakan untuk mendeklarasikan variabel dengan cakupan fungsi dan dapat dideklarasikan ulang.
- `let` digunakan untuk variabel yang nilainya dapat diubah.
- `const` digunakan untuk variabel yang tidak dapat diberi nilai ulang setelah dideklarasikan.

### 3. Apa fungsi `console.log()`?

`console.log()` digunakan untuk menampilkan informasi atau hasil program pada Console browser sehingga memudahkan pengujian dan pemeriksaan kode JavaScript.

### 4. Apa perbedaan `if-else` dan `switch`?

`if-else` digunakan untuk menjalankan kode berdasarkan kondisi tertentu, sedangkan `switch` digunakan untuk memilih tindakan berdasarkan kecocokan nilai dengan beberapa pilihan kasus.

### 5. Apa fungsi perulangan `for` dan `while`?

Perulangan `for` digunakan untuk menjalankan kode berulang kali dengan inisialisasi, kondisi, dan perubahan nilai. Perulangan `while` menjalankan kode selama kondisi yang ditentukan masih benar.

### 6. Apa yang dimaksud dengan DOM?

DOM (_Document Object Model_) adalah representasi dokumen HTML dalam bentuk objek yang dapat diakses dan dimanipulasi menggunakan JavaScript, misalnya untuk mengubah teks, warna, atau elemen halaman.

### 7. Bagaimana cara memvalidasi input agar nilai berada pada rentang 0–100?

Validasi dilakukan dengan memeriksa apakah input berupa angka dan nilainya tidak kurang dari 0 atau lebih dari 100. Jika nilai tidak memenuhi ketentuan tersebut, program menampilkan pesan bahwa input tidak valid.

Contoh kode:

```javascript
const inputNilai = prompt("Masukkan nilai (0-100):");
const nilai = Number(inputNilai);

if (
  inputNilai === null ||
  inputNilai.trim() === "" ||
  Number.isNaN(nilai) ||
  nilai < 0 ||
  nilai > 100
) {
  console.log("Input nilai tidak valid.");
} else {
  console.log("Input nilai valid.");
}
```

## F. Cara Menjalankan Program

1. Simpan seluruh file dalam satu folder.
2. Buka folder menggunakan Visual Studio Code.
3. Jalankan `index.html` melalui browser atau ekstensi Live Server.
4. Coba fitur-fitur yang tersedia pada halaman.
5. Tekan F12 dan pilih tab Console untuk melihat output JavaScript.
6. Buka `index2.html` untuk mencoba kalkulator nilai mahasiswa.

## G. Pengujian

Pengujian dilakukan menggunakan beberapa kondisi:

- Memasukkan nama dan mencoba input kosong.
- Menguji operasi aritmetika.
- Memasukkan nilai yang berbeda untuk menguji percabangan.
- Mencoba bilangan genap dan ganjil.
- Memilih beberapa menu makanan untuk memeriksa total harga.
- Menguji kalkulator nilai dengan kombinasi nilai Tugas, UTS, dan UAS yang berbeda.

## H. Kesimpulan

Praktikum ini memperkenalkan penggunaan JavaScript untuk membuat halaman web lebih interaktif. Melalui latihan yang dilakukan, JavaScript dapat digunakan untuk mengolah input pengguna, melakukan perhitungan, menjalankan percabangan dan perulangan, serta memanipulasi elemen HTML. Mini project kalkulator nilai mahasiswa menerapkan fungsi dan operasi aritmetika untuk menghitung nilai akhir, predikat, dan status kelulusan.
