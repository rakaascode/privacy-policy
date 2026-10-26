# Aturan pembuatan kebijakan privasi

Aturan ini berlaku untuk seluruh repository dan setiap aplikasi baru. Instruksi pengguna yang lebih baru tetap menjadi acuan utama.

## Bahasa dan isi

- Gunakan bahasa yang ringkas, jelas, dan mudah dipahami. Utamakan kalimat pendek dan istilah sehari-hari.
- Gunakan Bahasa Indonesia secara default. Pertahankan bahasa kebijakan yang sudah ada kecuali pengguna meminta perubahan.
- Gunakan daftar poin untuk beberapa rincian yang sejajar. Gunakan tabel bergaris untuk jenis data dan tujuan penggunaan, atau izin perangkat dan kegunaannya.
- Jelaskan sesuai kebutuhan aplikasi: pengelola dan kontak, data yang diproses, tujuan, penerima data, izin, layanan pihak ketiga, keamanan, retensi, penghapusan, usia pengguna, dan perubahan kebijakan.
- Verifikasi pernyataan terhadap kode, SDK, konfigurasi, serta informasi pengelola. Jangan mengarang penyedia, lama penyimpanan, batas usia, atau kemampuan keamanan.
- Jika fakta belum tersedia, tandai sebagai draf dan nyatakan asumsi secara singkat. Jangan menyajikan usulan sebagai praktik yang sudah diterapkan.
- Jangan mengklaim kepatuhan hukum secara mutlak atau menjamin keamanan tanpa bukti. Untuk persyaratan platform atau hukum yang dibahas, periksa sumber resmi terkini.
- Perubahan tampilan tidak boleh mengubah isi atau tanggal berlaku kebijakan tanpa instruksi yang relevan.

## Tampilan bersama

- Ikuti gaya HTML klasik yang sederhana: latar putih, teks hitam, Times New Roman, dan tautan biru.
- Gunakan CSS bersama di `assets/style.css`; hindari menyalin stylesheet terpisah untuk setiap aplikasi.
- Pertahankan tata letak rata kiri, tanpa batas lebar terpusat, dengan margin horizontal 40px di desktop dan 24px pada layar hingga 520px.
- Pertahankan ukuran dasar 16px dan jarak rapat. Hindari hero besar, kartu, ikon dekoratif, gradien, animasi, serta ruang kosong berlebihan.
- Header aplikasi mengikuti Wifora dan Testerindo: nama aplikasi besar sebagai h1, jenis dokumen sebagai subjudul, deskripsi singkat, lalu tanggal berlaku dan versi. Untuk draf, gunakan tanggal draf dan status; jangan mengarang versi atau tanggal berlaku.
- Gunakan kelas `app-header`, `app-title`, `policy-title`, `app-description`, dan `policy-meta` dari stylesheet bersama.
- Paragraf isi dan poin kebijakan memakai justify. Judul, daftar isi, metadata, tabel, kontak, dan footer tetap rata kiri.
- Jangan tambahkan tautan kembali atau tombol back.
- Jangan tampilkan garis pemisah antarbagian. Pertahankan garis pada tabel serta latar abu-abu sederhana untuk kepala tabel.
- Sediakan daftar isi dengan tautan bagian yang valid untuk dokumen dengan beberapa bagian.
- Semua halaman mempunyai footer konsisten dengan identitas aplikasi/pengelola, kontak, copyright, dan status draf jika relevan. Gunakan identitas serta kontak yang sudah dikonfirmasi; tandai usulan jika belum.

## Struktur dan penerbitan

- Setiap aplikasi memakai folder huruf kecil dengan tanda hubung: `nama-aplikasi/index.html`.
- Pertahankan URL aplikasi yang sudah diterbitkan dan ID bagian yang sudah ditautkan.
- Tambahkan aplikasi ke tabel halaman utama dan README. Tandai draf dengan jelas.
- Setelah mengubah CSS bersama, perbarui parameter `?v=` pada tautan stylesheet seluruh halaman menggunakan hash isi CSS agar cache tidak menahan desain lama.
- Periksa tautan, tampilan ponsel/desktop yang terdampak, dan `git diff --check`. Untuk perubahan tampilan saja, pastikan teks kebijakan tetap utuh.
- Commit dan push sesuai otorisasi pengguna. Bedakan status sudah dipush, build berjalan, dan sudah tayang. Jangan menyatakan sudah tayang sebelum memverifikasi build dan halaman publik.
- Jangan menghapus label draf hanya karena halaman sudah diterbitkan. Jadikan kebijakan resmi setelah fakta dan tanggal berlaku sudah dipastikan.
