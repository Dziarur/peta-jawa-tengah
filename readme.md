# Peta Interaktif Tingkat Pengangguran Terbuka (TPT) Jawa Tengah

Repository ini berisi skrip Python untuk memproses, menyelaraskan, dan memvisualisasikan data **Tingkat Pengangguran Terbuka (TPT)** per kabupaten/kota di Provinsi Jawa Tengah ke dalam bentuk peta tematik interaktif (*Choropleth Map*).

---

## 📊 Fitur Utama
* **Peta Tematik Choropleth:** Visualisasi wilayah berbasis gradasi warna yang merepresentasikan tinggi rendahnya angka TPT.
* **Pencocokan Data Cerdas (*Smart Name Matching*):** Algoritma pembersihan string otomatis untuk mengatasi perbedaan penulisan nama wilayah antara file data CSV dan file batas spasial GeoJSON.
* **Interaktivitas Penuh:** Dilengkapi dengan *tooltip* dinamis yang menampilkan nama wilayah beserta nilai TPT secara langsung saat kursor diarahkan, serta fitur *zoom-on-click*.
* **Transparansi Sumber:** Menyematkan informasi sumber data resmi secara langsung di dalam tampilan antarmuka peta dan skrip.

---

## 🛠️ Prasyarat & Kebutuhan Sistem
Pastikan Anda telah menginstal pustaka Python berikut di lingkungan (*environment*) Anda sebelum menjalankan skrip:

```bash
pip install pandas folium
```

---

## 📂 Struktur File
Pastikan file-file berikut berada dalam satu direktori yang sama:
```text
├── main.ipynb                  # Skrip utama python
├── data_tpt_jateng.csv         # Data statistik TPT (dari BPS)
├── peta_jateng.geojson         # Data spasial/peta wilayah Jawa Tengah
└── peta_interaktif_jateng_fix.html # File keluaran peta interaktif
```

---

## 🚀 Cara Menjalankan
1. Clone atau unduh repository ini ke komputer Anda.
2. Pastikan file CSV dan GeoJSON sudah sesuai dengan struktur kolom yang dibutuhkan.
3. Jalankan skrip Python melalui terminal atau IDE Anda
4. Buka file hasil keluaran berupa **`peta_interaktif_jateng_fix.html`** menggunakan browser web apa pun (Chrome, Edge, Firefox, dll.) untuk melihat peta interaktifnya.

---

## 🌐 Sumber Data & Komponen Pihak Ketiga (Third-Party)
Proyek ini memanfaatkan beberapa sumber data dan pustaka pihak ketiga berikut:

1. **Dataset TPT:** 
   * **Sumber:** **Badan Pusat Statistik (BPS) Provinsi Jawa Tengah**.
   * **Keterangan:** Data statistik resmi terkait persentase Tingkat Pengangguran Terbuka (TPT) tingkat kabupaten/kota 2025 (bersumber dari Survei Angkatan Kerja Nasional / Sakernas).
2. **Data Spasial / Peta Wilayah (GeoJSON):** 
   * **Sumber:** Repositori publik GitHub (salah satunya dari kontribusi akun **`ardian28`**) serta data batas administrasi wilayah Indonesia.
   * **Keterangan:** Berkas poligon geometris untuk memetakan batas wilayah administratif Jawa Tengah.
3. **Pustaka Pemrograman & Layanan Web:**
   * **Python Pandas & Folium:** Pustaka open-source untuk pemrosesan data dan perenderan peta berbasis JavaScript **Leaflet.js**.
   * **OpenStreetMap:** Penyedia ubin peta dasar (*basemap tiles*) untuk tampilan visual latar belakang peta.

---

## 📄 Lisensi
Proyek ini bersifat *open-source* dan dapat digunakan secara bebas untuk keperluan analisis data, pembelajaran, maupun portofolio profesional.

## Link Web Peta Jawa tengah Interaktif
https://peta-jawa-tengah.vercel.app/
