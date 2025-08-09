# 📦 Tutorial Menjalankan fathir-obf-v1 di Termux

## 📋 Persyaratan
Pastikan Termux sudah terinstall dan update repository.

```bash
pkg update && pkg upgrade



1️⃣ Install Paket Dasar

Pasang Node.js dan Git di Termux:

pkg install nodejs git




2️⃣ Clone Repository

Clone proyek dari GitHub:

git clone https://github.com/fathir-sthore/fathir-obf-v1.git




3️⃣ Masuk ke Direktori Proyek

cd fathir-obf-v1




4️⃣ Install Build Tools (opsional jika compile modul)

pkg install build-essential python




5️⃣ Install Semua Dependensi

Coba install semua dependensi:

npm install

> Jika proses ini gagal karena error isolated-vm, lanjutkan ke langkah 6.





6️⃣ Install Modul isolated-vm Tanpa Compile

Gunakan perintah ini untuk melewati proses build yang biasanya error di Termux:

npm install isolated-vm --ignore-scripts



7️⃣ Jalankan Aplikasi

Jika semua modul sudah terpasang, jalankan:

npm start

Atau:

node fathir.js




🛠 Catatan

Jika muncul error MODULE_NOT_FOUND untuk package tertentu (misalnya telegraf), install secara manual:

npm install nama_package

Gunakan Node.js versi LTS jika versi terbaru bermasalah:

pkg uninstall nodejs
pkg install nodejs-lts





✅ Selesai! Sekarang fathir-obf-v1 siap dijalankan di Termux.
