# 🎬 Netflix Content Analysis Dashboard

## 📊 Overview
Sebuah *dashboard* analitik interaktif yang dirancang untuk memantau tren penambahan konten, distribusi kategori, serta karakteristik produksi dari katalog *Netflix*. Proyek ini mengubah data mentah katalog *streaming* menjadi wawasan visual strategis guna memahami pola publikasi film dan serial televisi secara global menggunakan **Microsoft Excel**.
<img width="1113" height="640" alt="da2040a5-df79-4f4b-8800-c626b4f07078" src="https://github.com/user-attachments/assets/b3d7f851-341d-4cc5-a0db-52e80f3b7eb2" />


---

## 📋 Business Questions Framework
Tabel berikut menguraikan pertanyaan bisnis utama yang terjawab melalui analisis pada *dashboard*:

| Dimensi Analisis | Pertanyaan Bisnis Utama |
| :--- | :--- |
| **Distribusi Konten** | • Berapa total keseluruhan judul yang tersedia di platform serta bagaimana perbandingan proporsi antara *Movies* dan *TV Shows*? |
| **Geografi & Produksi** | • Negara mana saja yang menjadi 5 produsen konten (*Top 5 Producing Countries*) terbanyak bagi *Netflix*? |
| **Tren & Waktu** | • Bagaimana tren pertumbuhan penambahan konten baru setiap tahunnya dari periode 2015 hingga 2021? |
| **Kategori & Genre** | • Apa saja 5 genre (*Top 5 Genres*) yang paling mendominasi di dalam platform? |

---

## 🧹 Data Cleaning & Preparation (Python / Pandas)
1. **Handling Missing Values:** Mengatasi nilai kosong pada kolom penting seperti *director*, *cast*, dan *country*.
2. **Date Parsing:** Membersihkan dan memparsing kolom tanggal untuk mengekstrak informasi tahun penambahan (`YearAdded`).
3. **Feature Engineering (`PrimaryCountry`):** Memisahkan data negara produsen utama (mengambil negara pertama dari daftar multinegara) untuk memudahkan pengelompokan wilayah.
4. **Data Validation:** Memastikan format kategori teks dan tipe data numerik sudah konsisten sebelum diekspor ke format Excel.

---

## 📊 Visualizations & Dashboard Layout (Excel)
* **Header KPI Banner:** Banner metrik utama organisasi berlatar belakang *navy blue*, menampilkan *Total Titles* (8.807), *Movies* (6.126 / 70%), *TV Shows* (2.664 / 30%), dan *Top Country* (United States).
* **Content Distribution by Type (Doughnut Chart):** Grafik donat interaktif dari *Pivot Table* yang menunjukkan dominasi film *Movie* (70%) dibandingkan *TV Show* (30%).
* **Top 5 Producing Countries (Bar Chart):** Grafik batang horizontal berwarna hijau tua yang menampilkan lima negara produsen konten teratas, dipimpin oleh *United States*, *India*, *Unknown Country*, *United Kingdom*, dan *Japan*.
* **Content Added by Year (Column Chart):** Grafik batang vertikal (*column chart*) berwarna biru cerah yang merangkum jumlah penambahan konten per tahun dari 2016 hingga 2021.
* **Annual Addition Trend (2015-2021) (Area Chart):** Grafik tren area berwarna merah/oranye transparan yang melacak lonjakan volume penambahan konten dari tahun 2015 hingga puncaknya di 2019.
* **Top 5 Genres (Bar Chart):** Grafik batang horizontal berwarna ungu yang merinci lima kategori/genre teratas di platform.

---

## 💡 Key Business Insights
1. **Dominasi Film (*Movies*):** Katalog *Netflix* didominasi secara signifikan oleh film layar lebar (*Movies*) sebesar 70% (6.126 judul), sementara serial televisi (*TV Shows*) menyumbang sekitar 30% (2.664 judul).
2. **Konsentrasi Produksi Global:** Amerika Serikat (*United States*) memegang posisi mutlak sebagai negara produsen konten terbesar, diikuti oleh India dan Inggris.
3. **Lonjakan Tren Tahunan:** Penambahan konten mengalami pertumbuhan yang sangat masif dari tahun 2015 hingga mencapai titik tertinggi di sekitar tahun 2019 sebelum akhirnya menyesuaikan di tahun-tahun berikutnya.

---

## 🚀 Strategic Recommendations
1. **Diversifikasi Konten Serial (TV Shows):** Mengingat proporsi *TV Shows* berada di angka 30%, peningkatan investasi pada produksi serial berseri (*series*) berpotensi mendongkrak retensi penonton jangka panjang.
2. **Optimasi Portofolio Genre Populer:** Memperkuat produksi dan perolehan lisensi pada genre teratas seperti *Dramas*, *International Movies*, dan *Documentaries* guna mempertahankan tingkat *engagement* pengguna.
3. **Ekspansi Kemitraan Global:** Memperluas kolaborasi produksi lokal di luar Amerika Serikat dan India untuk memperkaya variasi katalog regional di platform.

---

## 🛠️ Tools Used
* **Python (Pandas):** Digunakan untuk tahapan awal pembersihan data (*data cleaning*) dan *feature engineering* pada dataset `netflix_titles.csv`.
* **Microsoft Excel:** Platform utama untuk perancangan *Pivot Table*, *Pivot Charts* dinamis, penyesuaian format angka/desimal, perapian sumbu grafik, hingga penyusunan tata letak *dashboard* akhir secara profesional.
