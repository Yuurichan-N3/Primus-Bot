# Prime Bot - Check-in Otomatis

## Deskripsi
Prime Bot adalah bot otomatis berbasis Node.js yang dirancang untuk mengotomatiskan tugas check-in harian di platform `padolabs.org` (achievement/complete). Bot ini menggunakan Telegram untuk verifikasi keanggotaan pengguna di grup tertentu (`@sentineldiscus`) dan mendukung penggunaan proxy serta multi-threading untuk memproses beberapa token secara bersamaan. Bot ini menampilkan progres check-in dalam baris perintah dengan warna cerah dan tabel hasil, serta fitur verifikasi keamanan menggunakan kode unik.

Proyek ini dikembangkan oleh [sentineldiscus](https://t.me/sentineldiscus) dan dirancang untuk mempermudah pengguna dalam mengotomatiskan tugas harian di `padolabs.org`.

## Fitur
- **Check-in Harian Otomatis**: Melakukan check-in harian untuk semua token yang terdaftar di `data.txt`.
- **Support Multi-Threading**: Memproses beberapa token secara paralel untuk efisiensi (dapat disesuaikan jumlah thread).
- **Support Proxy**: Mendukung penggunaan proxy dari file `proxy.txt` untuk koneksi yang lebih aman atau distribusi.
- **Verifikasi Telegram**: Memerlukan verifikasi keanggotaan di grup Telegram `@sentineldiscus` dan autentikasi dengan password unik untuk keamanan.
- **Progress Bar dan Tabel**: Menampilkan progres check-in dengan bar progres interaktif dan tabel hasil di terminal, menggunakan warna cerah untuk visualisasi yang menarik.
- **Hitung Mundur 24 Jam**: Menjalankan check-in setiap 24 jam dengan hitung mundur visual.

## Prasyarat
Pastikan Anda memiliki lingkungan berikut sebelum menjalankan bot ini:
- **Node.js 14+**
- **Dependensi Node.js**: Instal dependensi berikut menggunakan `npm`:
  ```bash
  npm install axios node-telegram-bot-api crypto colors cli-progress cli-table3 gradient-string
  ```


## Instalasi
1. Cloning Repository:

```
git clone https://github.com/Yuurichan-N3/Primus-Bot.git
cd Primus_Bot
```


2. Siapkan File Data:
Buat file `data.txt` di direktori proyek dengan format satu token per baris (contoh: token untuk login ke padolabs.org).

Contoh isi data.txt:

```
token_akun_1
token_akun_2
```

(Opsional) Buat file proxy.txt untuk menyimpan proxy (contoh: http://user:pass@ip:port, satu proxy per baris).


3. Jalankan bot
   ```
   noode bot.js
   ```


   ## 📜 Lisensi  

Script ini didistribusikan untuk keperluan pembelajaran dan pengujian. Penggunaan di luar tanggung jawab pengembang.  

Untuk update terbaru, bergabunglah di grup **Telegram**: [Klik di sini](https://t.me/sentineldiscus).


---

## 💡 Disclaimer
Penggunaan bot ini sepenuhnya tanggung jawab pengguna. Kami tidak bertanggung jawab atas penyalahgunaan skrip ini.
