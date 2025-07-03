# unity
Corona Dodge (atau Nama Game Anda)
Sebuah game 2D endless runner sederhana yang dibuat dengan Unity di mana pemain harus menghindari rintangan untuk mendapatkan skor tertinggi. Game ini dibuat sebagai proyek belajar untuk memahami mekanisme dasar Unity.

Daftar Isi
Tentang Game

Fitur

Cara Bermain

Dibuat Menggunakan

Struktur Proyek

Setup & Instalasi

Lisensi

Tentang Game
Dalam game ini, Anda mengontrol sebuah suntikan (Player) yang bergerak secara vertikal. Tujuannya adalah untuk bertahan hidup selama mungkin dari rintangan-rintangan yang muncul secara acak dari sisi kanan layar. Semakin lama Anda bertahan, semakin tinggi skor yang Anda dapatkan. Game berakhir ketika pemain menabrak salah satu rintangan.

Fitur
Gerakan Pemain Vertikal: Kontrol pemain yang responsif hanya pada sumbu Y.

Skor Berbasis Waktu: Skor akan terus bertambah seiring waktu pemain bertahan hidup.

Spawn Rintangan Acak: Rintangan muncul secara berkala pada posisi vertikal yang acak, membuat setiap sesi permainan unik.

Looping Background: Latar belakang yang bergerak terus-menerus untuk memberikan ilusi gerakan tanpa akhir.

Sistem Game Over & Restart: Ketika pemain hancur, panel Game Over akan muncul dengan opsi untuk memulai ulang permainan.

Musik Latar Persisten: Musik latar akan terus bermain bahkan setelah permainan di-restart, tanpa memulai dari awal (menggunakan Singleton Pattern).

Manajemen Scene: Memuat ulang scene permainan saat ini untuk fungsionalitas restart.

Cara Bermain
Gerak ke Atas: Tekan tombol W atau Panah Atas.

Gerak ke Bawah: Tekan tombol S atau Panah Bawah.

Tujuan: Hindari semua rintangan yang datang untuk mencapai skor setinggi mungkin!

Dibuat Menggunakan
Game Engine: Unity Engine (versi 2022.3.6f1 berdasarkan screenshot Anda)

Bahasa: C#

Struktur Proyek
Berikut adalah penjelasan singkat dari skrip-skrip utama yang digunakan dalam game ini:

Player.cs: Mengatur gerakan pemain secara vertikal berdasarkan input dari keyboard.

Obstacle.cs: Mengatur logika untuk rintangan. Skrip ini akan menghancurkan pemain jika terjadi tabrakan, dan menghancurkan dirinya sendiri jika menyentuh batas layar.

SpawnObstacles.cs: Bertanggung jawab untuk memunculkan prefab rintangan secara berkala pada posisi Y yang acak di luar layar.

LoopingBackground.cs: Menggerakkan tekstur material latar belakang untuk menciptakan efek scrolling atau looping yang tak terbatas.

CameraMovement.cs: Menggerakkan kamera ke kanan dengan kecepatan konstan (jika digunakan untuk membuat ilusi pemain bergerak maju).

ScoreManager.cs: Menghitung skor berdasarkan waktu bertahan hidup pemain dan menampilkannya ke UI Text.

GameOver.cs: Mendeteksi jika GameObject pemain sudah tidak ada lagi di scene, lalu menampilkan panel UI Game Over dan menyediakan fungsi untuk me-restart permainan.

BackgroundMusic.cs: Menggunakan pola Desain Singleton untuk memastikan hanya ada satu instance musik latar di seluruh sesi permainan dan tidak ikut hancur saat memuat ulang scene.

Setup & Instalasi
Untuk menjalankan proyek ini di komputer Anda:

Clone repositori ini:

Bash

git clone https://link-ke-repositori-ini.git
Buka proyek di Unity Hub:

Buka Unity Hub.

Klik "Open" atau "Add project from disk".

Arahkan ke folder yang baru saja Anda clone.

Pastikan versi Unity sesuai:

Proyek ini dibuat menggunakan Unity 2022.3.6f1. Pastikan Anda memiliki versi ini atau yang kompatibel.

Jalankan Game:

Buka scene utama (misalnya SampleScene) dari jendela Project.

Tekan tombol Play di Unity Editor.
