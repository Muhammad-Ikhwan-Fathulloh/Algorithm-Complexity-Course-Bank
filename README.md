# Kompleksitas Algoritma (Analysis & Design of Algorithms)

Silabus **16 pertemuan** (14 pertemuan materi, **UTS di P8**, **UAS di P16**). Kerangka klasiknya mengacu pada ITB (IF2211 Strategi Algoritma, Rinaldi Munir), MIT 6.006/6.046J, Stanford CS161, Princeton (Sedgewick & Wayne) dan CLRS. Versi ini diperbarui dengan **jalur AI dan algoritma modern**: kompleksitas pencarian dan inferensi pada sistem pakar, SAT/CSP solver, A\*, DP pada pemrosesan sekuens, *approximate nearest neighbor*, serta kompleksitas Transformer.

---

## Deskripsi Mata Kuliah

Mata kuliah ini membahas analisis efisiensi algoritma (waktu dan ruang), notasi asimtotik, teknik desain algoritma (*brute force, divide and conquer, greedy, dynamic programming, backtracking, branch and bound*), dan batas komputasi (P vs NP). Setiap teknik dikaitkan dengan penerapannya di bidang kecerdasan buatan dan sistem skala besar, misalnya pencarian ruang keadaan, inferensi berbasis aturan pada sistem pakar, solver SAT/CSP, pencarian vektor, dan biaya komputasi model bahasa.

## Capaian Pembelajaran

1. Menganalisis kompleksitas waktu dan ruang algoritma dengan notasi asimtotik.
2. Menyelesaikan persamaan rekurens (Master Theorem, recursion tree, substitusi).
3. Memilih dan merancang strategi algoritma yang sesuai untuk suatu persoalan.
4. Memahami batas komputasi (P, NP, NP-Complete, NP-Hard) dan dampaknya pada AI simbolik maupun statistik.
5. Menganalisis kompleksitas komponen sistem AI modern (search, inferensi logika, DP sekuens, attention, ANN).
6. Menerapkan analisis kompleksitas pada konteks industri dan benchmarking empiris.

---

## Sumber Referensi

### Buku teks utama
| Sumber | Penulis | Tautan |
|---|---|---|
| *Introduction to Algorithms* (CLRS) | Cormen, Leiserson, Rivest, Stein | https://mitpress.mit.edu/9780262046305/introduction-to-algorithms/ |
| *Algorithm Design* | Kleinberg & Tardos | https://www.pearson.com/en-us/subject-catalog/p/algorithm-design/P200000003259 |
| *Algorithms* (4th ed.) | Sedgewick & Wayne | https://algs4.cs.princeton.edu/home/ |
| *Algorithms* | Dasgupta, Papadimitriou, Vazirani | https://people.eecs.berkeley.edu/~vazirani/algorithms.html |
| *Algorithms* (gratis) | Jeff Erickson, UIUC | https://jeffe.cs.illinois.edu/teaching/algorithms/ |
| *The Algorithm Design Manual* | Steven Skiena | https://www.algorist.com/ |
| *Algorithms Illuminated* | Tim Roughgarden | https://www.algorithmsilluminated.org/ |
| *Artificial Intelligence: A Modern Approach* (AIMA) | Russell & Norvig | https://aima.cs.berkeley.edu/ |
| *Computational Complexity: A Modern Approach* | Arora & Barak | https://theory.cs.princeton.edu/complexity/ |
| *The Design of Approximation Algorithms* | Williamson & Shmoys | https://www.designofapproxalgs.com/ |
| *Probability and Computing* | Mitzenmacher & Upfal | https://www.cambridge.org/core/books/probability-and-computing/ |

### Kuliah terbuka (algoritma)
| Sumber | Institusi | Tautan |
|---|---|---|
| IF2211 Strategi Algoritma (slide, diktat) | STEI ITB, Rinaldi Munir | https://informatika.stei.itb.ac.id/~rinaldi.munir/Stmik/ |
| Playlist video Strategi Algoritma | ITB | https://www.youtube.com/playlist?list=PLyYkJZR4un3pdFjgNZU9sO3Lg0uezCTeW |
| 6.006 Introduction to Algorithms (Spring 2020) | MIT OCW | https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/ |
| 6.046J Design and Analysis of Algorithms | MIT OCW | https://ocw.mit.edu/courses/6-046j-design-and-analysis-of-algorithms-spring-2015/ |
| CS161 Design and Analysis of Algorithms | Stanford | https://cs161-stanford.github.io/ |
| CS168 The Modern Algorithmic Toolbox | Stanford | https://web.stanford.edu/class/cs168/ |
| Algorithms Part I & II | Princeton (Coursera) | https://www.coursera.org/learn/algorithms-part1 · https://www.coursera.org/learn/algorithms-part2 |

### Kuliah terbuka (AI dan sistem modern)
| Sumber | Institusi | Tautan |
|---|---|---|
| 6.034 Artificial Intelligence (termasuk rule-based expert systems, search, CSP) | MIT OCW | https://ocw.mit.edu/courses/6-034-artificial-intelligence-fall-2010/ |
| CS188 Introduction to AI | UC Berkeley | https://inst.eecs.berkeley.edu/~cs188/ |
| CS221 Artificial Intelligence: Principles and Techniques | Stanford | https://web.stanford.edu/class/cs221/ |
| CS50's Introduction to AI with Python | Harvard | https://cs50.harvard.edu/ai/ |
| 6.5940 TinyML and Efficient Deep Learning | MIT (Song Han) | https://hanlab.mit.edu/courses/2024-fall-65940 |
| CS336 Language Modeling from Scratch | Stanford | https://stanford-cs336.github.io/ |

### Makalah dan sumber riset
| Sumber | Tautan |
|---|---|
| Vaswani dkk., *Attention Is All You Need* (2017) | https://arxiv.org/abs/1706.03762 |
| Tay dkk., *Efficient Transformers: A Survey* | https://arxiv.org/abs/2009.06732 |
| Dao dkk., *FlashAttention* (2022) | https://arxiv.org/abs/2205.14135 |
| Malkov & Yashunin, *HNSW* (ANN search) | https://arxiv.org/abs/1603.09320 |
| Fawzi dkk., *AlphaTensor* (Nature, 2022) | https://www.nature.com/articles/s41586-022-05172-4 |
| Mankowitz dkk., *AlphaDev* (Nature, 2023) | https://www.nature.com/articles/s41586-023-06004-9 |
| Forgy, *Rete Algorithm* (1982), untuk pencocokan aturan sistem pakar | https://doi.org/10.1016/0004-3702(82)90020-0 |

### Praktik industri, latihan, dan alat bantu
| Sumber | Tautan |
|---|---|
| Google Tech Dev Guide | https://techdevguide.withgoogle.com/paths/data-structures-and-algorithms/ |
| NeetCode | https://neetcode.io/ |
| LeetCode | https://leetcode.com/ |
| Codeforces | https://codeforces.com/ |
| USACO Guide | https://usaco.guide/ |
| CP-Algorithms | https://cp-algorithms.com/ |
| VisuAlgo (visualisasi algoritma) | https://visualgo.net/ |
| Python TimeComplexity | https://wiki.python.org/moin/TimeComplexity |
| Big-O Cheat Sheet | https://www.bigocheatsheet.com/ |
| Google OR-Tools (CP-SAT, routing) | https://developers.google.com/optimization |
| CLIPS (shell sistem pakar) | https://www.clipsrules.net/ |
| FAISS (pencarian vektor) | https://github.com/facebookresearch/faiss |
| Concorde TSP Solver | https://www.math.uwaterloo.ca/tsp/concorde.html |

---

## Rencana 16 Pertemuan

UTS menempati **Pertemuan 8** dan UAS menempati **Pertemuan 16**. Tanda **[Modern]** menandai bagian yang ditambahkan dari jalur AI dan sistem skala besar.

### Pertemuan 1: Pendahuluan dan Notasi Asimtotik
- **Topik:** Model komputasi RAM; Big-O, Omega, Theta, little-o; analisis best/average/worst case. **[Modern]** Mengapa kompleksitas penting di era AI: biaya komputasi *training* dan *inference*.
- **Sumber:** ITB Strategi Algoritma; MIT 6.006; CLRS Bab 3; Erickson (bab *Recurrences & Asymptotics*).
- **Praktik:** Menghitung kompleksitas potongan kode (loop, nested loop) dan mengukur waktu eksekusi empiris.
- **Tugas:** Latihan notasi asimtotik.

### Pertemuan 2: Rekursi dan Persamaan Rekurens
- **Topik:** Recursion tree, substitusi, Master Theorem, Akra-Bazzi (pengantar).
- **Sumber:** MIT 6.006; Stanford CS161; CLRS Bab 4; Roughgarden, *Algorithms Illuminated* Bagian 1.
- **Praktik:** Menyelesaikan T(n) = 2T(n/2) + n, T(n) = 7T(n/2) + n², dan sejenisnya.
- **Tugas:** Rekurens Merge Sort dan Binary Search.

### Pertemuan 3: Brute Force, Exhaustive Search, dan Pencarian Ruang Keadaan
- **Topik:** Brute force, kompleksitas eksponensial/faktorial (TSP). **[Modern]** Pencarian ruang keadaan pada AI: BFS, DFS, uniform-cost, iterative deepening; kompleksitas O(b^d) dan trade-off waktu vs memori.
- **Sumber:** ITB (Brute Force); AIMA Bab 3; Berkeley CS188 (Search); CS50 AI (Search).
- **Praktik:** Selection sort, string matching brute force; 8-puzzle dengan BFS dan DFS.
- **Tugas:** Analisis kompleksitas brute force TSP dan perbandingan metode pencarian pada 8-puzzle.

### Pertemuan 4: Divide and Conquer I
- **Topik:** Divide, conquer, combine; Merge Sort, Quick Sort, Binary Search, Quickselect.
- **Sumber:** ITB (Divide and Conquer); MIT 6.006; Stanford CS161; Sedgewick & Wayne Bab 2.
- **Praktik:** Benchmark Merge Sort vs Quick Sort pada berbagai distribusi data.
- **Tugas:** Perbandingan performa teoritis dan empiris.

### Pertemuan 5: Divide and Conquer II
- **Topik:** Closest Pair, perkalian bilangan Karatsuba, Strassen, FFT. **[Modern]** Penemuan algoritma dengan AI: AlphaTensor (perkalian matriks) dan AlphaDev (sorting).
- **Sumber:** MIT 6.046J; Kleinberg & Tardos Bab 5; CLRS Bab 4 dan 30; makalah AlphaTensor dan AlphaDev.
- **Praktik:** Closest Pair; implementasi Karatsuba/Strassen.
- **Tugas:** Mini proyek Strassen dan analisis titik impas (*crossover point*) terhadap algoritma naif.

### Pertemuan 6: Decrease and Conquer dan Struktur Data Efisien
- **Topik:** Decrease by constant/factor/variable, Insertion Sort, DFS/BFS, Topological Sort; Heap, Hash Table, Balanced BST; analisis teramortisasi. **[Modern]** Struktur data probabilistik: Bloom filter dan Count-Min Sketch.
- **Sumber:** ITB (Decrease and Conquer); CLRS Bab 6, 10-13, 16 (amortized); Stanford CS168; Python TimeComplexity.
- **Praktik:** Membandingkan kompleksitas operasi struktur data; mengukur dict/set di Python.
- **Tugas:** Studi kasus pemilihan struktur data untuk mengoptimalkan suatu algoritma.

### Pertemuan 7: Greedy Algorithms I
- **Topik:** Prinsip greedy, *exchange argument*, Activity Selection, Fractional Knapsack, penjadwalan. **[Modern]** Greedy decoding vs beam search pada model bahasa (kapan greedy tidak optimal).
- **Sumber:** ITB (Algoritma Greedy); MIT 6.046J; Kleinberg & Tardos Bab 4; Stanford CS336 (decoding).
- **Praktik:** Activity Selection; contoh tandingan (*counterexample*) untuk greedy yang salah.
- **Tugas:** Studi kasus job scheduling.

### Pertemuan 8: UTS (Ujian Tengah Semester)
- **Cakupan:** Pertemuan 1-7.
- **Bentuk:** Tertulis; analisis kompleksitas, penyelesaian rekurens, perancangan algoritma (brute force, D&C, decrease and conquer, greedy), analisis ruang pencarian.

### Pertemuan 9: Greedy II (Graf) dan Pencarian Heuristik
- **Topik:** Kruskal, Prim (MST), Dijkstra, Huffman Coding. **[Modern]** A\* dan heuristik admissible/consistent; kompleksitas A\* dan hubungannya dengan Dijkstra.
- **Sumber:** ITB; Stanford CS161; CLRS Bab 21-24; AIMA Bab 3; Berkeley CS188 (A\* Search).
- **Praktik:** Implementasi MST dan shortest path; A\* pada peta/grid dengan heuristik Manhattan.
- **Tugas:** Kruskal vs Prim terhadap struktur data; Dijkstra vs A\*.

### Pertemuan 10: Dynamic Programming I
- **Topik:** *Overlapping subproblems*, *optimal substructure*, memoization vs tabulation, 0/1 Knapsack, Fibonacci, kompleksitas pseudo-polinomial.
- **Sumber:** ITB (Program Dinamis); MIT 6.006 (DP); Erickson (bab DP); Coursera Algorithms Part II.
- **Praktik:** 0/1 Knapsack top-down dan bottom-up; optimasi ruang.
- **Tugas:** Analisis waktu/ruang DP.

### Pertemuan 11: Dynamic Programming II
- **Topik:** LCS, Edit Distance, Matrix Chain, Bellman-Ford, Floyd-Warshall. **[Modern]** DP pada pemrosesan sekuens: algoritma Viterbi (HMM), CKY parsing, penjajaran sekuens (*sequence alignment*) dan *dynamic time warping*.
- **Sumber:** CLRS Bab 14; MIT 6.046J; Stanford CS161; AIMA (bab inferensi temporal); Jurafsky & Martin, *Speech and Language Processing* (https://web.stanford.edu/~jurafsky/slp3/).
- **Praktik:** Edit distance untuk spell checker/diff; implementasi Viterbi sederhana.
- **Tugas:** Mini proyek DP pilihan mahasiswa.

### Pertemuan 12: Backtracking dan Constraint Satisfaction
- **Topik:** *State space tree*, pruning, N-Queens, Sudoku, Subset Sum, Hamiltonian Cycle. **[Modern]** CSP: *forward checking*, propagasi kendala (AC-3), heuristik MRV/LCV.
- **Sumber:** ITB (Runut-balik); AIMA Bab 6; Berkeley CS188 (CSP); Kleinberg & Tardos; Google OR-Tools (CP-SAT).
- **Praktik:** N-Queens dan Sudoku; membandingkan backtracking murni dengan backtracking + propagasi.
- **Tugas:** Studi kasus CSP (penjadwalan kuliah, pewarnaan graf).

### Pertemuan 13: Branch and Bound dan Optimasi Kombinatorial
- **Topik:** Branch and Bound (TSP, 0/1 Knapsack), *bounding function*, perbandingan dengan backtracking. **[Modern]** Integer Linear Programming dan MIP solver di industri (logistik, routing).
- **Sumber:** ITB (Branch and Bound); CLRS; Google OR-Tools; Concorde TSP Solver.
- **Praktik:** TSP dengan Branch and Bound; menyelesaikan model yang sama dengan OR-Tools.
- **Tugas:** Efisiensi Branch and Bound vs Backtracking pada persoalan yang sama.

### Pertemuan 14: Teori Kompleksitas, SAT, dan Inferensi Logika
- **Topik:** P, NP, NP-Complete, NP-Hard, reduksi polinomial, Cook-Levin. **[Modern]** Kompleksitas inferensi logika: SAT dan algoritma DPLL/CDCL; entailment proposisional bersifat co-NP-complete, tetapi untuk klausa Horn (forward/backward chaining, inti sistem pakar berbasis aturan) berjalan linear; logika orde pertama bersifat semi-decidable; algoritma Rete untuk pencocokan aturan.
- **Sumber:** CLRS Bab 34; MIT 6.046J; Arora & Barak; AIMA Bab 7-9; MIT 6.034 (rule-based systems); Forgy (Rete); CLIPS.
- **Praktik:** Reduksi 3-SAT ke Clique/Vertex Cover; forward chaining pada basis aturan kecil (CLIPS atau Python).
- **Tugas:** Klasifikasi persoalan (P atau NP-Complete) dan analisis kompleksitas mesin inferensi sistem pakar.

### Pertemuan 15: Aproksimasi, Randomized, dan Algoritma Skala Besar
- **Topik:** Algoritma aproksimasi (Vertex Cover, TSP metrik), Randomized Quick Sort, algoritma Las Vegas vs Monte Carlo. **[Modern]** *Locality-Sensitive Hashing* dan ANN (HNSW, FAISS) untuk pencarian vektor; kompleksitas self-attention O(n²) dan varian efisien (FlashAttention, *sparse/linear attention*); studi kasus industri dan technical interview.
- **Sumber:** Williamson & Shmoys; Mitzenmacher & Upfal; Kleinberg & Tardos Bab 11 dan 13; Stanford CS168 dan CS336; MIT 6.5940; makalah *Attention Is All You Need*, *Efficient Transformers*, *FlashAttention*, *HNSW*; Google Tech Dev Guide; NeetCode.
- **Praktik:** Membandingkan pencarian tetangga terdekat eksak vs ANN; mengukur waktu dan memori attention terhadap panjang sekuens.
- **Tugas:** Refleksi akhir: peta konsep seluruh materi dan hubungannya dengan sistem AI.

### Pertemuan 16: UAS (Ujian Akhir Semester)
- **Cakupan:** Pertemuan 9-15, dapat bersifat komprehensif.
- **Bentuk:** Tertulis; perancangan algoritma (DP, backtracking, branch and bound), analisis kompleksitas, klasifikasi P/NP, dan analisis kompleksitas komponen sistem AI.

---

## Evaluasi

| Evaluasi | Waktu | Cakupan | Bobot |
|---|---|---|---|
| Kuis/Tugas mingguan | Sepanjang semester | Materi tiap pertemuan | 20% |
| Proyek/Mini Project | Dikumpulkan sebelum Pertemuan 16 | Menerapkan minimal 2 strategi algoritma | 20% |
| UTS | Pertemuan 8 | Pertemuan 1-7 | 25% |
| UAS | Pertemuan 16 | Pertemuan 9-15 (dapat komprehensif) | 35% |

## Proyek Akhir (Opsional)

Pilih satu persoalan nyata, misalnya optimasi rute, penjadwalan, pencarian teks, mesin inferensi sistem pakar mini, atau pencarian vektor, lalu:
1. Rancang minimal dua strategi algoritma berbeda (mis. brute force vs DP, backtracking vs CSP solver, eksak vs aproksimasi).
2. Analisis kompleksitas masing-masing secara teoritis.
3. Lakukan benchmarking empiris dan bandingkan dengan prediksi teoritis.
