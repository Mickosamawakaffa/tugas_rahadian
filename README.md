# TokoKita — Toko Online Sederhana Berbasis Web

> **Aplikasi E-Commerce Berbasis Web dengan Implementasi Array Struct, Bubble Sort, Binary Search, Konsep Pointer, dan Log Proses Algoritma.**

Repository ini berisi implementasi web marketplace modern (*single-file HTML/CSS/JS*) yang menggabungkan desain UI/UX e-commerce kontemporer dengan konsep dasar struktur data dan algoritma.

---

## 🌟 Fitur Utama

### 🛍️ Antarmuka Pengguna (UI/UX)
- **Desain Modern & Terang**: Terinspirasi dari marketplace besar Indonesia (Tokopedia & Shopee) dengan palet warna hijau profesional (`#03AC0E`), kartu produk rapi, serta tipografi *Plus Jakarta Sans*.
- **Responsive Design**: Tampilan fleksibel dan nyaman diakses baik melalui smartphone maupun desktop/laptop.
- **Hero Carousel Otomatis**: Banner promo dengan navigasi titik dan tombol geser.
- **Kategori Interaktif**: Filter produk instan berdasarkan kategori (Semua, Elektronik, Komputer, Aksesoris, Audio).
- **Keranjang Belanja (Drawer)**: Slide-out cart dari sisi kanan dengan counter badge, kontrol kuantitas, dan kalkulasi subtotal.
- **Sistem Notifikasi Toast**: Notifikasi animasi halus saat produk berhasil ditambahkan atau terjadi aksi penting.

### 🧠 Implementasi Struktur Data & Algoritma
1. **Array of Struct**:
   - Data produk dikelola dalam bentuk *array of struct/object* yang dibuat melalui factory function `buatProduk(kode, nama, kategori, harga, stok, gambar, diskon, rating, terjual, lokasi)`.
   - Mengelola minimal 12+ produk katalog lengkap.
2. **Konsep Pointer / Reference**:
   - Variabel referensi `ptrProdukDipilih` bertindak sebagai pointer yang menunjuk langsung ke objek produk di array memori yang sedang dipilih pengguna.
   - Status pointer ditampilkan secara visual di panel status algoritma.
3. **Bubble Sort**:
   - Pengurutan data produk secara interaktif:
     - Harga: Termurah → Termahal
     - Harga: Termahal → Termurah
     - Nama: A → Z
     - Stok: Terbanyak → Tersedikit
   - Setiap pertukaran (*swap*) dan perbandingan (*compare*) dicatat secara rinci.
4. **Binary Search**:
   - Pencarian cepat $O(\log n)$ berdasarkan **Kode Produk** (contoh: `P001`, `P005`).
   - Algoritma otomatis memverifikasi dan mengurutkan data terlebih dahulu sebelum melakukan pencarian biner, membagi rentang pencarian (*low, mid, high*) di setiap langkah.
5. **Sequential Search**:
   - Pencarian fleksibel untuk nama atau kata kunci produk umum.
6. **Live Terminal & Process Log**:
   - Panel terminal interaktif di bagian bawah halaman yang menampilkan detail langkah eksekusi algoritma, metrik perbandingan (*comparisons*), pertukaran (*swaps*), iterasi, dan waktu eksekusi dalam milidetik.

---

## 🚀 Cara Menjalankan

Tidak memerlukan instalasi framework atau backend khusus. Cukup gunakan browser apa pun:

### Opsi 1: Buka Langsung (Standalone)
Klik dua kali file `index.html` untuk langsung membukanya di browser favorit Anda (Chrome, Edge, Firefox, Safari).

### Opsi 2: Menggunakan PHP Built-in Server (Laragon / Terminal)
```bash
# Jalankan server lokal
php -S 127.0.0.1:8000

# Buka URL di browser
http://127.0.0.1:8000/index.html
```

### Opsi 3: Menggunakan VS Code Live Server
Klik kanan pada file `index.html` dan pilih **"Open with Live Server"**.

---

## 📁 Struktur Berkas

```
tugas_rahadian/
│
├── index.html        # File utama (HTML5, Vanilla CSS, dan Vanilla JavaScript)
├── .gitignore        # Konfigurasi file yang diabaikan Git
└── README.md         # Dokumentasi proyek
```

---

## 💻 Lisensi & Pembuat

Dibuat untuk keperluan pembelajaran struktur data dan algoritma pemrograman web. Bebas dipelajari dan dikembangkan lebih lanjut.
