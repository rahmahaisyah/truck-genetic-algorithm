# 🚚 Case Based: Genetic Algorithm untuk Optimasi Muatan Truk

## 📘 Deskripsi Kasus
**Mata Kuliah**: Kecerdasan Buatan  
**Semester**: Ganjil 2024/2025  
**Jenis Kasus**: Searching – Genetic Algorithm  

### 👥 Kelompok:
- Rahmah Aisyah – 103022300014  
- Dewanta Rahma Satria – 103022300071  

---

## 🧩 Deskripsi Masalah

Sebuah perusahaan logistik memiliki armada truk yang digunakan untuk mengangkut berbagai jenis barang dari gudang pusat ke lokasi distribusi.  
Setiap truk memiliki batas maksimal kapasitas muatan (dalam kilogram). Tujuan perusahaan adalah **memaksimalkan nilai total muatan** (berupa estimasi profit, urgensi, atau nilai bisnis dari barang), **tanpa melebihi batas berat truk**.

Permasalahan ini merupakan bentuk klasik dari **Knapsack Problem**, dan dalam proyek ini diselesaikan menggunakan pendekatan **Genetic Algorithm (GA)**.

---

## 🛠 Implementasi Program

- **Bahasa Pemrograman**: Python
- **Library Eksternal**: Tidak menggunakan library yang secara langsung menjalankan proses GA (misalnya: `deap`, `pygad`, dll)

### 📌 Representasi Genetik:

- **Genom**: Representasi biner (`0` dan `1`) untuk setiap barang  
  `1` → barang dimuat  
  `0` → barang tidak dimuat  

- **Fitness Function**: 
  - Menjumlahkan nilai semua barang yang dimuat
  - Jika total berat melebihi kapasitas truk → fitness = 0 (penalti)

- **Operator GA**:
  - Seleksi: Random tournament
  - Crossover: One-point crossover
  - Mutasi: Mutasi bit secara acak

---
