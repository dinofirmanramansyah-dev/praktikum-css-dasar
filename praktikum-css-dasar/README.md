# Laporan Praktikum  - Pemrograman Web Dasar (CSS)

**Nama:** Dino Firman Ramansyah  
**Instansi:** Universitas Pelita Bangsa  

## Jawaban Pertanyaan dan Tugas Modul

### 1. Perbedaan Selektor `h1` dan `#intro h1`
* **`h1` (Element Selector):** Mengatur gaya untuk **semua** elemen `<h1>` yang ada di dalam dokumen HTML secara keseluruhan/global.
* **`#intro h1` (Descendant Selector):** Hanya mengatur elemen `<h1>` yang berada **secara khusus di dalam** elemen pembungkus (seperti `<div>`) yang memiliki `id="intro"`. Elemen `<h1>` lain di luar ID tersebut tidak akan berubah gaya visualnya.

### 2. Urutan Prioritas CSS (Internal, Eksternal, dan Inline CSS)
Jika suatu elemen dikenakan tiga jenis CSS sekaligus secara bersamaan, maka yang akan dimenangkan dan ditampilkan oleh browser adalah **Inline CSS**.
* **Alasan:** Inline CSS ditulis langsung pada atribut tag HTML (seperti tag `<p style="...">`), sehingga memiliki tingkat spesifisitas (*<span>specificity score</span>*) yang paling tinggi dibandingkan Internal CSS (tag `<style>`) maupun Eksternal CSS (file `.css` terpisah).

### 3. Prioritas ID Selector vs Class Selector
Apabila ada bentrokan gaya antara ID Selector dan Class Selector pada satu elemen yang sama, browser akan memprioritaskan gaya dari **ID Selector**.
* **Alasan:** Browser memberikan bobot nilai spesifisitas yang jauh lebih tinggi pada ID Selector (skor 100) dibandingkan dengan Class Selector (skor 10). Oleh karena itu, aturan dekorasi pada ID akan selalu menimpa Class.