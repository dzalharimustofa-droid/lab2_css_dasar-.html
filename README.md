Praktikum 3: CSS Dasar - Pemrograman Web

Repositori ini berisi laporan praktikum untuk mata kuliah Pemrograman Web di Universitas Pelita Bangsa, materi Praktikum 3: CSS Dasar.

Dibuat oleh: Agung Nugroho (Modul Praktikum) / Dikerjakan oleh mahasiswa.

🎯 Tujuan Praktikum

Mahasiswa mampu memahami konsep dasar CSS.

Mahasiswa mampu memahami aturan penulisan pada CSS.

Mahasiswa mampu memahami selector sebagai pengontrol CSS.

Mahasiswa mampu membuat pengaturan CSS pada HTML.

🛠️ Langkah-Langkah Praktikum

1. Membuat Dokumen HTML (lab2_css_dasar.html)

Membuat struktur dasar dokumen HTML yang berisi bagian header, navigasi, serta konten teks dengan pembungkus ID dan Class selector.

Hasil Tampilan: Dokumen HTML dasar sebelum diberikan styling tambahan.

2. Mendeklarasikan CSS Internal

Menambahkan tag <style> pada bagian <head> dokumen untuk mengatur gaya elemen dasar seperti body, header, dan tag h1.

Kode Utama:

<style>
  body { font-family: 'Open Sans', sans-serif; }
  header { min-height: 80px; border-bottom: 1px solid #77CCEF; }
  h1 { font-size: 24px; color: #0F189F; text-align: center; padding: 20px 10px; }
  h1 i { color: #6d6a6b; }
</style>


3. Menambahkan Inline CSS

Menambahkan atribut style langsung pada tag HTML tertentu untuk memberikan gaya spesifik pada satu baris elemen.

Contoh: <p style="text-align: center; color: #ccd8e4;">

4. Membuat CSS Eksternal (style_eksternal.css)

Membuat file CSS terpisah untuk mengatur elemen navigasi secara global dan menyisipkannya menggunakan tag <link> di dalam bagian <head> HTML.

Kode Utama:

nav { background: #20A759; color: #fff; padding: 10px; }
nav a { color: #fff; text-decoration: none; padding: 10px 20px; }
nav .active, nav a:hover { background: #0B6B3A; }


5. Menambahkan CSS Selector (ID & Class Selector)

Menggunakan ID Selector (#intro) dan Class Selector (.button, .btn-primary) untuk menargetkan elemen secara spesifik pada halaman web.

ID Selector: Diawali dengan tanda # (unik untuk satu elemen).

Class Selector: Diawali dengan tanda . (bisa digunakan oleh banyak elemen).

❓ Pertanyaan & Tugas

Eksperimen Properti: Melakukan modifikasi properti dan nilai CSS sesuai dengan referensi CSS Cheat Sheet.

Perbedaan h1 {...} dengan #intro h1 {...}:

h1 {...} adalah Element Selector yang akan menerapkan gaya ke seluruh tag h1 di dalam dokumen HTML.

#intro h1 {...} adalah Descendant Selector (kombinasi ID dan Element) yang hanya akan menargetkan tag h1 yang berada di dalam elemen dengan id="intro".

Prioritas Penulisan CSS (Internal vs Eksternal vs Inline):

Inline CSS memiliki prioritas tertinggi dibandingkan Internal dan Eksternal CSS karena ditulis langsung pada tag elemen tersebut (Cascading Order).

Prioritas ID Selector vs Class Selector:

Jika sebuah elemen memiliki ID dan Class secara bersamaan dengan properti yang sama, ID Selector akan lebih diprioritaskan oleh browser dibandingkan Class Selector karena tingkat spesifisitas (specificity) ID lebih tinggi.

