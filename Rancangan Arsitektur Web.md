# RANCANGAN ARSITEKTUR WEB

Dokumen ini memuat struktur direktori dan rute (*routing*) aplikasi berdasarkan pola App Router (Next.js). Pengelompokan menggunakan *Route Groups* (folder dalam kurung) agar tata letak (*layout*) dan middleware dapat dikelola secara modular.

## 1. Front-End / Portal Publik
**Catatan Direktori:** Seluruh halaman ini diletakkan di dalam folder `app/(public)/`. Tujuannya agar dapat menggunakan satu `layout.tsx` khusus yang memuat Navbar dan Footer publik.

| Path / Direktori | Nama Halaman | Fungsi & Fitur |
| :--- | :--- | :--- |
| `app/(public)/about/page.tsx` | Profil Himpunan | Memuat sejarah HIMATIFA, visi-misi, makna logo, dan bagan struktur organisasi (BPH, Departemen, KSP). Berfungsi sebagai *company profile* untuk *branding* eksternal. |
| `app/(public)/events/page.tsx` | Katalog Event & Proker | Menampilkan kalender program kerja (Infotech, LKMM, Webinar). Dilengkapi filter kategori, pencarian, dan label status (Pendaftaran Buka/Tutup). |
| `app/(public)/events/[id]/page.tsx` | Detail Event & Registrasi | Halaman spesifik per acara. Berisi *rundown*, profil pemateri, *pricing* tiket, dan form pendaftaran interaktif dengan fitur unggah KTP/KTM serta bukti bayar. |
| `app/(public)/news/page.tsx` | Warta Informatika (Blog) | Pusat publikasi *press release* pasca-acara, berita himpunan, atau artikel opini teknologi buatan mahasiswa. |
| `app/(public)/contact/page.tsx` | Kontak & Kemitraan | Memuat *embed* Google Maps lokasi sekretariat, tautan media sosial resmi, dan form kontak khusus untuk pengajuan *sponsorship* atau kerja sama eksternal. |

## 2. Layanan Khusus Mahasiswa
**Catatan Direktori:** Diletakkan di dalam folder `app/(layanan)/`.

| Path / Direktori | Nama Halaman | Fungsi & Fitur |
| :--- | :--- | :--- |
| `app/(layanan)/akademik/page.tsx` | Portal Akademik (Bank Materi) | Repositori digital untuk mengunduh modul praktikum, *slide* materi (opsional), dan bank soal UTS/UAS per semester. |
| `app/(layanan)/aspirasi/page.tsx` | Kotak Suara Mahasiswa | Form penampung kritik, saran, atau keluhan. Wajib ada fitur *toggle* "Kirim secara Anonim" agar mahasiswa lebih nyaman menyampaikan pendapat. |
| `app/(layanan)/showcase/page.tsx` | Galeri Karya (Showcase) | Etalase portofolio untuk memamerkan *project* terbaik anak Informatika (IoT, *web/app development*, *machine learning*). Cocok untuk pameran digital akreditasi. |

## 3. Ekosistem Ekraf Store (E-Commerce)
**Catatan Direktori:** Digabungkan ke dalam folder `app/(shop)/`.

| Path / Direktori | Nama Halaman | Fungsi & Fitur |
| :--- | :--- | :--- |
| `app/(shop)/ekrafstore/cart/page.tsx` | Keranjang Belanja | Menampung *merchandise* yang dipilih, penyesuaian jumlah pesanan (kuantitas), dan kalkulasi estimasi total harga. |
| `app/(shop)/ekrafstore/checkout/page.tsx` | Checkout & Pembayaran | Form data pembeli (Nama, NIM, No. WA), pemilihan metode pengambilan (Ambil di Sekre / COD area kampus), dan form unggah bukti transfer. |
| `app/(shop)/ekrafstore/orders/[id]/page.tsx`| Lacak Status Pesanan | Halaman pelacakan *real-time* untuk pembeli dengan indikator status (*Menunggu Konfirmasi* → *Diproses* → *Siap Diambil* → *Selesai*). |

## 4. Autentikasi & Keamanan Sistem
**Catatan Direktori:** Diletakkan di dalam folder `app/(auth)/`.

| Path / Direktori | Nama Halaman | Fungsi & Fitur |
| :--- | :--- | :--- |
| `app/(auth)/login/page.tsx` | Gerbang Login Terpusat | Satu halaman *login* untuk semua peran. Menerapkan *Role-Based Access Control* (RBAC) di *backend* (Supabase/API), sehingga setelah berhasil *login*, sistem otomatis mengarahkan *user* ke *dashboard* yang sesuai. |

## 5. Manajemen Internal (Dashboard Pengurus)
**Catatan Direktori:** Dipindahkan ke dalam `app/(dashboard)/` agar mudah diamankan/dikunci menggunakan satu `middleware.ts`.

| Path / Direktori | Nama Halaman | Fungsi & Fitur |
| :--- | :--- | :--- |
| `app/(dashboard)/admin/inventory/page.tsx` | Sistem Manajemen Inventaris| Modul pencatatan peminjaman barang sekretariat (kabel *roll*, proyektor, *sound system*). Berisi log siapa yang meminjam dan tenggat waktu pengembalian. |
| `app/(dashboard)/admin/sertifikat/page.tsx`| Generator & Validasi Sertifikat | Halaman khusus untuk *generate* ID unik sertifikat kepanitiaan/peserta, sekaligus sistem validasi jika ada pihak luar yang melakukan *scan* QR Code dari sertifikat tersebut. |

## 6. System & Error Handling
**Catatan Direktori:** Ditempatkan langsung di *root folder* `app/`.

| Path / Direktori | Nama Halaman | Fungsi & Fitur |
| :--- | :--- | :--- |
| `app/not-found.tsx` | 404 Custom Page | Tampilan khusus jika pengunjung mengakses *route* yang tidak ada. Desain bernuansa *programmer* (misalnya layar terminal atau pesan *error compile*) agar sesuai *branding* jurusan. |
| `app/error.tsx` | Error Boundary | Menangkap *crash* pada aplikasi (baik *client* maupun *server*) agar layar tidak *blank* putih. Dilengkapi tombol "Coba Lagi" (*Try Again*) untuk mereset *state* halaman. |
