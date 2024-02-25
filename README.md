
# Pengaturan Zona Waktu untuk Cron Job di Server

Repository ini berisi instruksi tentang cara mengatur cron job di server agar mengikuti zona waktu Jakarta menggunakan aaPanel.

## Prasyarat

Pastikan Anda memiliki akses root atau sudo untuk server Anda.

## Langkah-langkah

### 1. Ubah Zona Waktu Server

Untuk mengatur zona waktu server ke WIB (Waktu Indonesia Barat), jalankan perintah berikut di terminal server Anda:

```
sudo timedatectl set-timezone Asia/Jakarta
```

### 2. Verifikasi Zona Waktu Server

Setelah mengubah zona waktu, verifikasi perubahan tersebut dengan perintah:

```
timedatectl
```

### 3. Atur Cron Job di aaPanel

1. Login ke dashboard aaPanel.
2. Navigasi ke menu **Cron Jobs** atau **Tugas Terjadwal**.
3. Klik **Add Cron Job** atau **Tambah Cron Job**.
4. Masukkan perintah yang ingin dijalankan dan atur waktu eksekusi. Waktu yang diatur akan mengikuti zona waktu Jakarta.

### 4. Simpan Pengaturan Cron Job

Setelah mengisi detail, klik **Save** atau **Simpan** untuk menerapkan pengaturan.

## Catatan

Perubahan zona waktu server akan mempengaruhi semua operasi berbasis waktu pada server, bukan hanya cron job.

## Dukungan

Untuk konfigurasi lanjutan atau jika mengalami kesulitan, silakan merujuk pada dokumentasi resmi aaPanel atau mendapatkan dukungan dari komunitas atau forum aaPanel.

