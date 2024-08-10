# MARI MENGENAL APA ITU GIT
>  GIT merupakan salah satu VCS (Version Control System) yang dapat mengatur dan merekam perubahan pada file atau sekumpulan file dari waktu ke waktu

<p>Sebagai seorang developer tentu kita akan sering melakukan revisi atau perubahan terhadap file kita</p>
<p>Umumnya, kita akan menggunakan duplikat file agar setiap revisi atau perubahan pada file dapat terekam. Akan tetapi, hal itu tentu dapat memakan memori yang ada di dekstop kita, sehingga dengan hadirnya git ini kita dapat mengatur perubahan pada file kita.</p>

### Sebagai contoh :
<img src="/assets/Screenshot 2024-08-11 054707.png" width="100px" alt="image"><br>

<p>Pada contoh diatas kita melakukan duplikat file setiap kali akan melakukan perubahan, hal tersebut bisa saja dilakukan akan tetapi tentu dapat memakan memory yang cukup banyak. Oleh karena itulah kita membutuhkan GIT untuk mengatur setiap versi pada file kita</p>

# LATAR BELAKANG
 > GIT memudahkan kita ketika bekrja dalam tim untuk melihat siapa dan kapan yang terakhir memodifikasi file kita dan sebagainya

## Sejarah Singkat Git

### Pengenalan
Git adalah sistem kontrol versi terdistribusi yang dikembangkan oleh Linus Torvalds, pencipta kernel Linux. Git pertama kali dirilis pada tahun 2005 dan sejak itu telah menjadi alat yang sangat populer di kalangan pengembang perangkat lunak untuk melacak perubahan dalam kode sumber selama pengembangan perangkat lunak.

### Awal Mula
Pada awal 2000-an, pengembangan kernel Linux menggunakan sistem kontrol versi terpusat yang disebut BitKeeper. Namun, pada tahun 2005, terjadi perselisihan antara komunitas pengembang kernel Linux dan pemilik BitKeeper, yang menyebabkan pencabutan lisensi gratis untuk proyek open-source. Akibatnya, Linus Torvalds memutuskan untuk membuat sistem kontrol versi baru yang memenuhi kebutuhan pengembangan kernel Linux.

### Pengembangan Git
Linus Torvalds mulai mengembangkan Git pada April 2005 dengan beberapa tujuan utama:
1. **Kecepatan**: Git dirancang untuk dapat menangani proyek dengan skala besar dengan cepat.
2. **Sederhana**: Sistem ini harus mudah dipelajari dan digunakan oleh pengembang.
3. **Dukungan Pengembangan Non-linear**: Mendukung banyak cabang (branch) dan penggabungan (merge) dengan mudah.
4. **Distribusi**: Setiap pengembang memiliki salinan penuh dari sejarah proyek, memungkinkan pengembangan terdistribusi.
5. **Integritas Data**: Setiap perubahan teracak secara kriptografi untuk melindungi integritas sejarah proyek.

### Evolusi dan Adopsi
Git dengan cepat diadopsi oleh pengembang kernel Linux dan komunitas open-source yang lebih luas karena kehandalannya. Dalam beberapa tahun, banyak proyek perangkat lunak besar lainnya mulai menggunakan Git. Salah satu pendorong utama adopsi Git adalah kemunculan platform hosting seperti GitHub (didirikan pada tahun 2008), yang menyediakan layanan kolaborasi berbasis Git dan mempermudah pengembang untuk berbagi dan berkolaborasi dalam proyek.

### Git Hari Ini
Saat ini, Git adalah sistem kontrol versi terdistribusi yang paling populer dan banyak digunakan di dunia. Git digunakan oleh berbagai macam proyek perangkat lunak, mulai dari proyek open-source hingga proyek komersial besar. Kecepatan, fleksibilitas, dan kemampuannya untuk mendukung pengembangan kolaboratif menjadikan Git alat yang sangat penting dalam dunia pengembangan perangkat lunak modern.

### Referensi
- Torvalds, Linus. “Git - Fast Version Control System.”
- Chacon, Scott, and Ben Straub. "Pro Git." Apress, 2014.
- Git Documentation: https://git-scm.com/doc


## Git Syntaks


### Perintah Dasar

#### 1. Inisialisasi Repositori
```bash
git init
```
- **Penjelasan**: Perintah ini membuat repositori Git baru di folder yang sedang kamu gunakan. Ini seperti membuat kotak penyimpanan khusus untuk proyekmu sehingga kamu bisa mulai melacak perubahan.

#### 2. Menambahkan File ke Staging Area
```bash
git add <nama-file>
```
- **Penjelasan**: Perintah ini menyiapkan file untuk di-commit. Ini seperti memilih barang-barang yang ingin kamu masukkan ke dalam kotak sebelum menutup dan menyegelnya.

#### 3. Melihat Status
```bash
git status
```
- **Penjelasan**: Perintah ini menunjukkan status terkini dari proyekmu. Kamu bisa melihat file mana yang telah diubah, mana yang siap di-commit, dan mana yang belum di-track.

#### 4. Commit Perubahan
```bash
git commit -m "Pesan commit"
```
- **Penjelasan**: Perintah ini menyimpan perubahan yang telah kamu siapkan dengan `git add`. Ini seperti menutup dan menyegel kotak penyimpananmu, serta memberi label pada kotak tersebut dengan catatan tentang isinya.

### Perintah Cabang

#### 5. Membuat Cabang Baru
```bash
git branch <nama-cabang>
```
- **Penjelasan**: Perintah ini membuat cabang baru. Anggap cabang sebagai jalur pengembangan paralel tempat kamu bisa membuat perubahan tanpa memengaruhi jalur utama.

#### 6. Berpindah ke Cabang Lain
```bash
git checkout <nama-cabang>
```
- **Penjelasan**: Perintah ini memindahkanmu ke cabang yang lain, sehingga kamu bisa bekerja di jalur pengembangan yang berbeda.

#### 7. Menggabungkan Cabang
```bash
git merge <nama-cabang>
```
- **Penjelasan**: Perintah ini menggabungkan perubahan dari satu cabang ke cabang lain. Ini seperti menggabungkan dua jalur pengembangan menjadi satu.

### Perintah Remote

#### 8. Menambahkan Remote Repository
```bash
git remote add origin <url-repo>
```
- **Penjelasan**: Perintah ini menambahkan repositori remote (online) yang bisa kamu hubungkan dengan repositorimu. Ini seperti menambahkan alamat tujuan pengiriman kotak penyimpananmu.

#### 9. Mengirim Perubahan ke Remote
```bash
git push origin <nama-cabang>
```
- **Penjelasan**: Perintah ini mengirim perubahan dari cabang lokal ke cabang remote. Ini seperti mengirim kotak penyimpananmu ke alamat tujuan yang sudah kamu tambahkan.

#### 10. Mengambil Perubahan dari Remote
```bash
git pull origin <nama-cabang>
```
- **Penjelasan**: Perintah ini mengambil dan menggabungkan perubahan dari repositori remote ke cabang lokalmu. Ini seperti menerima kotak penyimpanan dari orang lain dan menggabungkan isinya dengan milikmu.

### Perintah Lainnya

#### 11. Melihat Log Commit
```bash
git log
```
- **Penjelasan**: Perintah ini menunjukkan daftar commit yang telah dibuat dalam repositori. Ini seperti melihat catatan semua kotak penyimpanan yang telah kamu buat beserta labelnya.

#### 12. Membatalkan Perubahan
```bash
git reset --hard <commit-id>
```
- **Penjelasan**: Perintah ini membatalkan semua perubahan dan mengembalikan proyekmu ke kondisi tertentu berdasarkan commit ID. Ini seperti membongkar kotak penyimpanan dan mengembalikan semua barang ke tempat semula sesuai catatan tertentu.

#### 13. Melihat Perbedaan
```bash
git diff
```
- **Penjelasan**: Perintah ini menunjukkan perbedaan antara file yang telah diubah tapi belum di-commit. Ini seperti membandingkan dua versi barang dalam kotak penyimpanan sebelum memutuskan mana yang akan disimpan.

### Referensi
- Dokumentasi Git: [Git Documentation](https://git-scm.com/doc)
- Buku "Pro Git" oleh Scott Chacon dan Ben Straub: [Pro Git Book](https://git-scm.com/book/en/v2)


## Konfigurasi Warna Git

Git memiliki kemampuan untuk menampilkan output dengan warna untuk memudahkan pengguna dalam membaca informasi. Berikut adalah cara mengaktifkan dan mengonfigurasi warna di Git.

### Mengaktifkan Warna di Git

Untuk mengaktifkan warna pada semua output Git, kamu dapat menggunakan perintah berikut:

```bash
git config --global color.ui auto
```

Ini akan mengaktifkan warna pada semua output Git seperti `status`, `diff`, dan `branch`.

### Mengonfigurasi Warna untuk Perintah Tertentu

Git memungkinkan pengguna untuk menyesuaikan warna untuk perintah tertentu. Berikut adalah beberapa konfigurasi warna yang umum:

#### Warna untuk Git Status

Untuk mengonfigurasi warna output `git status`, gunakan perintah berikut:

```bash
git config --global color.status.added "green"
git config --global color.status.changed "yellow"
git config --global color.status.untracked "red"
```

#### Warna untuk Git Diff

Untuk mengonfigurasi warna output `git diff`, gunakan perintah berikut:

```bash
git config --global color.diff.meta "yellow bold"
git config --global color.diff.frag "magenta bold"
git config --global color.diff.old "red bold"
git config --global color.diff.new "green bold"
```

#### Warna untuk Git Branch

Untuk mengonfigurasi warna output `git branch`, gunakan perintah berikut:

```bash
git config --global color.branch.current "yellow reverse"
git config --global color.branch.local "green"
git config --global color.branch.remote "cyan"
```

### Mengatur Warna untuk Seluruh Output Git

Jika ingin mengatur warna untuk semua output Git sekaligus, kamu dapat mengedit file konfigurasi `.gitconfig` yang biasanya berada di direktori home (`~/.gitconfig`) dan menambahkan konfigurasi warna di sana. Berikut adalah contoh pengaturan yang dapat kamu tambahkan:

```ini
[color]
    ui = auto

[color "branch"]
    current = yellow reverse
    local = green
    remote = cyan

[color "diff"]
    meta = yellow bold
    frag = magenta bold
    old = red bold
    new = green bold

[color "status"]
    added = green
    changed = yellow
    untracked = red
```

### Cara Mengedit File `.gitconfig`

1. Buka terminal atau command prompt.
2. Ketik `nano ~/.gitconfig` untuk membuka file konfigurasi dengan editor teks `nano` (kamu bisa menggunakan editor lain seperti `vim` atau `notepad` di Windows).
3. Tambahkan atau edit konfigurasi warna seperti contoh di atas.
4. Simpan dan keluar dari editor teks (`Ctrl + O` untuk menyimpan, lalu `Ctrl + X` untuk keluar di `nano`).

### Referensi Warna

Git menggunakan kombinasi warna dan atribut untuk mengonfigurasi output. Berikut adalah beberapa nilai yang dapat digunakan:

- **Warna**: black, red, green, yellow, blue, magenta, cyan, white
- **Atribut**: bold, dim, ul (underline), blink, reverse, italic

### Contoh Penggunaan

Jika kamu ingin menggunakan warna biru dengan teks tebal untuk perubahan yang ditambahkan pada `git status`, gunakan perintah:

```bash
git config --global color.status.added "blue bold"
```

Dengan konfigurasi warna yang sesuai, kamu dapat membuat output Git lebih mudah dibaca dan membantu dalam mengidentifikasi informasi penting dengan cepat.

## REPOSITORY
### Apa Itu Repository?

Repository, atau biasa disebut "repo," adalah tempat penyimpanan untuk proyek perangkat lunak. Dalam konteks Git, repository adalah struktur penyimpanan yang menyimpan semua file, sejarah perubahan, dan informasi lainnya yang dibutuhkan untuk mengelola dan melacak proyek perangkat lunak.

### Jenis Repository

1. **Repository Lokal**: Ini adalah repository yang ada di komputer lokal pengembang. Semua perubahan dan versi disimpan di mesin lokal.
2. **Repository Remote**: Ini adalah repository yang disimpan di server atau layanan hosting (seperti GitHub, GitLab, atau Bitbucket) dan dapat diakses oleh beberapa pengembang untuk kolaborasi.

### Struktur Repository

Sebuah repository Git biasanya terdiri dari beberapa komponen utama:
- **.git**: Direktori tersembunyi yang menyimpan semua data tentang sejarah proyek, termasuk komit, cabang, tag, dan konfigurasi.
- **Working Directory**: Tempat di mana kamu bekerja dengan file proyek. Semua perubahan dilakukan di sini sebelum di-commit ke repository.
- **Staging Area**: Tempat sementara untuk menampung perubahan sebelum di-commit. Ini memungkinkan kamu untuk mempersiapkan snapshot tertentu dari proyek sebelum menyimpannya ke dalam sejarah.

### Perintah Dasar untuk Mengelola Repository

#### Inisialisasi Repository Baru
```bash
git init
```
Perintah ini digunakan untuk membuat repository Git baru di direktori yang ada.

#### Mengkloning Repository
```bash
git clone <url-repository>
```
Perintah ini membuat salinan lokal dari repository remote.

#### Menambahkan File ke Repository
```bash
git add <nama-file>
```
Perintah ini menambahkan file ke staging area.

#### Melakukan Commit
```bash
git commit -m "Pesan commit"
```
Perintah ini menyimpan perubahan dari staging area ke repository dengan pesan deskriptif.

#### Menghubungkan ke Repository Remote
```bash
git remote add origin <url-repo>
```
Perintah ini menghubungkan repository lokal ke repository remote.

#### Mengirim Perubahan ke Repository Remote
```bash
git push origin <nama-cabang>
```
Perintah ini mengirim perubahan dari cabang lokal ke cabang di repository remote.

#### Mengambil Perubahan dari Repository Remote
```bash
git pull origin <nama-cabang>
```
Perintah ini mengambil dan menggabungkan perubahan dari cabang remote ke cabang lokal.

### Mengelola Cabang

Cabang (branch) adalah jalur pengembangan terpisah yang memungkinkan kamu untuk bekerja pada fitur atau perbaikan tanpa mengganggu jalur utama proyek.

#### Membuat Cabang Baru
```bash
git branch <nama-cabang>
```
Perintah ini membuat cabang baru.

#### Berpindah ke Cabang Lain
```bash
git checkout <nama-cabang>
```
Perintah ini memindahkanmu ke cabang yang lain.

#### Menggabungkan Cabang
```bash
git merge <nama-cabang>
```
Perintah ini menggabungkan perubahan dari satu cabang ke cabang lain.

### Keuntungan Menggunakan Repository

1. **Versi Kontrol**: Melacak semua perubahan yang terjadi pada proyek, memungkinkan untuk kembali ke versi sebelumnya jika terjadi kesalahan.
2. **Kolaborasi**: Memungkinkan banyak pengembang untuk bekerja pada proyek yang sama secara bersamaan tanpa saling mengganggu.
3. **Backup**: Repository remote bertindak sebagai cadangan proyek, mengamankan pekerjaan dari kehilangan data lokal.
4. **Manajemen Cabang**: Mendukung pengembangan paralel dengan menggunakan cabang, memungkinkan tim untuk bekerja pada fitur yang berbeda tanpa konflik.

### Kesimpulan

Repository adalah alat penting dalam pengembangan perangkat lunak modern yang memungkinkan manajemen versi, kolaborasi, dan pengelolaan proyek yang efektif. Dengan memahami dasar-dasar repository dan perintah Git yang terkait, pengembang dapat bekerja lebih efisien dan terorganisir.

### Referensi
- Dokumentasi Git: [Git Documentation](https://git-scm.com/doc)
- Buku "Pro Git" oleh Scott Chacon dan Ben Straub: [Pro Git Book](https://git-scm.com/book/en/v2)

---
