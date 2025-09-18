# 🗺️ Klastering Angka Perceraian di Indonesia Berdasarkan Penyebab

Repositori ini berisi analisis klastering (clustering) untuk mengelompokkan provinsi di Indonesia berdasarkan faktor-faktor penyebab perceraian. Proyek ini menggunakan data resmi dari **Badan Pusat Statistik (BPS)** tahun 2024 dan dilengkapi dengan visualisasi peta interaktif menggunakan **Leaflet**.



## 📝 Deskripsi Proyek

Tujuan utama dari proyek ini adalah untuk mengidentifikasi pola dan kesamaan karakteristik antar provinsi di Indonesia berdasarkan berbagai faktor penyebab perceraian yang tercatat. Dengan menggunakan algoritma clustering, kita dapat melihat provinsi mana saja yang memiliki profil penyebab perceraian yang serupa.

Hasil dari analisis ini divisualisasikan dalam bentuk peta klastering interaktif, di mana setiap provinsi akan dikelompokkan ke dalam klaster tertentu yang ditandai dengan warna yang berbeda.

---
## 📊 Sumber Data

Data yang digunakan dalam analisis ini berasal dari tabel **"Jumlah Perceraian Menurut Provinsi dan Faktor Penyebab Perceraian (perkara), 2024"** yang dipublikasikan oleh **Badan Pusat Statistik (BPS)**.

-   **Sumber**: [BPS - Jumlah Perceraian Menurut Provinsi dan Faktor Penyebab](https://www.bps.go.id/id/statistics-table/3/YVdoU1IwVmlTM2h4YzFoV1psWkViRXhqTlZwRFVUMDkjMw==/jumlah-perceraian-menurut-provinsi-dan-faktor-penyebab-perceraian--perkara---2024.html?year=2024)
-   **Tahun Data**: 2024

Faktor-faktor penyebab yang dianalisis meliputi:
-   Zina
-   Mabuk
-   Madat
-   Judi
-   Meninggalkan salah satu pihak
-   Dan lain-lain (sesuai kolom pada data BPS)

---

## ⚙️ Metodologi

Analisis ini dilakukan dengan beberapa tahapan utama:

1.  **Pengumpulan Data**: Data diambil dari situs resmi BPS.
2.  **Pembersihan Data (Data Cleaning)**: Menangani nilai yang hilang (missing values), memperbaiki tipe data, dan melakukan normalisasi atau standarisasi agar skala data antar kolom seimbang.
3.  **Analisis Eksplorasi Data (EDA)**: Memahami distribusi dan korelasi antar variabel penyebab perceraian.
4.  **Pemodelan Klastering**: Menerapkan algoritma clustering (misalnya **K-Means**) untuk mengelompokkan provinsi. Penentuan jumlah klaster optimal dilakukan menggunakan metode seperti *Elbow Method* atau *Silhouette Score*.
5.  **Visualisasi**: Hasil klastering divisualisasikan ke dalam peta interaktif menggunakan library **Folium** (sebagai wrapper Python untuk Leaflet.js). Setiap klaster diberi warna yang berbeda untuk kemudahan interpretasi.


## 🌐 Visualisasi Peta Leaflet

Hasil akhir dari analisis ini adalah sebuah peta interaktif yang menunjukkan pengelompokan (klaster) setiap provinsi di Indonesia.

**Fitur Peta:**
-   **Marker Klaster**: Setiap provinsi ditandai dengan marker yang warnanya sesuai dengan klaster hasil analisis.
-   **Informasi Pop-up**: Klik pada setiap marker untuk melihat informasi detail seperti nama provinsi, nomor klaster, dan data penyebab perceraian yang dominan di provinsi tersebut.
