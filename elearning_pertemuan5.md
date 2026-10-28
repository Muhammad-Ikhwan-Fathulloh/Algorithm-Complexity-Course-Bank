# Tugas Rumah E-Learning: Pertemuan 5 (Divide and Conquer II)

**Batas kumpul:** [isi tanggal]
**Format:** PDF laporan + file `.ipynb` (P05)
**Pengerjaan:** individu

Materi: [Session5.html](Session5.html) · [P05_DivideConquer2.ipynb](P05_DivideConquer2.ipynb)

---

## 1. Ringkasan konsep

- **Karatsuba:** 3 perkalian rekursif, bukan 4. T(n) = 3T(n/2) + n → Θ(n^log₂3) ≈ Θ(n^1.585).
- **Strassen:** 7 perkalian blok 2×2, bukan 8. T(n) = 7T(n/2) + n² → Θ(n^2.807).
- **Titik impas (crossover):** Strassen baru menang jika matriksnya cukup besar, karena konstanta dan penjumlahan tambahannya besar.
- **Closest Pair:** strip selebar 2δ hanya perlu dicek dengan ≤ 7 tetangga per titik → Θ(n log n) jika strip terurut menurut y.
- **[Modern]** AlphaTensor (2022) menemukan dekomposisi 4×4 dengan 47 perkalian pada aritmetika modulo 2. AlphaDev (2023) menemukan rutin sorting yang masuk ke LLVM libc++.

---

## 2. Soal teori: pilihan ganda

Pilih satu jawaban untuk setiap soal.

**1.** Karatsuba membutuhkan T(n) = 3T(n/2) + n. Berapa eksponen kompleksitasnya?

- a) Θ(n)
- b) Θ(n^1.585)
- c) Θ(n²)
- d) Θ(n³)

**2.** Pada langkah combine Closest Pair, berapa tetangga paling banyak yang perlu diperiksa untuk tiap titik di strip?

- a) 3
- b) 7
- c) n
- d) log n

**3.** Berapa perkalian submatriks yang dipakai Strassen untuk blok 2×2?

- a) 6
- b) 8
- c) 7
- d) 49

---

## 3. Soal uraian

1. Jelaskan mengapa strip pada Closest Pair hanya perlu dicek dengan 7 titik berikutnya. Gambarkan persegi panjang δ × 2δ di sekitar garis tengah dan tunjukkan mengapa paling banyak 8 titik dapat berada di dalamnya.
2. Gunakan Master Theorem untuk menunjukkan bahwa Strassen (T(n) = 7T(n/2) + n²) lebih cepat daripada perkalian matriks naif (T(n) = 8T(n/2) + n²).
3. Hitung log₄47 dan bandingkan eksponen AlphaTensor dengan Strassen. Untuk n = 4096, berapa persen operasi yang dihemat secara kasar? Tunjukkan langkah perhitunganmu.

---

## 4. Tugas koding (Colab, notebook P05)

1. **Padding.** Lengkapi fungsi `strassen_padded(A, B)` yang masih berisi `pass  # TODO`. Fungsi harus menerima matriks berukuran bebas (bukan pangkat dua), memperluas ke ukuran pangkat dua terdekat dengan nol, lalu memotong hasilnya. Verifikasi terhadap `A @ B` untuk minimal 3 ukuran berbeda, termasuk ukuran ganjil.
2. **Cutoff optimal.** Cari nilai `n0` yang paling cepat untuk ukuran 512 (atau 256 jika mesin lambat). Buat grafik waktu vs `n0` dan tentukan nilainya.
3. **Kemiringan log-log.** Ukur waktu Strassen dan perkalian naif dengan kode Python murni (tanpa BLAS) untuk beberapa ukuran. Hitung kemiringan kurva dan bandingkan dengan teori (≈ 2.807 vs 3). Jika waktu terlalu lama, ukuran kecil saja sudah cukup.
4. **Benchmark Karatsuba.** Implementasikan Karatsuba untuk bilangan 200, 500, dan 1000 digit. Bandingkan dengan perkalian sekolah dan dengan operator `*` bawaan Python. Jelaskan hasilnya.

---

## 5. Laporan singkat (1–2 halaman)

Bandingkan titik impas teoritis (dari jumlah operasi) dengan titik impas empiris (dari waktu), lalu jelaskan mengapa keduanya berbeda.

---

## 6. Penilaian

| Aspek | Bobot | Kriteria |
|---|---|---|
| Ketepatan teori | 40% | Jawaban benar, langkah perhitungan jelas, Master Theorem diterapkan dengan benar. |
| Kode | 35% | Berjalan tanpa error, hasil diverifikasi (assert atau perbandingan dengan baseline), kode rapi. |
| Analisis dan laporan | 25% | Grafik atau tabel diberi label, perbedaan teori vs empiris dijelaskan, kesimpulan tidak melebihi data. |

Tugas ini termasuk komponen Kuis/Tugas mingguan (20%).

**Cara kumpul:** kumpulkan satu file PDF laporan dan file `.ipynb` P05 yang sudah dijalankan ulang dari awal (Runtime → Restart and run all). Beri nama `NIM_Nama_P05.ipynb`.
