Logika dari program di atas bisa dijelaskan sebagai sebuah **sistem kasir sederhana** untuk sebuah toko yang menjual 5 jenis barang. Berikut penjelasan logika utamanya, step by step:

---

## 💡 **Tujuan Program:**
Membuat aplikasi kasir yang:
- Menampilkan daftar barang.
- Menerima input jumlah pembelian dari pengguna.
- Menghitung total harga dan diskon berdasarkan jumlah beli.
- Menampilkan rekap pesanan dan proses pembayaran.
- Menyimpan struk pembelian ke file teks.

---

## 🧠 **Logika Utama Program (alurnya):**

1. ### **Inisialisasi Barang**
   Fungsi: `initialize_items()`
   - Mengisi daftar barang dengan nama, harga, dan jumlah awal 0.
   - Misalnya:
     ```c
     {"Pensil", 2000, 0, 0}
     ```

2. ### **Menampilkan Menu**
   Fungsi: `display_menu()`
   - Menampilkan daftar barang dan menu pilihan (input nomor barang, lihat struk, edit barang, reset, keluar).

3. ### **User Memilih Barang**
   - User memasukkan nomor barang dan jumlah barang yang ingin dibeli.
   - Nilai ini disimpan di `quantity` tiap barang.

4. ### **Perhitungan Diskon**
   Fungsi: `calculate_discounts()`
   - Jika beli > 3 tapi ≤ 5 → diskon 10%.
   - Jika beli > 5 → diskon 15%.
   - Diskon dihitung berdasarkan total harga per item.

5. ### **Pengurutan Item (untuk ditampilkan secara rapi)**
   Fungsi: `sort_items()`
   - Mengurutkan barang berdasarkan `quantity` secara descending (terbanyak ke terkecil).
   - Hanya memengaruhi tampilan saat checkout.

6. ### **Proses Checkout**
   Fungsi: `process_checkout()`
   - Menampilkan rekap barang, harga, total, diskon.
   - Meminta user memasukkan uang pembayaran.
   - Menghitung kembalian.
   - Menyimpan struk pembelian ke file teks (pakai `time()` sebagai ID struk).

7. ### **Simpan Struk**
   Fungsi: `save_receipt()`
   - Menyimpan semua data pembelian ke file `struk_<timestamp>.txt`.

8. ### **Edit Jumlah Barang**
   Fungsi: `edit_selected_items()`
   - Menampilkan barang yang sudah dipilih (quantity > 0).
   - Memungkinkan user mengubah jumlahnya.

9. ### **Reset Pilihan**
   - Mengatur ulang semua `quantity` dan `discount` ke 0.

10. ### **Validasi Input**
   Fungsi: `get_valid_input()`
   - Memastikan input adalah angka dan memenuhi nilai minimum (misalnya tidak boleh bayar kurang dari tagihan).

---

## 💬 **Logika Inti Singkatnya:**

**Input Barang → Hitung Diskon → Hitung Total → Checkout & Pembayaran → Simpan Struk**

---

Kalau kamu ditanya:
> *"Apa logika dari program ini?"*

Jawaban simpel:
> Logika program ini adalah seperti sistem kasir yang memungkinkan pelanggan memilih barang, menghitung total belanja termasuk diskon jika beli banyak, dan membuat struk pembayaran yang disimpan ke file. Semua prosesnya otomatis berdasarkan input jumlah barang dan uang pembayaran dari pengguna.

---

Kalau kamu mau, aku juga bisa bantu buatkan *flowchart logika program ini*. Mau?
