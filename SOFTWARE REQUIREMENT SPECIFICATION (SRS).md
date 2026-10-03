# SOFTWARE REQUIREMENT SPECIFICATION (SRS)

## 1. UI/UX Design Guidelines

Desain antarmuka mengusung estetika minimalis, memastikan navigasi yang intuitif, fokus pada tipografi bersih, dan meminimalisir distraksi visual.

### 1.1. Palet Warna

**Brand & Background**
* <span style="background-color:#0F172A; width:14px; height:14px; display:inline-block; border-radius:3px; border:1px solid #ccc; vertical-align:middle;"></span> **Primary (Brand):** `#0F172A` (Slate 900) - Memberikan kesan profesional, kokoh, dan modern khas keilmuan informatika.
* <span style="background-color:#3B82F6; width:14px; height:14px; display:inline-block; border-radius:3px; border:1px solid #ccc; vertical-align:middle;"></span> **Secondary (Accent):** `#3B82F6` (Blue 500) - Digunakan untuk tombol utama (Call-to-Action), tautan, dan indikator aktivitas.
* <span style="background-color:#FAFAFA; width:14px; height:14px; display:inline-block; border-radius:3px; border:1px solid #ccc; vertical-align:middle;"></span> **Background (Light Mode):** `#FAFAFA` (Neutral 50) - Latar belakang utama untuk menjaga kontras teks tinggi dan *white space* luas.
* <span style="background-color:#020617; width:14px; height:14px; display:inline-block; border-radius:3px; border:1px solid #ccc; vertical-align:middle;"></span> **Background (Dark Mode):** `#020617` (Slate 950) - Latar belakang gelap pekat untuk kenyamanan visual (teks bernuansa `#F8FAFC`).

**Semantic Colors**
* <span style="background-color:#10B981; width:14px; height:14px; display:inline-block; border-radius:3px; border:1px solid #ccc; vertical-align:middle;"></span> **Success:** `#10B981` (Emerald 500) - Status pesanan berhasil, notifikasi simpan.
* <span style="background-color:#F59E0B; width:14px; height:14px; display:inline-block; border-radius:3px; border:1px solid #ccc; vertical-align:middle;"></span> **Warning:** `#F59E0B` (Amber 500) - Stok menipis, peringatan aksi.
* <span style="background-color:#EF4444; width:14px; height:14px; display:inline-block; border-radius:3px; border:1px solid #ccc; vertical-align:middle;"></span> **Destructive:** `#EF4444` (Red 500) - Hapus data, pembatalan pesanan, error.

### 1.2. Tipografi

**Font Family:** Inter atau Geist (Sans-serif)

| Hierarki | Ukuran | Bobot (Weight) | Keterangan Tambahan |
| :--- | :--- | :--- | :--- |
| **Heading 1 (H1)** | 36px | 700 (Bold) | Tracking: Tighter |
| **Heading 2 (H2)** | 24px | 600 (Semibold) | - |
| **Body Text** | 16px | 400 (Regular) | Line-height: 1.5 |
| **Small/Caption** | 14px | Normal | Text-muted |

### 1.3. Komponen Visual & Interaksi (shadcn/ui)

* **Borders & Radius:** Menggunakan radius sudut medium (`rounded-md` atau 8px) pada kartu (*cards*), modal, dan tombol untuk kesan tegas namun ramah.
* **Shadows:** Bayangan sangat halus (`shadow-sm` hingga `shadow-md`) untuk membedakan elemen yang melayang (dropdown, modal) tanpa merusak konsep minimalis.
* **Form & Input:** Input field dengan border tipis (1px) yang berubah warna (`ring-accent`) saat dalam status *focus*. Form disertai validasi *real-time*.
* **Feedback:** Toast notifications diletakkan di sudut kanan bawah untuk setiap aksi CRUD (Create, Update, Delete).

---

## 2. Spesifikasi Fungsional

| Modul | Kebutuhan Sistem (System Shall) | 
| :--- | :--- | 
| **Autentikasi (Auth)** | Memproses login menggunakan kombinasi Email/NIM dan Password. Menerapkan proteksi *rate-limiting* pada form login. | 
| **Public Portal** | Menyediakan CMS statis (SSG) untuk memuat Halaman Berita dan Event dengan FCP (*First Contentful Paint*) < 1 detik. | 
| **Layanan Akademik** | Menampilkan struktur folder hierarkis (Semester > Mata Kuliah > Jenis Dokumen) yang dapat diunduh oleh pengguna terautentikasi. | 
| **Ekraf Store (Shop)** | Mengelola keranjang sesi (*Session Cart*), menghitung subtotal secara otomatis, dan menyediakan integrasi bukti transfer pada form *Checkout*. | 
| **Order Management** | Menyediakan perubahan status pesanan linear: `Pending` &rarr; `Paid` &rarr; `Processed` &rarr; `Shipped/Ready` &rarr; `Completed`. | 
| **Keuangan (Bendum)** | Menjumlahkan total arus kas bulanan secara dinamis dan menyediakan tombol *Export to CSV/PDF* untuk pelaporan rekapitulasi. | 
