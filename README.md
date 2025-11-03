# Personal Portfolio Website — Nabilla Chairunisa

Website portfolio ini dikembangkan untuk menampilkan informasi pribadi, latar pendidikan, proyek, serta keahlian secara profesional dan responsif. Seluruh konten disajikan dalam satu halaman (single-page layout) agar pengunjung dapat mengenal profil secara ringkas namun informatif.

Proyek ini merupakan bagian dari tugas mata kuliah Praktikum Pemrograman Web di Program Studi Teknik Informatika, Universitas Lampung. Tujuan utamanya adalah untuk memahami struktur dasar pengembangan website menggunakan HTML dan CSS, serta mempraktikkan prinsip desain antarmuka yang bersih, sederhana, dan mudah dikembangkan.

## Biodata

**Nama:** Nabilla Chairunisa  
**NPM:** 2315061022  
**Universitas:** Universitas Lampung  
**Program Studi:** Teknik Informatika  
**Konsentrasi:** Rekayasa Perangkat Lunak (RPL)

## Struktur Folder
```plaintext
TAPercobaan2_PW-B/
│
├── index.html       → Halaman utama website portfolio
├── style.css        → File stylesheet untuk tampilan visual
├── photo.jpg        → Foto profil yang ditampilkan di halaman utama
└── README.md        → Dokumentasi proyek
```

## Fitur Website

- **Header / Navbar:** Menampilkan nama, NPM, serta tautan kontak seperti email, LinkedIn, dan GitHub.
- **Profile Section:** Menjelaskan profil singkat dan aktivitas perkuliahan, termasuk keaktifan organisasi.
- **Projects Section:** Menampilkan daftar proyek yang pernah dikerjakan, seperti WorkHub dan Smart Digital Library, beserta deskripsi, teknologi, dan tujuannya.
- **Education Section:** Menyajikan informasi pendidikan di Universitas Lampung beserta IPK terkini.
- **Skills Section:** Menguraikan kemampuan teknis dalam kategori seperti Programming Languages, Web Development, dan Tools.
- **Footer:** Berisi hak cipta tahun 2025 atas nama pengembang.

# Instalasi dan Pengelolaan Proyek dengan Git
**1. Konfigurasi awal Git**
Sebelum menggunakan Git untuk melakukan commit, dilakukan konfigurasi identitas pengguna agar setiap perubahan yang dikirimkan ke repositori memiliki informasi pembuatnya.

```plaintext
User@WINDOWS-U6C0O0Q MINGW64 ~/TAPercobaan2_PW-B (main)
$ git config --global user.name  "NabillaChai"

User@WINDOWS-U6C0O0Q MINGW64 ~/TAPercobaan2_PW-B (main)
$ it config --global user.email  "bilanisa23@gmail.com"
bash: it: command not found

User@WINDOWS-U6C0O0Q MINGW64 ~/TAPercobaan2_PW-B (main)
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
```
**2. Membuat Folder dan Inisialisasi Repository** 
```plaintext
mkdir TAPercobaan2_PW-B
cd TAPercobaan2_PW-B
git init
```
Langkah ini membuat folder proyek baru bernama TAPercobaan2_PW-B dan menginisialisasi Git di dalamnya.
Setelah menjalankan git init, terbentuk folder .git/ yang menyimpan seluruh riwayat versi proyek.

**3. Menambahkan File Pertama dan Commit Awal**
```plaintext
git add index.html
git commit -m "buat struktur dasar halaman portfolio"
```
Tahap ini menambahkan file pertama (index.html) yang berisi struktur awal website portfolio, kemudian disimpan sebagai commit pertama dalam riwayat Git.

**4. Membuat dan Menyimpan Styling**
```plaintext
git add .
git commit -m "tambahkan styling utama dan animasi untuk portfolio"
```
Menambahkan file style.css untuk memberikan tampilan visual dan efek animasi pada website. Commit kedua mencatat perubahan tersebut ke dalam repository lokal.
 
**5. Menghubungkan ke Repository GitHub**
```plaintext
git remote add origin https://github.com/NabillaChai/TAPercobaan2_PW-B
git branch -m main
git push -u origin main
```
Langkah ini menghubungkan repository lokal ke repository GitHub dengan alamat tersebut.Branch default awalnya bernama master, kemudian diganti menjadi main agar sesuai standar GitHub modern.
Perintah git push -u origin main mengunggah seluruh commit dari lokal ke GitHub.

**6. Membuat Branch Baru untuk Pengembangan Konten**
```plaintext
git checkout -b feature/content-update
```
Branch baru bernama feature/content-update dibuat untuk menambahkan konten utama website seperti proyek, pendidikan, dan keahlian tanpa mengganggu branch utama (main).

**7. Menambahkan dan Menggabungkan Konten**
```plaintext
git add .
git commit -m "isi konten portfolio dengan project, pendidikan, dan keahlian"
git checkout main
git merge feature/content-update
```
Menambahkan seluruh pembaruan menggunakan git add . agar semua file yang diubah tercatat.
Melakukan commit dengan pesan deskriptif untuk menyimpan perubahan tersebut.
Berpindah kembali ke branch utama (main) dan menggabungkan hasilnya dengan git merge, sehingga semua pembaruan dari branch fitur menjadi bagian dari versi utama proyek.

**8. Menghapus Branch yang Sudah Digabungkan**
```plaintext
git branch -d feature/content-update
```
Setelah proses penggabungan berhasil dan tidak ada konflik, branch feature/content-update dihapus karena seluruh perubahannya sudah menjadi bagian dari branch utama (main).

**9. Menambahkan Foto Profil**
```plaintext
git add photo.jpg
git commit -m "menambahkan foto profil"
```
Menambahkan file gambar (photo.jpg) yang digunakan sebagai foto profil di halaman utama.

**10. Membuat dan Mengisi README.md**
```plaintext
touch README.md
git add README.md
git commit -m "menambahkan deskripsi proyek"
git commit -m "langkah-langkah instalasi dan penggunaan"
```
File README.md dibuat sebagai dokumentasi proyek. Isinya menjelaskan deskripsi website portfolio, struktur folder, dan tujuan pembuatannya.

**11. Mengunggah Seluruh Perubahan ke GitHub**
```plaintext
git push origin main
```
Semua perubahan (termasuk file HTML, CSS, gambar, dan dokumentasi) diunggah ke branch main di repository GitHub.
 

# Menampilkan Visualisasi Riwayat Commit
<img width="820" height="225" alt="image" src="https://github.com/user-attachments/assets/75c1cdf9-6e3f-4c17-afb7-cec7a0d9aa45" />





