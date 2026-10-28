# Tugas Rumah E-Learning: Pertemuan 12 (Backtracking dan CSP)

**Batas kumpul:** [isi tanggal]
**Format:** PDF laporan + file `.ipynb` (P12)
**Pengerjaan:** individu

Materi: [Session12.html](Session12.html) · [P12_Backtracking_CSP.ipynb](P12_Backtracking_CSP.ipynb)

---

## 1. Ringkasan konsep

- **Backtracking** = DFS pada state-space tree dengan pruning: cabang yang sudah melanggar constraint dibuang sebelum dijelajahi.
- **CSP** = (X, D, C): variabel, domain, dan constraint. Contoh: N-Queens, Sudoku, pewarnaan peta, penjadwalan kuliah.
- **Forward checking:** setelah X = v, hapus nilai konflik dari domain tetangga. Jika ada domain kosong, langsung mundur.
- **AC-3:** propagasi konsistensi arc ke seluruh jaringan. Lebih kuat memangkas domain, tetapi lebih mahal per langkah.
- **MRV** memilih variabel dengan domain terkecil. **LCV** memilih nilai yang paling sedikit membatasi tetangga.

---

## 2. Soal teori: pilihan ganda

Pilih satu jawaban untuk setiap soal.

**1.** Apa yang dilakukan forward checking setelah sebuah variabel diberi nilai?

- a) Menghapus nilai konflik dari domain variabel tetangga
- b) Mengurutkan ulang seluruh variabel
- c) Mengulang pencarian dari akar
- d) Menghitung ulang rekurens

**2.** Heuristik MRV memilih variabel dengan kriteria apa?

- a) Domain terbesar
- b) Domain tersisa terkecil
- c) Indeks terkecil
- d) Jumlah tetangga terkecil

**3.** Berapa jumlah solusi N-Queens untuk n = 6?

- a) 2
- b) 4
- c) 10
- d) 92

**4.** Dibanding forward checking, AC-3 umumnya:

- a) Memangkas lebih sedikit, dan lebih murah per langkah
- b) Memangkas lebih banyak, tetapi lebih mahal per langkah
- c) Tidak pernah memangkas domain
- d) Hanya bekerja pada N-Queens

---

## 3. Soal uraian

1. Gambarkan state-space tree untuk 4-Queens dengan urutan kolom 0 → 3 sampai solusi pertama ditemukan. Tandai cabang yang dipangkas dan sebutkan alasannya.
2. Modelkan Sudoku 4×4 sebagai CSP: tentukan X, D, dan C. Berapa jumlah variabel, ukuran domain, dan constraint alldiff?
3. Pada pewarnaan peta Australia dengan 3 warna, jelaskan bagaimana forward checking dan MRV bekerja bersama dalam mengurangi jumlah backtrack.

---

## 4. Tugas koding (Colab, notebook P12)

1. **LCV.** Lengkapi fungsi `lcv_order(v, doms, nbrs, ok)` yang masih berisi `pass  # TODO`. Fungsi mengembalikan nilai-nilai domain `v` diurutkan dari yang paling sedikit membatasi tetangga. Integrasikan ke `solve_csp`, lalu bandingkan jumlah node dengan dan tanpa LCV pada N-Queens n = 8.
2. **Hitung semua solusi.** Modifikasi solver agar mencari semua solusi N-Queens untuk n = 4 sampai 8. Hasil yang diharapkan: 2, 10, 4, 40, 92.
3. **Penjadwalan.** Modelkan penjadwalan kuliah minimal 5 mata kuliah, 3 dosen, dan 4 slot waktu sebagai CSP. Tulis X, D, dan C secara eksplisit, jalankan solver FC+MRV, lalu tampilkan jadwalnya. Jika tidak ada solusi, jelaskan constraint mana yang menyebabkannya.
4. **Perbandingan.** Untuk Sudoku minimal 3 puzzle (satu mudah, satu sedang, satu sulit), tabulasikan jumlah node untuk backtracking murni dan FC+MRV.

> Jika solver melebihi batas node, naikkan `limit` atau catat hasilnya sebagai "LIMIT". Jangan menghapus batas tanpa menuliskannya di laporan.

---

## 5. Penilaian

| Aspek | Bobot | Kriteria |
|---|---|---|
| Ketepatan teori | 40% | Jawaban benar, langkah perhitungan jelas, definisi CSP dan constraint tepat. |
| Kode | 35% | Berjalan tanpa error, hasil diverifikasi (jumlah solusi cocok dengan baseline), kode rapi. |
| Analisis dan laporan | 25% | Tabel node diberi label, perbandingan FC+MRV dan backtracking dijelaskan, batas (limit) dilaporkan. |

Tugas ini termasuk komponen Kuis/Tugas mingguan (20%).

**Cara kumpul:** kumpulkan satu file PDF laporan dan file `.ipynb` P12 yang sudah dijalankan ulang dari awal (Runtime → Restart and run all). Beri nama `NIM_Nama_P12.ipynb`.
