# 📘 Kompleksitas Algoritma (Analysis & Design of Algorithms)

Materi kuliah **14 pertemuan** (murni materi, di luar UTS & UAS) yang disusun dari kurikulum **Institut Teknologi Bandung (IF2211 – Strategi Algoritma, Rinaldi Munir)**, kurikulum kampus luar negeri (**MIT 6.006/6.046J**, **Stanford CS161**, **Princeton Algorithms – Sedgewick & Wayne**, buku **CLRS**), serta praktik industri (Google Tech Dev Guide, NeetCode).

---

## 🎯 Deskripsi Mata Kuliah

Mata kuliah ini membahas cara menganalisis efisiensi algoritma (waktu & ruang), notasi asimtotik, teknik desain algoritma (*brute force, divide and conquer, greedy, dynamic programming, backtracking, branch and bound*), serta pengantar teori kompleksitas komputasi (P vs NP). Mahasiswa juga dikenalkan pada praktik penerapan analisis kompleksitas di dunia industri (interview teknis, optimasi sistem skala besar).

## 🧭 Capaian Pembelajaran (Learning Outcomes)

1. Mampu menganalisis kompleksitas waktu & ruang suatu algoritma menggunakan notasi asimtotik.
2. Mampu memilih dan merancang strategi algoritma yang tepat untuk suatu persoalan.
3. Mampu menyelesaikan persamaan rekurens (Master Theorem, recursion tree, substitution).
4. Memahami batas kemampuan komputasi (P, NP, NP-Complete, NP-Hard).
5. Mampu menerapkan analisis kompleksitas dalam konteks nyata/industri (technical interview, optimasi sistem).

## 📚 Sumber Referensi Utama

| Sumber | Institusi/Penulis | Link |
|---|---|---|
| IF2211 Strategi Algoritma | Rinaldi Munir, STEI ITB | [informatika.stei.itb.ac.id/~rinaldi.munir](https://informatika.stei.itb.ac.id/~rinaldi.munir/) |
| 6.006 Introduction to Algorithms | MIT OpenCourseWare | [ocw.mit.edu/6.006](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/) |
| 6.046J Design and Analysis of Algorithms | MIT OpenCourseWare | [ocw.mit.edu/6.046j](https://ocw.mit.edu/courses/6-046j-design-and-analysis-of-algorithms-spring-2015/) |
| CS161 Design and Analysis of Algorithms | Stanford University | [cs161-stanford.github.io](https://cs161-stanford.github.io/) |
| Algorithms, Part I & II (Coursera) | Sedgewick & Wayne, Princeton University | [Part I](https://www.coursera.org/learn/algorithms-part1) · [Part II](https://www.coursera.org/learn/algorithms-part2) |
| *Introduction to Algorithms* (CLRS) | Cormen, Leiserson, Rivest, Stein | [mitpress.mit.edu](https://mitpress.mit.edu/9780262046305/introduction-to-algorithms/) |
| *Algorithm Design* | Jon Kleinberg & Éva Tardos | dipakai sebagai textbook Stanford CS161 |
| Tech Dev Guide – Data Structures & Algorithms | Google | [techdevguide.withgoogle.com](https://techdevguide.withgoogle.com/paths/data-structures-and-algorithms/) |
| NeetCode (praktisi) | Praktisi industri | [neetcode.io](https://neetcode.io/) |
| Video Kuliah Strategi Algoritma ITB | Rinaldi Munir / STEI ITB | [Playlist YouTube](https://www.youtube.com/playlist?list=PLyYkJZR4un3pdFjgNZU9sO3Lg0uezCTeW) |

---

## 🗓️ Rencana 14 Pertemuan (Materi)

> Catatan: UTS dan UAS **tidak** menempati slot pertemuan — keduanya adalah agenda evaluasi terpisah (lihat bagian **Evaluasi** di bawah).

### Pertemuan 1 — Pendahuluan & Notasi Asimtotik
- **Topik:** Apa itu kompleksitas algoritma, model komputasi RAM, notasi Big-O, Big-Omega, Big-Theta, Little-o.
- **Sumber:** [ITB – Pengantar Strategi Algoritma](https://informatika.stei.itb.ac.id/~rinaldi.munir/Stmik/), [MIT 6.006](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/), CLRS Bab 3.
- **Praktik:** Menghitung kompleksitas dari potongan kode sederhana (loop, nested loop).
- **Tugas:** Latihan soal notasi asimtotik.

### Pertemuan 2 — Rekursi & Persamaan Rekurens
- **Topik:** Rekursi, recursion tree, metode substitusi, Master Theorem.
- **Sumber:** [MIT 6.006 – Recurrences](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/), [Stanford CS161](https://cs161-stanford.github.io/), CLRS Bab 4.
- **Praktik:** Menyelesaikan rekurens T(n) = 2T(n/2) + n, dsb.
- **Tugas:** Studi kasus rekurens Merge Sort & Binary Search.

### Pertemuan 3 — Brute Force & Exhaustive Search
- **Topik:** Strategi brute force, exhaustive search, kompleksitas eksponensial/faktorial (contoh: TSP).
- **Sumber:** [ITB – Algoritma Brute Force](https://informatika.stei.itb.ac.id/~rinaldi.munir/Stmik/), CLRS.
- **Praktik:** Selection sort, sequential search, string matching brute force.
- **Tugas:** Analisis kompleksitas algoritma brute force TSP.

### Pertemuan 4 — Divide and Conquer I
- **Topik:** Konsep *divide, conquer, combine*; Merge Sort, Quick Sort, Binary Search.
- **Sumber:** [ITB – Divide and Conquer](https://informatika.stei.itb.ac.id/~rinaldi.munir/Stmik/), [MIT 6.006](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/), [Stanford CS161](https://cs161-stanford.github.io/).
- **Praktik:** Implementasi & analisis kompleksitas Merge Sort vs Quick Sort (best/average/worst case).
- **Tugas:** Studi perbandingan performa D&C sorting.

### Pertemuan 5 — Divide and Conquer II
- **Topik:** Closest Pair of Points, perkalian matriks Strassen, pengantar Fast Fourier Transform.
- **Sumber:** [MIT 6.046J](https://ocw.mit.edu/courses/6-046j-design-and-analysis-of-algorithms-spring-2015/), Kleinberg & Tardos Bab 5, [Stanford CS161](https://cs161-stanford.github.io/).
- **Praktik:** Studi kasus Closest Pair.
- **Tugas:** Mini proyek: implementasi Strassen's Matrix Multiplication.

### Pertemuan 6 — Decrease and Conquer & Struktur Data untuk Efisiensi
- **Topik:** Decrease by constant/factor/variable, Insertion Sort, DFS/BFS, Topological Sort; kompleksitas Heap, Hash Table, Balanced BST (AVL/Red-Black).
- **Sumber:** [ITB – Decrease and Conquer](https://informatika.stei.itb.ac.id/~rinaldi.munir/Stmik/), [Stanford CS161](https://cs161-stanford.github.io/), CLRS Bab 6, 10–13.
- **Praktik:** Analisis kompleksitas operasi struktur data.
- **Tugas:** Studi kasus pemilihan struktur data untuk mengoptimalkan algoritma.

### Pertemuan 7 — Greedy Algorithms I
- **Topik:** Prinsip greedy, bukti kebenaran (*exchange argument*), Activity Selection, Fractional Knapsack.
- **Sumber:** [ITB – Algoritma Greedy](https://informatika.stei.itb.ac.id/~rinaldi.munir/Stmik/), [MIT 6.046J](https://ocw.mit.edu/courses/6-046j-design-and-analysis-of-algorithms-spring-2015/), Kleinberg & Tardos Bab 4.
- **Praktik:** Implementasi Activity Selection Problem.
- **Tugas:** Studi kasus penjadwalan (job scheduling).

### Pertemuan 8 — Greedy Algorithms II (Graf)
- **Topik:** Algoritma Kruskal, Prim (MST), Dijkstra (shortest path), Huffman Coding.
- **Sumber:** [ITB](https://informatika.stei.itb.ac.id/~rinaldi.munir/Stmik/), [Stanford CS161](https://cs161-stanford.github.io/), CLRS Bab 22–24.
- **Praktik:** Implementasi & analisis kompleksitas MST dan shortest path.
- **Tugas:** Perbandingan kompleksitas Kruskal vs Prim tergantung struktur data.

### Pertemuan 9 — Dynamic Programming I
- **Topik:** Prinsip *overlapping subproblems* & *optimal substructure*, memoization vs tabulation, 0/1 Knapsack, Fibonacci.
- **Sumber:** [ITB – Program Dinamis](https://informatika.stei.itb.ac.id/~rinaldi.munir/Stmik/), [MIT 6.006](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/), [Coursera Algorithms Part II](https://www.coursera.org/learn/algorithms-part2).
- **Praktik:** Implementasi 0/1 Knapsack top-down & bottom-up.
- **Tugas:** Analisis kompleksitas waktu/ruang DP.

### Pertemuan 10 — Dynamic Programming II
- **Topik:** Longest Common Subsequence, Edit Distance, Matrix Chain Multiplication, DP pada graf (Bellman-Ford, Floyd-Warshall).
- **Sumber:** CLRS Bab 14–15, [MIT 6.046J](https://ocw.mit.edu/courses/6-046j-design-and-analysis-of-algorithms-spring-2015/), [Stanford CS161](https://cs161-stanford.github.io/).
- **Praktik:** Studi kasus edit distance (aplikasi: spell checker, diff tool).
- **Tugas:** Mini proyek DP pilihan mahasiswa.

### Pertemuan 11 — Backtracking
- **Topik:** Konsep *state space tree*, pruning, N-Queens, Sudoku Solver, Subset Sum, Hamiltonian Cycle.
- **Sumber:** [ITB – Runut-balik (Backtracking)](https://informatika.stei.itb.ac.id/~rinaldi.munir/Stmik/), Kleinberg & Tardos.
- **Praktik:** Implementasi N-Queens dengan analisis kompleksitas *worst case*.
- **Tugas:** Studi kasus backtracking untuk constraint satisfaction problem.

### Pertemuan 12 — Branch and Bound
- **Topik:** Branch and Bound (TSP, 0/1 Knapsack) dengan *bounding function*, perbandingan dengan backtracking.
- **Sumber:** [ITB – Branch and Bound](https://informatika.stei.itb.ac.id/~rinaldi.munir/Stmik/), CLRS.
- **Praktik:** Studi kasus TSP dengan Branch and Bound.
- **Tugas:** Perbandingan efisiensi Branch and Bound vs Backtracking pada persoalan yang sama.

### Pertemuan 13 — Pengantar Teori Kompleksitas Komputasi
- **Topik:** Kelas kompleksitas **P, NP, NP-Complete, NP-Hard**, reduksi polinomial, Cook-Levin theorem (pengantar).
- **Sumber:** [MIT 6.046J – Complexity Theory](https://ocw.mit.edu/courses/6-046j-design-and-analysis-of-algorithms-spring-2015/), CLRS Bab 34, [Stanford CS161](https://cs161-stanford.github.io/).
- **Praktik:** Latihan pembuktian NP-Completeness sederhana (mis. reduksi 3-SAT ke persoalan lain).
- **Tugas:** Studi kasus klasifikasi persoalan (P atau NP-Complete?).

### Pertemuan 14 — Algoritma Aproksimasi, Randomized, & Studi Kasus Industri
- **Topik:** Algoritma aproksimasi untuk persoalan NP-Hard, algoritma randomized (Randomized Quick Sort), studi kasus penerapan analisis kompleksitas di industri (optimasi query database, sistem rekomendasi, technical interview).
- **Sumber:** [Google Tech Dev Guide](https://techdevguide.withgoogle.com/paths/data-structures-and-algorithms/), [NeetCode](https://neetcode.io/), [Stanford CS161 – Randomized Algorithms](https://cs161-stanford.github.io/), Kleinberg & Tardos Bab 11 & 13.
- **Praktik:** Studi kasus praktisi + sesi tanya jawab/guest talk (opsional).
- **Tugas:** Refleksi akhir: pemetaan seluruh materi 14 pertemuan ke dalam satu peta konsep.

---

## 📝 Evaluasi (Terpisah dari 14 Pertemuan)

| Evaluasi | Waktu Pelaksanaan | Cakupan Materi | Bobot |
|---|---|---|---|
| **Kuis/Tugas mingguan** | Sepanjang semester | Mengikuti materi tiap pertemuan | 20% |
| **Proyek/Mini Project** | Menyusul, di luar jadwal pertemuan | Bebas (menerapkan ≥2 strategi algoritma) | 20% |
| **UTS (Ujian Tengah Semester)** | Minggu tengah semester, setelah Pertemuan 6–7 selesai | Pertemuan 1–6 (Notasi asimtotik s.d. Decrease and Conquer) | 25% |
| **UAS (Ujian Akhir Semester)** | Minggu akhir semester, setelah Pertemuan 14 selesai | Pertemuan 7–14 (Greedy s.d. Teori Kompleksitas & Aproksimasi), dapat bersifat komprehensif | 35% |

## 🛠️ Proyek Akhir (Opsional)

Mahasiswa memilih satu persoalan nyata (mis. optimasi rute, penjadwalan, pencarian teks) lalu:
1. Merancang minimal dua strategi algoritma berbeda (mis. greedy vs DP, atau brute force vs D&C).
2. Menganalisis kompleksitas masing-masing secara teoritis.
3. Melakukan benchmarking empiris dan membandingkan dengan hasil analisis teoritis.

## 🔗 Referensi & Link Lengkap

- Rinaldi Munir, *Diktat & Slide Kuliah IF2211 Strategi Algoritma*, STEI ITB — https://informatika.stei.itb.ac.id/~rinaldi.munir/
- Playlist Video Kuliah Strategi Algoritma ITB — https://www.youtube.com/playlist?list=PLyYkJZR4un3pdFjgNZU9sO3Lg0uezCTeW
- MIT OCW 6.006 *Introduction to Algorithms* — https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/
- MIT OCW 6.046J *Design and Analysis of Algorithms* — https://ocw.mit.edu/courses/6-046j-design-and-analysis-of-algorithms-spring-2015/
- Stanford CS161 *Design and Analysis of Algorithms* — https://cs161-stanford.github.io/
- Coursera *Algorithms, Part I* (Princeton – Sedgewick & Wayne) — https://www.coursera.org/learn/algorithms-part1
- Coursera *Algorithms, Part II* (Princeton – Sedgewick & Wayne) — https://www.coursera.org/learn/algorithms-part2
- Cormen, Leiserson, Rivest, Stein, *Introduction to Algorithms (CLRS)* — https://mitpress.mit.edu/9780262046305/introduction-to-algorithms/
- Kleinberg & Tardos, *Algorithm Design* — digunakan sebagai textbook di Stanford CS161
- Google, *Tech Dev Guide – Data Structures & Algorithms* — https://techdevguide.withgoogle.com/paths/data-structures-and-algorithms/
- NeetCode (praktisi, latihan soal & penjelasan visual) — https://neetcode.io/

---

> Catatan: Silabus ini dapat disesuaikan dengan jumlah SKS, bahasa pemrograman praktikum (C/C++/Python/Java), dan tingkat kedalaman materi teori kompleksitas komputasi sesuai kebutuhan program studi.
