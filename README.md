# Prediksi Nilai Ekspor Komoditas Indonesia

Proyek ini merupakan penelitian mengenai prediksi nilai ekspor komoditas Indonesia menggunakan metode Decision Tree Regression. Data yang digunakan merupakan data bulanan yang bersumber dari BPS dengan periode 2022–2024.

## Tujuan

Penelitian ini bertujuan untuk membangun model yang dapat memprediksi nilai ekspor komoditas Indonesia serta mengetahui kinerja model berdasarkan beberapa skenario pembagian data.

## Data

Data yang digunakan dalam penelitian melalui beberapa tahap pengolahan, yaitu:

- Data mentah
- Data bersih
- Data siap digunakan untuk pemodelan

Dataset akhir yang digunakan dalam pemodelan terdiri dari 3.587 record.

## Pengolahan Data

Sebelum digunakan untuk pemodelan, data melalui beberapa tahap pengolahan, meliputi:

- Pembersihan data
- Penanganan nilai kosong
- Penyesuaian format dan struktur data
- Transformasi data
- Normalisasi
- Pengelompokan komoditas
- Pembentukan variabel lag
- Pembentukan atribut Pertumbuhan_Ekspor

Tahapan tersebut dilakukan untuk menghasilkan dataset yang lebih terstruktur dan sesuai dengan kebutuhan pemodelan.

## Pemodelan

Pemodelan dilakukan menggunakan Decision Tree Regression pada RapidMiner Studio.

Pengujian dilakukan dengan empat skenario pembagian data:

- Random split 70:30
- Random split 80:20
- Time-based split 1
- Time-based split 2

Evaluasi model dilakukan menggunakan Root Mean Squared Error (RMSE) dan Mean Absolute Error (MAE).

## Hasil

Hasil pengujian menunjukkan bahwa skenario time-based split 2 memberikan hasil terbaik.

Pada skenario tersebut, data Januari 2022 hingga Mei 2024 digunakan sebagai data pelatihan, sedangkan data Juni hingga Desember 2024 digunakan sebagai data pengujian.

Hasil evaluasi:

- RMSE: 0,027
- MAE: 0,017

Hasil tersebut menunjukkan bahwa model menghasilkan tingkat kesalahan prediksi yang rendah pada data penelitian.

## Variabel yang Berpengaruh

Berdasarkan struktur pohon yang dihasilkan, variabel yang berperan dominan dalam pembentukan model adalah:

- Average_Nilai_Ekspor_USD
- Periode_Index
- Pertumbuhan_Ekspor

## Tools

- Microsoft Excel
- RapidMiner Studio
- Decision Tree Regression

## Dokumentasi

Repository ini berisi dataset yang digunakan dalam penelitian serta dokumentasi tahapan pengolahan data, pemodelan, dan hasil prediksi menggunakan RapidMiner Studio.
