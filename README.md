# Sprint Planning: Aplikasi Peminjaman Buku Perpustakaan Kampus

> Tugas Praktik Minggu Ini: Simulasi Sprint & Tugas Kelompok
> Tools papan kerja: **GitHub Projects**
> Papan proyek: tab **Projects** pada repository ini

## 1. Informasi Kelompok

| Peran | Nama | NIM |
|---|---|---|
| Product Owner | Dedek Irwansyah | 24210002 |
| Scrum Master | Rio Refaldo | 24210004 |
| Development Team | Farhan | 24210010 |
| Development Team | Amsalul Hadi | 24210041 |

## 2. Gambaran Proyek

Aplikasi web untuk membantu mahasiswa mencari, meminjam, dan memperpanjang peminjaman buku perpustakaan kampus secara online, serta membantu petugas mengelola data peminjaman.

**Durasi sprint:** 1 minggu (5 hari kerja)
**Kapasitas tim (velocity):** ± 20 story points

## 3. Product Backlog (User Story)

Format: *Sebagai [peran], saya ingin [fitur], agar [manfaat].*

| ID | User Story | Kriteria Penerimaan | Prioritas | Estimasi (SP) |
|---|---|---|---|---|
| US-01 | Sebagai mahasiswa, saya ingin login dengan akun kampus, agar data peminjaman saya aman. | Login berhasil dengan NIM dan password valid; pesan error muncul bila salah. | Tinggi | 3 |
| US-02 | Sebagai mahasiswa, saya ingin mencari buku berdasarkan judul atau pengarang, agar cepat menemukan buku. | Hasil pencarian tampil kurang dari 3 detik; menampilkan status ketersediaan. | Tinggi | 5 |
| US-03 | Sebagai mahasiswa, saya ingin melihat detail buku, agar tahu isi dan ketersediaannya. | Halaman detail menampilkan judul, pengarang, tahun, stok. | Tinggi | 2 |
| US-04 | Sebagai mahasiswa, saya ingin meminjam buku secara online, agar tidak antre di perpustakaan. | Stok berkurang 1 setelah pinjam; bukti peminjaman muncul. | Tinggi | 5 |
| US-05 | Sebagai mahasiswa, saya ingin melihat riwayat peminjaman, agar bisa memantau buku yang saya pinjam. | Daftar pinjaman aktif dan selesai tampil lengkap dengan tanggal jatuh tempo. | Sedang | 3 |
| US-06 | Sebagai mahasiswa, saya ingin memperpanjang peminjaman, agar tidak terkena denda. | Perpanjangan maksimal 1 kali, +7 hari. | Sedang | 5 |
| US-07 | Sebagai petugas, saya ingin menambah dan mengubah data buku, agar katalog selalu terbaru. | Petugas dapat menambah, mengubah, dan menghapus buku. | Sedang | 8 |
| US-08 | Sebagai mahasiswa, saya ingin menerima notifikasi jatuh tempo, agar tidak lupa mengembalikan buku. | Notifikasi dikirim H-2 sebelum jatuh tempo. | Rendah | 5 |

**Total backlog:** 36 SP

## 4. Estimasi dengan Planning Poker

Kartu yang dipakai: deret Fibonacci (1, 2, 3, 5, 8, 13).
Tanggal pelaksanaan: 22 / 11 / 2026

| ID | Putaran 1 (Dedek / Rio / Farhan / Amsalul) | Diskusi | Hasil Akhir |
|---|---|---|---|
| US-01 | 3 / 3 / 5 / 3 | Farhan menilai validasi login mungkin membutuhkan sedikit pekerjaan tambahan. Setelah membahas ruang lingkup login NIM dan password, tim sepakat pada estimasi awal. | 3 SP |
| US-02 | 5 / 8 / 5 / 5 | Rio mempertimbangkan proses pencarian dan status ketersediaan. Tim menyepakati estimasi 5 karena ruang lingkup pencarian dibatasi pada judul atau pengarang. | 5 SP |
| US-03 | 2 / 2 / 3 / 2 | Farhan menilai ada pekerjaan tambahan untuk menyusun tampilan, tetapi informasi yang ditampilkan sederhana. Tim sepakat pada 2. | 2 SP |
| US-04 | 5 / 8 / 5 / 8 | Rio dan Amsalul mempertimbangkan validasi stok serta pembuatan bukti peminjaman. Setelah diskusi ruang lingkup, tim sepakat pada 5. | 5 SP |
| US-05 | 3 / 3 / 5 / 3 | Farhan mempertimbangkan pengelompokan pinjaman aktif dan selesai. Tim menyepakati 3 karena hanya menampilkan data riwayat. | 3 SP |
| US-06 | 5 / 8 / 5 / 8 | Rio dan Amsalul mempertimbangkan aturan maksimal satu kali perpanjangan dan tambahan tujuh hari. Tim sepakat pada 5. | 5 SP |
| US-07 | 8 / 8 / 8 / 5 | Amsalul menilai fitur CRUD lebih sederhana, sedangkan anggota lain mempertimbangkan seluruh proses tambah, ubah, dan hapus. Tim sepakat pada 8. | 8 SP |
| US-08 | 5 / 8 / 5 / 8 | Rio dan Amsalul mempertimbangkan mekanisme pengiriman notifikasi H-2. Tim sepakat pada 5. | 5 SP |


## 5. Sprint Planning

### Sprint Goal

> **"Mahasiswa dapat login, mencari buku, melihat detail, dan meminjam buku secara online."**

### Sprint Backlog (Sprint 1)

| ID | Item | SP | PIC | Status |
|---|---|---|---|---|
| US-01 | Login mahasiswa | 3 | Dedek | To Do |
| US-02 | Pencarian buku | 5 | Rio | To Do |
| US-03 | Detail buku | 2 | Farhan | To Do |
| US-04 | Peminjaman buku online | 5 | Amsalul | To Do |
| US-05 | Riwayat peminjaman | 3 | Dedek | To Do |

**Total sprint:** 18 SP (di bawah kapasitas 20 SP, menyisakan ruang untuk risiko).

Item yang **tidak** masuk Sprint 1: US-06, US-07, US-08 (dikerjakan di sprint berikutnya).

### Struktur Papan GitHub Projects

Kolom status: `Backlog` → `Sprint Backlog` → `In Progress` → `Review/Testing` → `Done`

Setiap user story dibuat sebagai **Issue** (US-01 sampai US-08) dan ditambahkan ke papan Project, dengan label prioritas dan field *Story Points*.

## 6. Definition of Done (DoD)

Sebuah item dianggap **selesai** jika:

- [ ] Kode selesai dan sudah di-*merge* ke branch `main` melalui pull request
- [ ] Kode sudah direview minimal oleh 1 anggota lain
- [ ] Semua kriteria penerimaan terpenuhi
- [ ] Lolos pengujian manual (dan unit test bila ada)
- [ ] Tidak ada bug kritis yang tersisa
- [ ] Dokumentasi singkat (README/komentar) diperbarui
- [ ] Sudah didemokan dan diterima oleh Product Owner

## 7. Simulasi Sprint

### 7.1 Daily Scrum (5 menit)

Tiga pertanyaan: *Apa yang dikerjakan kemarin? Apa rencana hari ini? Apa hambatannya?*

| Hari / Tanggal | Dedek | Rio | Farhan | Amsalul | Hambatan |
|---|---|---|---|---|---|
| Hari 1 | Kemarin: Sprint baru dimulai. Hari ini: Menentukan kebutuhan login dan memeriksa kesesuaian fitur. | Kemarin: Menyiapkan Sprint Backlog dan pembagian tugas. Hari ini: Memastikan Issue tersedia di GitHub Projects. | Kemarin: Belum ada pengerjaan. Hari ini: Membuat rancangan halaman detail buku. | Kemarin: Belum ada pengerjaan. Hari ini: Merancang fitur peminjaman online. | Tim perlu memahami alur GitHub Projects; desain UI dan alur validasi stok belum ditentukan. |
| Hari 2 | Kemarin: Memeriksa kebutuhan login. Hari ini: Memeriksa kriteria penerimaan login dan riwayat. | Kemarin: Memastikan Issue masuk Sprint Backlog. Hari ini: Memantau progres dan memperbarui status Issue. | Kemarin: Membuat rancangan detail buku. Hari ini: Menyelesaikan tampilan judul, pengarang, tahun, dan stok. | Kemarin: Merancang fitur peminjaman. Hari ini: Membuat alur peminjaman dan pengecekan stok. | Desain database belum final; data buku masih contoh; validasi stok perlu diperiksa. |
| Hari 3 | Kemarin: Memeriksa kebutuhan login dan riwayat. Hari ini: Memeriksa hasil fitur dan memberi feedback. | Kemarin: Memantau progres Issue. Hari ini: Mengkoordinasikan pengujian dan menyiapkan Sprint Review. | Kemarin: Menyelesaikan tampilan detail buku. Hari ini: Menguji dan memperbaiki tampilan. | Kemarin: Membuat alur peminjaman dan pengecekan stok. Hari ini: Menguji proses peminjaman dan pengurangan stok. | Ada tampilan yang perlu disesuaikan; waktu pengujian terbatas dan masih membutuhkan data buku untuk pengujian. |

### 7.2 Sprint Review (mini)

**Pembukaan Scrum Master (Rio):**

> "Pada Sprint 1 ini, tujuan kami adalah membuat fitur dasar aplikasi peminjaman buku perpustakaan kampus. Kami akan menunjukkan fitur yang sudah dikerjakan, kemudian meminta masukan dari Product Owner."

- **Item yang selesai (simulasi):** US-01 Login mahasiswa dan US-03 Detail buku.
- **Item yang belum selesai (simulasi):** US-02 Pencarian buku, US-04 Peminjaman buku online (masih Review/Testing), dan US-05 Riwayat peminjaman.
- **Demo yang ditunjukkan:** Rancangan halaman login berisi input NIM, password, tombol Login, dan pesan kesalahan; halaman detail buku berisi judul, pengarang, tahun terbit, stok, serta tombol pinjam.
- **Masukan Product Owner (Dedek):**

> "Tampilan login dan detail buku sudah cukup baik serta mudah dipahami. Untuk fitur peminjaman, tambahkan konfirmasi sebelum buku berhasil dipinjam. Informasi stok buku juga harus terlihat dengan jelas."

**Kesimpulan Sprint Review:**

> "Beberapa fitur utama telah berhasil dibuat dalam bentuk rancangan dan simulasi. Fitur pencarian buku dan penyempurnaan proses peminjaman masih perlu dilanjutkan."

> **Catatan:** Status selesai di atas hanya asumsi simulasi. Dalam pelaksanaan nyata, item hanya boleh dipindahkan ke Done jika seluruh kriteria Definition of Done terpenuhi dan diterima Product Owner.

### 7.3 Sprint Retrospective (singkat)

| Anggota | Berjalan baik | Perlu diperbaiki | Aksi berikutnya |
|---|---|---|---|
| Dedek | Komunikasi dengan anggota cukup baik. | Kriteria fitur perlu dijelaskan lebih detail sejak awal. | Membahas Acceptance Criteria sebelum pengerjaan. |
| Rio | Pembagian tugas berjalan cukup teratur. | Pemantauan progres perlu lebih konsisten. | Memastikan GitHub Projects diperbarui setiap hari. |
| Farhan | Dapat menyelesaikan rancangan detail buku. | Perlu lebih aktif menyampaikan kendala. | Memberikan update progres dan kendala saat Daily Scrum. |
| Amsalul | Dapat memahami alur peminjaman. | Pengujian fitur perlu dilakukan lebih awal. | Menyiapkan data uji dan menguji alur peminjaman sejak awal. |

**Kesimpulan Retrospective:**

> "Komunikasi dan pembagian tugas sudah berjalan cukup baik. Namun, tim perlu meningkatkan pengujian, memperjelas kebutuhan fitur sebelum pengerjaan, serta memperbarui progres pada GitHub Projects secara rutin. Perbaikan ini akan diterapkan pada Sprint berikutnya."

### 7.4 Simulasi Pergerakan Issue di GitHub Projects

| Issue | Hari 1 | Hari 2 | Hari 3 |
|---|---|---|---|
| US-01 Login | In Progress | Review/Testing | Done* |
| US-02 Pencarian Buku | Sprint Backlog | In Progress | In Progress |
| US-03 Detail Buku | In Progress | Review/Testing | Done* |
| US-04 Peminjaman Buku | In Progress | In Progress | Review/Testing |
| US-05 Riwayat Peminjaman | Sprint Backlog | Sprint Backlog | Sprint Backlog |

\*Status Done hanya contoh simulasi dan mengasumsikan seluruh Definition of Done telah terpenuhi. Jika belum, pertahankan status Review/Testing.

### 7.5 Pembagian Peran Saat Presentasi

| Anggota | Tugas saat simulasi |
|---|---|
| Dedek Irwansyah (Product Owner) | Membacakan atau menjelaskan kebutuhan User Story dan memberikan feedback saat Sprint Review. |
| Rio Refaldo (Scrum Master) | Memimpin Planning Poker dan Daily Scrum, mengatur waktu, serta memperbarui GitHub Projects. |
| Farhan (Developer) | Menjelaskan dan mendemonstrasikan rancangan halaman Detail Buku (US-03). |
| Amsalul Hadi (Developer) | Menjelaskan rancangan alur peminjaman buku online (US-04). |

### 7.6 Contoh Naskah Farhan (Developer – US-03)

**Planning Poker:**

> "Saya memberikan estimasi 2 Story Points untuk fitur detail buku karena fitur ini menampilkan informasi seperti judul, pengarang, tahun terbit, dan stok. Tingkat kesulitannya relatif sederhana."

**Daily Scrum Hari 1:**

> "Kemarin belum ada pengerjaan karena sprint baru dimulai. Hari ini saya akan mulai membuat rancangan halaman detail buku. Hambatan saya adalah belum menentukan desain tampilan yang sesuai."

**Daily Scrum Hari 2:**

> "Kemarin saya sudah membuat rancangan halaman detail buku. Hari ini saya akan menyelesaikan tampilan informasi buku, seperti judul, pengarang, tahun terbit, dan stok. Hambatan saya adalah data buku masih menggunakan data contoh."

**Daily Scrum Hari 3:**

> "Kemarin saya menyelesaikan tampilan detail buku. Hari ini saya akan melakukan pengecekan dan pengujian tampilan. Hambatan besar tidak ada, hanya perlu memastikan informasi buku ditampilkan dengan benar."

**Sprint Review:**

> "Pada Sprint ini, saya mengerjakan fitur detail buku. Halaman ini menampilkan judul buku, pengarang, tahun terbit, dan stok buku, sehingga mahasiswa bisa melihat informasi buku sebelum melakukan peminjaman."

**Retrospective:**

> "Hal yang berjalan baik adalah saya dapat memahami tugas dan menyelesaikan rancangan detail buku. Hal yang perlu diperbaiki adalah saya harus lebih aktif menyampaikan progres dan kendala agar pekerjaan tim lebih terkoordinasi."

### 7.7 Catatan Pelaksanaan

Seluruh hasil voting, jawaban Daily Scrum, demo, dan evaluasi dalam dokumen ini merupakan **contoh simulasi untuk latihan**. Saat praktik kelompok, sesuaikan dengan hasil diskusi dan pekerjaan yang benar-benar dilakukan. Jangan menyatakan kode, pengujian, atau fitur telah selesai jika belum memenuhi Definition of Done.
