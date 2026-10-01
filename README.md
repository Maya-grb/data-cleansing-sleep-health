# Data Cleansing Dataset Sleep Health

Penerapan data cleansing menggunakan Python pada dataset kebiasaan tidur dan gaya hidup.
Dataset yang sengaja dibuat kotor (tidak urut dan format tidak konsisten) dibersihkan
agar siap dipakai untuk analisis lanjutan, yaitu pengelompokan pola tidur dengan metode K-Means.

## Isi Repository

 File 
 `2418064DataCleansing.ipynb`  Notebook proses data cleansing (Google Colab) 
 `sleep_health_data_kotor.csv`  Dataset sebelum dibersihkan 
 `sleep_health_data_bersih.csv`  Dataset setelah dibersihkan 

## Masalah pada Dataset Kotor

- Nama kolom tidak seragam (huruf besar/kecil campur, ada spasi)
- Penulisan kategori berbeda untuk makna yang sama (misalnya gender dan exercise day)
- Format angka tidak konsisten (koma desimal, angka bercampur satuan, angka ditulis dengan kata)
- Data kosong dan nilai pengganti seperti N/A dan tanda minus
- Nilai tidak logis (outlier)
- Baris duplikat dan urutan data acak

## Tahapan Data Cleansing

1. Import Libraries
2. Baca Dataset
3. Menampilkan struktur variabel dan kondisi data
4. Standarisasi nama kolom
5. Standarisasi kolom No (Primary Key)
6. Standarisasi kolom Gender dan Exercise Day
7. Standarisasi kolom numerik
8. Penanganan nilai tidak logis (outlier)
9. Deduplikasi data
10. Penanganan missing value
11. Data enrichment
12. Validasi akhir dan simpan hasil

## Hasil

Dataset bersih memiliki format yang seragam, tanpa duplikat, tanpa data kosong, dan seluruh
nilainya berada pada rentang yang masuk akal. Ditambahkan juga kolom kategori hasil enrichment
(kelompok usia, kategori durasi tidur, kualitas tidur, tingkat stres, konsumsi kafein dan alkohol,
serta total tidur sehari).

## Cara Menjalankan

1. Upload `sleep_health_data_kotor.csv` ke Google Drive, saya membuat floder barunamanya DATMIN jadi filenya ada di dalam floder DATMIN.
2. Buka `2418064DataCleansing.ipynb` di Google Colab.
3. Sesuaikan alamat file pada bagian Baca Dataset dengan lokasi file di Drive Anda.
4. Jalankan seluruh sel secara berurutan (Runtime, Run all).
5. Hasil tersimpan sebagai `sleep_health_data_bersih.csv`.

## Tools

Python, pandas, numpy, Google Colab

## Penulis

Nama: Maya Via Agustin Rahayu
NIM: 2418064
Program Studi Teknik Informatika, Institut Teknologi Nasional Malang
