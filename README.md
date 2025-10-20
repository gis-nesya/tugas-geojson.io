🌎 Tugas Pemetaan Geospasial: Jaringan Jalan Area Sarimanah
Proyek ini adalah penyelesaian tugas untuk membuat, memvalidasi, dan mengintegrasikan data geospasial (jalan) dalam format GeoJSON ke dalam alur kerja pengembangan menggunakan GitHub dan MongoDB.

1. Data GeoJSON (LineString)
Data yang digunakan bersumber dari file tugas-1.geojson. File ini memetakan jaringan jalan di sebuah area residensial, di mana jalan utama yang teridentifikasi dalam properti data adalah Jalan Sarimanah dan Jalan Sariasih.

Data ini terdiri dari total 15 segmen jalan  (Feature) yang direpresentasikan menggunakan tipe geometri LineString. Setiap Feature LineString menyimpan atribut penting, seperti tipe jalan (residential, living_street, atau tertiary) , lebar jalan , dan koordinat geografisnya.

2. Validasi Sintaks dan Semantik
Struktur GeoJSON dari file tugas-1.geojson sudah memenuhi standar GeoJSON.

Sintaks: Struktur data FeatureCollection yang membungkus 15 Feature LineString  sudah terjamin kebenarannya secara sintaksis.

Semantik: Apabila data ini dibuka pada platform visualisasi (seperti geojson.io), semua 15 segmen jalan akan berhasil dirender dan ditampilkan sebagai garis yang terhubung, yang mengonfirmasi validitasnya secara semantik.

3. Dokumentasi dan Penyimpanan di GitHub
File GeoJSON yang telah divalidasi, yaitu tugas-1.geojson, telah diunggah ke repositori GitHub ini. Repositori ini berfungsi sebagai tempat penyimpanan data geospasial dan dokumentasi resmi proyek.

4. Integrasi Akhir dengan MongoDB
Data dari file GeoJSON telah berhasil diimpor ke database NoSQL MongoDB.

Sesuai dengan persyaratan tugas, aturan impor yang diterapkan adalah satu jalan (Feature) diubah menjadi satu record (dokumen). Dengan adanya 15 Feature di dalam file, impor ke MongoDB menghasilkan 15 dokumen di dalam collection, di mana setiap dokumen menyimpan geometri LineString lengkap dan properti dari satu segmen jalan.
