Berikut adalah catatan penjelasan untuk kode program **Simple Web Server dengan Go** yang dapat dimasukkan ke dalam README proyek GitHub:

---

# 🌐 **Simple Web Server dengan Go**
Ini adalah program **Web Server berbasis Go** yang menangani permintaan HTTP, termasuk penyajian file statis dan pemrosesan formulir.

## 🚀 **Fitur Utama**
✅ Menyajikan file statis dari direktori `./static`  
📩 Menangani permintaan **POST** untuk formulir (`/form`)  
👋 Menyediakan endpoint **GET** untuk `/hello`  
⚠️ Menampilkan pesan error jika halaman tidak ditemukan  

## 🏗 **Struktur Kode**
Program ini menggunakan **Go** dengan package bawaan:
- `fmt`: Menampilkan teks ke terminal dan merespons HTTP.
- `log`: Menangani logging untuk error server.
- `net/http`: Menyediakan fungsi untuk menangani HTTP request dan response.

## 📜 **Penjelasan Kode**
- **`formHandler()`** → Menangani permintaan **POST** dari formulir dan mengambil nilai dari input `name` dan `address`.
- **`helloHandler()`** → Menampilkan pesan `"Hello!"` jika pengguna mengakses `/hello` dengan metode **GET**.
- **`main()`** → 
  - Menyajikan file statis dari direktori `./static`.
  - Menetapkan handler untuk `/form` dan `/hello`.
  - Memulai server pada port **8080** menggunakan `http.ListenAndServe()`.

## 🔧 **Cara Menjalankan**
Pastikan Go sudah terinstall, lalu jalankan:
```bash
go run main.go
```
Atau build terlebih dahulu dengan:
```bash
go build -o webserver main.go
./webserver
```

---
