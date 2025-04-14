# Sistem Informasi Sekolah – Analisis Struktur Data & Pendekatan Pemrograman

## 1. Struktur Data untuk Pengelolaan Data Siswa Dinamis

Skenario: Jumlah siswa dalam kelas tidak tetap karena adanya proses **add/drop** selama satu semester.

### Rekomendasi Struktur Data (Dinamis)

| No | Struktur Data | Alasan Singkat                              |
|----|----------------|----------------------------------------------|
| 1  | List           | Bisa menampung data yang berubah-ubah.       |
| 2  | ArrayList      | Mudah digunakan dan fleksibel di Java.       |
| 3  | LinkedList     | Efisien untuk tambah/hapus data sering.      |
| 4  | HashMap        | Cepat mencari data siswa berdasarkan ID.     |
| 5  | Queue/Stack    | Cocok jika ada urutan masuk/keluar data.     |

---

## 2. Faktor Pemilihan Prosedural vs OOP untuk Sistem Sekolah

Skenario: Sistem mencakup **pendaftaran siswa baru**, **manajemen data siswa**, **penjadwalan kelas**, dan **pengelolaan nilai**.

### Faktor Pertimbangan

| No | Faktor                           | Penjelasan Singkat                                  |
|----|----------------------------------|-----------------------------------------------------|
| 1  | Kompleksitas Sistem             | OOP lebih rapi untuk sistem besar.                  |
| 2  | Relasi antar Data               | OOP cocok karena banyak entitas saling berhubungan. |
| 3  | Pengembangan Jangka Panjang     | OOP lebih mudah dikelola dan dikembangkan.          |
| 4  | Reusability (Kode yang bisa dipakai ulang) | Class OOP bisa digunakan ulang.         |
| 5  | Tim & Kolaborasi                | OOP memudahkan pembagian tugas dan kolaborasi.      |
