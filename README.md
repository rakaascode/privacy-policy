# Kebijakan Privasi Aplikasi

Pusat kebijakan privasi aplikasi Raka Agi Saputra / MetroLabs, diterbitkan menggunakan GitHub Pages. Setiap aplikasi mempunyai URL sendiri agar kebijakannya dapat diperbarui secara terpisah.

**Halaman utama:** https://rakaascode.github.io/privacy-policy/

| Aplikasi | Kebijakan privasi | Bahasa |
| --- | --- | --- |
| Wifora | https://rakaascode.github.io/privacy-policy/wifora/ | English |

Kebijakan Wifora sebelumnya ditampilkan pada halaman utama. Isi dan tanggal berlaku kebijakan tersebut dipertahankan di `wifora/index.html`. Tautan utama sekarang menampilkan direktori, dengan tautan yang jelas ke Wifora; tautan lama dengan `#section-1` sampai `#section-9` diarahkan ke bagian kebijakan yang sesuai.

## Struktur

```text
index.html                      # Direktori aplikasi
assets/style.css                # Tampilan direktori
wifora/index.html               # Kebijakan Wifora
nama-aplikasi/index.html        # Pola untuk aplikasi mendatang
docs/privacy-policy-template.md # Template draf, bukan kebijakan aktif
.nojekyll                      # Publikasi HTML statis tanpa Jekyll
```

## Menambah aplikasi

1. Buat folder dengan slug huruf kecil dan tanda hubung, misalnya `aplikasi-baru/`.
2. Gunakan `docs/privacy-policy-template.md` sebagai panduan menyiapkan isi berdasarkan perilaku aplikasi. Template ini adalah Markdown draf; jangan menautkannya sebagai kebijakan aplikasi.
3. Buat `aplikasi-baru/index.html` berisi kebijakan lengkap. Sertakan nama aplikasi, tanggal berlaku, kontak, serta tautan kembali ke `../`. Kebijakan Wifora dapat dipakai sebagai referensi struktur HTML; klaim privasinya hanya berlaku untuk Wifora.
4. Tambahkan kartu aplikasi pada `index.html`, tautkan ke `aplikasi-baru/`, lalu perbarui jumlah aplikasi dan tabel README.
5. Commit dan push ke branch `main`. GitHub Pages memublikasikan isi root repository.
6. Periksa halaman yang sudah terbit sebelum memakai URL `https://rakaascode.github.io/privacy-policy/aplikasi-baru/` di aplikasi atau halaman distribusi.

Gunakan URL khusus aplikasi sebagai tautan kebijakan privasi. Pertahankan slug setelah URL digunakan. Tambahkan aplikasi ke daftar hanya setelah kebijakannya siap diterbitkan.

## Preview lokal

Jalankan dari root repository:

```bash
python3 -m http.server 8000
```

Buka http://localhost:8000/ dan http://localhost:8000/wifora/.

## GitHub Pages

Pengaturan: **Settings → Pages → Deploy from a branch → main → / (root)**.

Kontak: metrolabssoftware@gmail.com
