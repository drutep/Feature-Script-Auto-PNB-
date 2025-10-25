# Dokumentasi Lengkap Fitur PNB Script

PNB Script adalah alat otomatisasi yang dirancang untuk membantu proses farming di Growtopia dengan berbagai fitur canggih. Berikut adalah penjelasan lengkap dari setiap fitur yang tersedia.

---

## Pengaturan Utama
Pengaturan ini mencakup konfigurasi dasar yang diperlukan agar script dapat berjalan dengan baik.

- **Posisi Break (X/Y)**:  
  Koordinat tempat bot akan memulai proses farming atau breaking block. Pastikan koordinat ini sesuai dengan lokasi yang diinginkan di world Anda.

- **ID Background**:  
  ID dari background block yang digunakan untuk mendeteksi lokasi magplant. Default-nya adalah `12840`. Pastikan background ini ada di world Anda untuk mendukung deteksi otomatis.

- **Posisi Telephone (X/Y)**:  
  Koordinat telephone di world Anda yang digunakan untuk mengonversi gems menjadi Diamond Lock (DL) atau Blue Gem Lock (BGL). Pastikan telephone berada di lokasi yang mudah dijangkau.

- **Batas Maksimal Gems**:  
  Jumlah maksimal gems yang dapat dimiliki sebelum script secara otomatis mengonversinya menjadi DL atau BGL. Default-nya adalah `2.2 miliar`.

- **Drop Gems**:  
  Pilihan untuk menentukan apakah gems akan dijatuhkan (0) atau langsung diambil (1).  
  - `0`: Gems akan dijatuhkan di world.  
  - `1`: Gems akan langsung diambil oleh bot.

- **Sembunyikan Pemain**:  
  Menyembunyikan pemain lain di world untuk mengurangi gangguan visual. Aktifkan dengan nilai `1`.

- **Sembunyikan Drop Item**:  
  Menyembunyikan item yang jatuh di world untuk mengurangi lag. Aktifkan dengan nilai `1`.

- **Anti Lag**:  
  Mengaktifkan fitur anti-lag untuk meningkatkan performa script, terutama di world dengan banyak objek. Aktifkan dengan nilai `1`.

---

## Pengaturan Opsional
Fitur tambahan yang dapat diaktifkan sesuai kebutuhan untuk meningkatkan efisiensi farming.

- **Ambil Black Gems**:  
  Script akan secara otomatis mengambil Black Gems yang jatuh di world. Cocok untuk farming yang menghasilkan Black Gems.

- **Konversi ke DL**:  
  Mengonversi gems menjadi Diamond Lock secara otomatis menggunakan telephone. Pastikan gems Anda mencukupi untuk konversi.

- **Konversi ke BGL**:  
  Mengonversi gems menjadi Blue Gem Lock secara otomatis menggunakan telephone. Fitur ini berguna untuk mengelola gems dalam jumlah besar.

- **Auto Bank**:  
  Menyetorkan Blue Gem Lock (BGL) ke bank secara otomatis untuk keamanan dan pengelolaan yang lebih baik.

- **Hilangkan Animasi**:  
  Menghilangkan animasi saat breaking atau farming untuk mengurangi lag dan meningkatkan performa.

- **Hilangkan Pesan Collected**:  
  Menyembunyikan pesan "Collected" yang muncul saat farming untuk mengurangi gangguan visual.

- **Tunggu Gems Maksimal**:  
  Script akan menunggu hingga jumlah gems mencapai batas maksimal sebelum melakukan konversi ke DL atau BGL.

- **Statistik GUI**:  
  Menampilkan statistik farming secara real-time dalam jendela GUI. Statistik ini mencakup informasi seperti jumlah gems, waktu runtime, dan posisi magplant.

---

## Pengaturan Konsumsi
Fitur ini dirancang untuk memastikan bot tetap aktif dengan mengonsumsi makanan secara otomatis.

- **Ambil dari Storage**:  
  Jika makanan habis, script akan secara otomatis mengambil makanan dari world storage yang telah ditentukan.

- **Nama World Storage**:  
  Nama world tempat makanan disimpan. Pastikan world ini dapat diakses oleh bot.

- **Konsumsi Otomatis**:  
  Mengaktifkan konsumsi makanan secara otomatis untuk menjaga efek buff tetap aktif.

- **Konfigurasi Makanan**:  
  Anda dapat mengatur jenis makanan yang digunakan dan posisi vending machine untuk setiap makanan.  
  - **Arroz** (ID: 4604): Makanan ini dapat diaktifkan/dinonaktifkan sesuai kebutuhan.  
  - **Clover** (ID: 528): Memberikan buff tambahan untuk farming.  
  - **Songpyeon** (ID: 1056): Pilihan lain untuk buff farming.  
  Pastikan posisi vending machine telah dikonfigurasi dengan benar.

---

## Pengaturan Webhook
Fitur ini memungkinkan integrasi dengan Discord untuk menerima notifikasi real-time.

- **Gunakan Webhook**:  
  Mengaktifkan pengiriman notifikasi ke Discord webhook. Cocok untuk memantau aktivitas farming dari jarak jauh.

- **Delay Webhook**:  
  Waktu jeda antar pengiriman notifikasi ke Discord (dalam menit). Default-nya adalah `5 menit`.

- **URL Webhook Info**:  
  URL webhook Discord untuk menerima informasi farming, seperti jumlah gems yang diperoleh.

- **URL Webhook Disconnect/Reconnect**:  
  URL webhook Discord untuk menerima notifikasi saat terjadi disconnect atau reconnect.

- **User ID Discord**:  
  ID pengguna Discord yang akan disebutkan dalam notifikasi disconnect.

- **Message ID**:  
  ID pesan Discord yang digunakan untuk mode edit. Jika tidak diatur, script akan mengirim pesan baru setiap kali.

- **Mode Webhook Info**:  
  Pilihan antara:  
  - `edit`: Mengedit pesan yang sudah ada.  
  - `spam`: Mengirim pesan baru setiap kali.

---

## Tips Penggunaan
1. **Konfigurasi Awal**:  
   Atur posisi break, deteksi magplant, dan pengaturan telephone sebelum menjalankan script.

2. **Pengaturan Makanan**:  
   Pastikan posisi vending machine makanan telah diatur jika menggunakan fitur konsumsi otomatis.

3. **Aktifkan Fitur yang Dibutuhkan**:  
   Sesuaikan pengaturan opsional dengan kebutuhan farming Anda.

4. **Gunakan Webhook**:  
   Jika ingin memantau aktivitas farming dari jarak jauh, pastikan webhook telah dikonfigurasi dengan benar.

5. **Pantau Statistik**:  
   Gunakan GUI untuk memantau statistik farming secara real-time.

---

## Catatan Penting
- Jangan mengubah ID item di tabel makanan untuk menghindari error.
- Jaga kerahasiaan URL webhook Anda agar tidak disalahgunakan.
- Pastikan koordinat telephone sudah benar untuk mendukung konversi otomatis.
- Fitur anti-lag dapat memengaruhi tampilan visual, tetapi meningkatkan performa.
- World storage harus dapat diakses dan berisi item yang diperlukan untuk konsumsi otomatis.

---

Dengan memahami fitur-fitur di atas, Anda dapat memaksimalkan efisiensi farming menggunakan PNB Script. Pastikan semua pengaturan telah disesuaikan dengan kebutuhan Anda sebelum menjalankan script.
