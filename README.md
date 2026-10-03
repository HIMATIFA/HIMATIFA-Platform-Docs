# Platform Web HIMATIFA

Platform digital terpusat yang dirancang untuk mendigitalisasi seluruh alur kerja Himpunan Mahasiswa Informatika (HIMATIFA). Sistem ini bertujuan untuk memangkas birokrasi administratif, meningkatkan transparansi keuangan, mempermudah layanan akademik, dan menyediakan kanal komersialisasi mandiri melalui Ekraf Store.

## Dokumentasi Proyek

Dokumentasi utama proyek ini dibagi menjadi tiga bagian pokok untuk memudahkan pengembangan, pelacakan kebutuhan sistem, dan pembagian tugas antar *developer*:

1. [**Product Requirement Document (PRD)**](./Product_Requirement_Document.md)
   Berisi landasan bisnis produk, visi dan objektif, target pengguna (*roles* & *pain points*), serta *Key Performance Indicators* (KPI) untuk mengukur keberhasilan rilis.

2. [**Software Requirement Specification (SRS)**](./Software_Requirements_Specification.md)
   Berisi spesifikasi teknis dan fungsional dari sistem. Mencakup pedoman UI/UX, palet warna, tipografi, komponen interaksi (*shadcn/ui*), serta matriks spesifikasi fungsional per modul.

3. [**Rancangan Arsitektur Web**](./Rancangan_Arsitektur_Web.md)
   Berisi struktur direktori dan *routing* aplikasi berbasis Next.js (App Router). Mencakup pengelompokan *Route Groups* untuk halaman publik, layanan mahasiswa, ekosistem *e-commerce* (Ekraf Store), autentikasi, *dashboard* pengurus, hingga penanganan *error*.

## Ringkasan Teknologi (Tech Stack)

Berdasarkan spesifikasi dan arsitektur yang telah dirancang, proyek ini dikembangkan menggunakan ekosistem modern berikut:

* **Framework:** Next.js (App Router) dengan kapabilitas SSG (*Static Site Generation*) untuk optimasi performa dan FCP < 1 detik.
* **Styling & UI:** Tailwind CSS (skema warna *Slate*, *Blue*, dll) & komponen UI dari **shadcn/ui**.
* **Typography:** Font keluarga Inter atau Geist (Sans-serif).
* **Database & Auth:** Supabase / API Eksternal terintegrasi (Mendukung perlindungan *rate-limiting* dan *Role-Based Access Control*).

## Hak Akses (Role-Based Access)

Sistem ini mendukung 6 level peran pengguna melalui satu gerbang *login* terpusat:

* **Public / Guest:** Portal informasi (*company profile*, berita, kontak).
* **Mahasiswa:** Repositori akademik, penyampaian aspirasi anonim, dan akses pembelian *merchandise*.
* **Sekretaris Umum:** Manajemen arsip persuratan.
* **Bendahara Umum:** Manajemen kas bulanan dan ekspor laporan.
* **Admin Ekraf:** Manajemen inventaris toko, katalog, dan pelacakan pesanan.
* **Super Admin:** Manajemen hak akses, validasi sertifikat, inventaris BEM, dan log aktivitas.
