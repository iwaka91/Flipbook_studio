# TeGe Flipbook Studio

Mesin pembuat flipbook HTML dari gambar atau PDF, dengan animasi kertas melengkung (*page curl*), efek suara, serta dua format ekspor.

**Versi proyek:** V1.2 — Page Curl Engine

## Jalankan

1. Unduh `index.html` dari repo ini dan buka di browser modern, atau buka langsung jika dihosting.
2. Impor halaman gambar (JPG, PNG, WEBP) atau dokumen PDF.
3. Urutkan halaman, lengkapi judul buku, atur kualitas dan tema, lalu coba pratinjau.
4. Pilih hasil ekspor **HTML tunggal** (semua halaman tertanam) atau **ZIP** (`index.html` + folder `images/`, serta file PDF asli bila dipilih).

Anda dapat mencoba pembaca mandiri pada [contoh flipbook](examples/Contoh_Flipbook_Curl_v1_2.html).

## Fitur

- Pratinjau flipbook responsif desktop dan mobile.
- Animasi page curl / lembar kertas melengkung dengan bayangan dan dukungan tarik halaman.
- Suara lembar dibalik, dapat diaktifkan/dinonaktifkan pembaca.
- Editor urutan halaman dan pengaturan ukuran/kualitas.
- Ekspor HTML tunggal atau paket ZIP yang dapat dibuka secara offline.
- Panel **Tentang** berisi kredit, informasi teknologi, dan identitas pembuat.

## Catatan teknis

- Mesin pembuat dapat dibuka dari file HTML lokal.
- **Impor PDF membutuhkan koneksi internet** untuk memuat PDF.js. Setelah PDF dikonversi menjadi gambar halaman, flipbook hasil ekspor bisa digunakan tanpa internet.
- Page curl memakai Canvas 2D untuk menyimulasikan lengkungan; bukan simulasi fisika 3D sepenuhnya.
- PDF yang dirender menjadi halaman gambar tidak mempertahankan teks yang bisa diseleksi di flipbook.
- HTML tunggal dapat sangat besar bila jumlah halaman banyak; paket ZIP memisahkan aset.

## Kredit dan lisensi

**Pembuat:** Toto Gutomo — Guru SMA Negeri 3 Maliku  
**Website:** https://totogutomo.com

- **Efek suara:** “Page flip (smaller page)” oleh **OxidVideos** dari Pixabay, digunakan sesuai **Pixabay Content License**. Kredit ini tidak menjadikan efek suara berada di bawah lisensi kode aplikasi.
- **PDF.js:** Mozilla Foundation dan kontributor; Apache License 2.0.
- **Kode mesin:** informasi lisensi proyek mengikuti keterangan lisensi dalam panel **Tentang** pada aplikasi. Lisensi aset pihak ketiga tetap berlaku sendiri.

## Struktur repo

```text
Flipbook_studio/
├── index.html
├── README.md
└── examples/
    └── Contoh_Flipbook_Curl_v1_2.html
```

**Status:** fitur ekspor HTML/ZIP, pratinjau, pembalikan halaman, dan tampilan mobile telah diuji; impor PDF asli tetap membutuhkan pengujian lapangan dengan browser yang dapat mengakses PDF.js.
