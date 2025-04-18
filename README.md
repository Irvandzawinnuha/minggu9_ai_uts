# 📦 minggu9_ai_uts_kecerdasan buatan

**Minggu 9 Case Based – Searching Kecerdasan Buatan AI menggunakan Python dengan manual.**  
Seluruh proses dibangun tanpa menggunakan library khusus seperti DEAP, PyGAD, dll.

---
## Kelompok
- **Irvan Dzawin Nuha – 1302223076**
- **Joshua Daniel Simanjuntak – 1302220072**
---

## 📌 Deskripsi

Tugas ini bertujuan untuk meminimalkan fungsi dua variabel berikut dengan pendekatan *Genetic Algorithm (GA)*:

![soal minggu 9 ai uts tubes](https://github.com/user-attachments/assets/59843c40-810c-4653-a620-0bc139e7ca20)


Program dibangun dari nol menggunakan Python, dan semua komponen GA diimplementasikan secara manual (tanpa library GA).

---

## 🔧 Parameter GA

| Parameter           | Nilai                            |
|--------------------|----------------------------------|
| Jumlah Populasi    | 50                               |
| Panjang Kromosom   | 32 bit (16 bit untuk masing-masing x1 dan x2) |
| Rentang Nilai      | [-10, 10] untuk x1 dan x2         |
| Probabilitas Crossover | 0.9 (90%)                    |
| Probabilitas Mutasi | 1 / panjang_kromosom (= 3.125%)   |
| Generasi           | 100 iterasi                      |
| Seleksi Orang Tua  | Tournament Selection              |
| Crossover          | One-point Crossover               |
| Mutasi             | Bit Flip                          |
| Replacement        | Steady-State Replacement          |

---

## ⚙️ Alur Proses GA
1. Inisialisasi populasi acak.
2. Decode kromosom biner ke real \(x1\) dan \(x2\).
3. Evaluasi fitness setiap individu.
4. Seleksi orang tua via turnamen.
5. Crossover untuk menghasilkan offspring.
6. Mutasi bit secara acak.
7. Seleksi survivor dan generational replacement.
8. Ulangi hingga generasi terakhir.
9. Tampilkan kromosom terbaik dan nilai \(x1\), \(x2\), serta fitness-nya.

---

## 💻 Contoh Output
```txt
Best Chromosome: 10100101101101101100110101101101
x1 = -3.214, x2 = 6.902
Fitness = -1.98321
