# Tugas Pemetaan Sederhana: Data Jalan untuk Database

Halo! Repositori ini berisi hasil tugas saya untuk mendigitalkan (memetakan) jalan dan menyimpannya ke dalam database.

## File Utama: Peta Jalan Kita (`tugas-1.geojson`)

Bayangkan ini seperti **peta digital** yang dibuat khusus untuk komputer.

* [cite_start]**Apa Isinya?** File ini berisi **14 garis** [cite: 1] yang menggambarkan jalan-jalan di satu area perumahan.
* **Kenapa Garis?** Karena jalan adalah garis (LineString) di peta.
* **Apa saja Informasi di Dalamnya?** Selain bentuk garisnya, setiap jalan punya "kartu identitas" (disebut *properties*). Jadi, kita tahu ini Jalan apa, misalnya:
    * [cite_start]**Nama Jalan:** "Jalan Sarimanah 2" [cite: 1] [cite_start]atau "Jalan Sariasih"[cite: 28, 58].
    * [cite_start]**Tipe Jalan:** Ada jalan utama (*tertiary* [cite: 58][cite_start]), jalan perumahan biasa (*residential* [cite: 1, 28][cite_start]), dan jalan-jalan kecil (*living_street* [cite: 7, 10, 16, 20, 23, 30, 34, 38, 44, 47, 54, 57]).
    * [cite_start]**Lebar/Lajur:** Ada yang punya 2 lajur [cite: 1, 57][cite_start], ada yang 1 lajur[cite: 7, 10, 16, 20, 23, 28, 30, 34, 45, 54].
    * [cite_start]**Permukaan:** Ada yang aspal [cite: 1, 16, 20, 23, 34, 45, 54][cite_start], ada yang beton (*concrete* [cite: 7, 23]).

## Cek dan Ricek Data (Validasi)

File peta ini sudah saya pastikan benar, baik bentuknya maupun isinya:

* **Bentuk Kode (Sintaks):** Kode GeoJSON-nya sudah rapi, tidak ada salah ketik atau salah taruh kurung, jadi komputer pasti bisa membacanya.
* **Bentuk di Peta (Semantik):** Garis-garis jalan ini muncul dengan benar di peta digital (saat dicek di geojson.io). Jadi, bentuknya memang sudah sesuai dengan jalan yang sebenarnya di lokasi.
