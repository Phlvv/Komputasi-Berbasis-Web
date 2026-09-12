# Audit Modul 2 Semantic HTML dan Formulir

## Sebelum perbaikan
| Temuan | Halaman/elemen | Bukti | Rencana perbaikan |
|---|---|---|---|
| Katalog masih berupa ul/li | peralatan.html | DOM | Ubah menjadi section + article |
| Form belum tersedia | peminjaman.html | file baru | Buat form lengkap |

## Setelah perbaikan
- [x] Landmark halaman masuk akal.
- [x] Hierarki heading logis.
- [x] Minimal tiga item katalog lengkap.
- [x] Label dapat diklik dan fokus berpindah.
- [x] Field penting memiliki name.
- [x] Submit kosong memunculkan validasi browser.
- [x] Urutan Tab logis.
- [x] Validator tidak menampilkan error utama.

## Analisis Katalog: `article` vs `table` (Challenge Advanced)
Penggunaan elemen `<article>` lebih tepat digunakan untuk katalog peralatan SIPERALAB karena setiap item memiliki entitas mandiri yang kaya akan konten visual (seperti gambar, deskripsi, stok, dan kondisi). Struktur ini fleksibel dan mudah diadaptasi menjadi tata letak kartu (*card layout*) pada tampilan responsif. Sebaliknya, elemen `<table>` lebih cocok digunakan jika fokus utama data adalah perbandingan matriks antar variabel secara tabular (seperti perbandingan baris kolom spesifikasi teknis). Dalam kasus katalog SIPERALAB, `<article>` memberikan hierarki dokumen semantik yang lebih baik untuk pembaca layar dibanding tabel.
