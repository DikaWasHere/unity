🎮 Corona Dodge (atau Ganti dengan Nama Game Anda)
Corona Dodge adalah game 2D endless runner sederhana yang dibuat menggunakan Unity. Pemain mengontrol sebuah suntikan (vaksin) untuk menghindari rintangan dan meraih skor setinggi mungkin. Game ini dikembangkan sebagai proyek pembelajaran untuk memahami mekanisme dasar Unity.

📑 Daftar Isi
Tentang Game

Fitur

Cara Bermain

Dibuat Menggunakan

Struktur Proyek

Setup & Instalasi

Lisensi

🧩 Tentang Game
Dalam game ini, pemain mengendalikan sebuah suntikan yang bergerak secara vertikal. Rintangan akan muncul dari sisi kanan layar secara acak. Pemain harus bertahan hidup selama mungkin tanpa menabrak rintangan untuk mendapatkan skor tertinggi. Permainan berakhir jika pemain bertabrakan dengan rintangan.

✨ Fitur
Gerakan Vertikal: Pemain hanya bisa bergerak ke atas dan bawah.

Skor Dinamis: Skor bertambah secara otomatis berdasarkan waktu bermain.

Rintangan Acak: Rintangan muncul secara berkala dengan posisi vertikal acak.

Latar Bergerak: Background game terus bergerak untuk menciptakan efek endless scrolling.

Sistem Game Over: UI Game Over muncul ketika pemain kalah, lengkap dengan tombol restart.

Musik Latar Persisten: Musik tetap berjalan saat restart berkat penggunaan Singleton Pattern.

Manajemen Scene: Restart dilakukan dengan me-reload scene saat ini.

🎮 Cara Bermain
Aksi	Tombol
Gerak ke Atas	W atau ↑ (Panah Atas)
Gerak ke Bawah	S atau ↓ (Panah Bawah)

Tujuan: Hindari semua rintangan dan capai skor setinggi mungkin!

🔧 Dibuat Menggunakan
Game Engine: Unity 2022.3.6f1

Bahasa Pemrograman: C#

🗂️ Struktur Proyek
Penjelasan singkat skrip utama:

Skrip	Deskripsi
Player.cs	Mengatur gerakan vertikal pemain berdasarkan input keyboard.
Obstacle.cs	Mengelola tabrakan antara pemain dan rintangan serta penghancuran diri saat melewati layar.
SpawnObstacles.cs	Memunculkan rintangan secara acak di posisi vertikal.
LoopingBackground.cs	Membuat efek scrolling pada latar belakang.
CameraMovement.cs	(Opsional) Menggerakkan kamera untuk ilusi gerakan maju.
ScoreManager.cs	Menghitung dan menampilkan skor berdasarkan waktu bermain.
GameOver.cs	Menampilkan UI Game Over dan memuat ulang permainan saat diperlukan.
BackgroundMusic.cs	Mengelola musik latar agar tetap berjalan antar restart scene menggunakan Singleton Pattern.

🛠️ Setup & Instalasi
Clone repositori ini

bash
Copy
Edit
git clone https://github.com/DikaWasHere/unity
Buka proyek di Unity Hub

Jalankan Unity Hub.

Klik Open atau Add Project from Disk.

Arahkan ke folder hasil clone tadi.

Pastikan versi Unity sesuai

Proyek ini menggunakan Unity 2022.3.6f1. Disarankan untuk menggunakan versi yang sama atau kompatibel.

Jalankan game

Buka scene utama, contoh: SampleScene.

Tekan tombol Play di Unity Editor.

📄 Lisensi
Proyek ini dikembangkan sebagai bahan belajar. Anda bebas menggunakan, memodifikasi, dan menyebarluaskan proyek ini sesuai kebutuhan.
source:Yt Hooson

