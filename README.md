# Job Scheduling Algorithms

## Anggota
- 103012380503 - Muhammad Idris
- 103012380520 - Fikri Ramandha Noor
- 103012380547 - Rifki Padilah

## Deskripsi

Proyek ini membandingkan dua algoritma penjadwalan pekerjaan, yaitu algoritma Greedy dan Dynamic Programming, dalam hal waktu eksekusi untuk berbagai jumlah pekerjaan. Algoritma-algoritma tersebut digunakan untuk menjadwalkan pekerjaan berdasarkan waktu pemrosesan dan tanggal jatuh tempo (due date) untuk meminimalkan total keterlambatan.

## Struktur Proyek

- `dummy_data.csv`: File CSV yang berisi data dummy pekerjaan dengan ID, waktu pemrosesan, dan tanggal jatuh tempo.
- `tubes.py`: Script utama yang memuat data, mendefinisikan kelas `Job`, mengimplementasikan algoritma penjadwalan, mengukur waktu eksekusi, dan memplot hasilnya.

## Instalasi

1. Clone repositori ini:

   ```bash
   git clone https://github.com/mhmadidris/tubes-strategi-algoritma.git
   ```

2. Instal dependensi yang diperlukan:
   ```bash
   pip install pandas matplotlib
   ```

## Cara Penggunaan

1. Pastikan file `dummy_data.csv` berada di direktori yang sama dengan `tubes.py`.

2. Jalankan script `tubes.py`:

   ```bash
   python tubes.py
   ```

3. Hasil waktu eksekusi untuk setiap algoritma dan jumlah pekerjaan akan dicetak di terminal, dan grafik perbandingan waktu eksekusi akan ditampilkan.

## Algoritma yang Digunakan

### 1. Greedy

Algoritma Greedy menyortir pekerjaan berdasarkan tanggal jatuh tempo (due date) dan menjadwalkan pekerjaan satu per satu. Jika waktu saat ini melebihi tanggal jatuh tempo pekerjaan, total keterlambatan dihitung.

### 2. Dynamic Programming

Algoritma Dynamic Programming menggunakan tabel `dp` untuk melacak minimum keterlambatan untuk sejumlah pekerjaan tertentu dan waktu tertentu. Algoritma ini lebih kompleks dan mempertimbangkan setiap pekerjaan secara bertahap untuk meminimalkan total keterlambatan.

## Hasil dan Analisis

Hasil waktu eksekusi untuk kedua algoritma akan dicetak di terminal dalam format berikut:
