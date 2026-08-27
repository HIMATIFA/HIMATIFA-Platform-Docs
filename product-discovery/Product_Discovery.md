# Product Discovery

# Himatifa Platform

**Website Resmi Himpunan Mahasiswa Informatika (HIMATIFA)**

> **STATUS:** RETROSPECTIVE DISCOVERY BASELINE  
> **Versi:** 1.0  
> **Tanggal:** 28 Agustus 2026  
> **Product Direction:** V1 — Digital Face HIMATIFA

---

## 1. Document Overview

### 1.1 Document Purpose

Dokumen ini merekonstruksi pemahaman produk Himatifa Platform secara retrospektif berdasarkan artefak yang telah tersedia dan informasi baru yang diberikan.

Fokusnya adalah menjelaskan **WHY, WHO, masalah, peluang, keputusan, batasan, dan arah produk**; bukan menggantikan PRD, SRS, UI/UX Specification, atau dokumentasi teknis.

### 1.2 Product Identity

| Item | Value | Status |
|---|---|---|
| Product | Himatifa Platform | CONFIRMED |
| Organization | Himpunan Mahasiswa Informatika (HIMATIFA) | CONFIRMED |
| Initial type | Public organizational website / digital face | CONFIRMED |
| V1 direction | Digital Face HIMATIFA | CONFIRMED |

### 1.3 Retrospective Note

Project sudah berjalan dan PRD dibuat sebelum Product Discovery formal. Karena itu discovery ini tidak mengulang proses dari nol dan tidak membuka kembali keputusan yang sudah jelas.

Requirement **TBD tetap TBD**; peluang baru tidak otomatis menjadi scope V1.

> **SOURCE NOTE**  
> PRD tersedia sebagai sumber utama. SRS dan UI/UX Specification tidak tersedia sebagai file terpisah dalam konteks file yang dapat diakses saat penyusunan ini, sehingga tidak dibuat klaim verifikasi langsung atas isi file tersebut.

---

## 2. Product Context

### 2.1 Background

Himatifa Platform adalah website resmi HIMATIFA. Arahan stakeholder adalah menjaga tahap awal tetap sederhana dan memprioritaskan keberadaan **“wajah digital”** sebelum membangun sistem organisasi yang lebih kompleks.

### 2.2 Current Situation

PRD mencatat potensi fragmentasi representasi digital pada media sosial, pesan instan, dokumen, dan sumber lain.

Dampaknya adalah identitas, profil, struktur, dan aktivitas organisasi lebih sulit ditemukan secara terstruktur.

### 2.3 Why the Product Exists

- Memberikan representasi digital resmi HIMATIFA.
- Memudahkan akses informasi dasar organisasi.
- Menampilkan struktur kepengurusan dan bidang.
- Menampilkan aktivitas, berita, dan dokumentasi jika tersedia.
- Menyediakan kontak dan social media resmi.
- Membangun fondasi yang tidak menghambat pengembangan masa depan.

### 2.4 Stakeholder Context

Arah utama stakeholder/Ketua Himpunan adalah agar tahap awal tidak terlalu kompleks.

Prinsip ini menjadi batas produk:

> Kompleksitas harus berasal dari kebutuhan nyata dan business justification.

---

## 3. Problem Discovery

### 3.1 Confirmed Problems

| Problem | Interpretation | Status |
|---|---|---|
| Representasi digital terfragmentasi | Belum ada satu representasi web resmi yang menjadi wajah digital organisasi. | CONFIRMED |
| Informasi sulit ditemukan terstruktur | Pengunjung membutuhkan titik akses yang jelas. | CONFIRMED |
| Profil/struktur tidak terpusat | Profil, kepengurusan, dan bidang perlu dipahami dari satu website. | CONFIRMED |
| Aktivitas kurang terarsip | Dokumentasi/berita dapat tersebar. | CONFIRMED |
| Pemahaman eksternal tidak cepat | Publik/calon mahasiswa/pihak eksternal dapat kesulitan memahami HIMATIFA. | CONFIRMED |
| Fondasi future content | Struktur informasi yang buruk dapat menyulitkan CMS masa depan. | CONFIRMED |

### 3.2 Problems/Hypotheses Requiring Validation

| Hypothesis | Implication | Status |
|---|---|---|
| Pengurus membutuhkan update konten tanpa developer | Dasar peluang CMS. | POTENTIAL / TBD |
| Ekraf membutuhkan kanal digital lebih terstruktur | Dasar peluang showcase/marketplace. | POTENTIAL |
| Member membutuhkan kanal menawarkan skill | Dasar peluang skill ecosystem. | POTENTIAL |
| External channels memengaruhi continuity konten | Membutuhkan governance content ecosystem. | POTENTIAL |

---

## 4. Opportunity Discovery

| Opportunity | Description | Classification |
|---|---|---|
| Digital Presence | Website sebagai representasi resmi HIMATIFA. | CONFIRMED |
| Information Hub | Berkembang dari digital face menjadi pusat informasi. | FUTURE / POTENTIAL |
| Content Ecosystem | Menghubungkan website dengan sumber eksternal/social media. | POTENTIAL |
| Future CMS | Pengurus dapat mengelola konten bila kebutuhan nyata. | FUTURE |
| Ekraf Showcase/Marketplace | Produk/jasa Ekraf dapat memperoleh kanal digital. | POTENTIAL / FUTURE |
| Member Skill Ecosystem | Fotografi, coding, desain, video editing, dan skill lain berpotensi ditawarkan. | POTENTIAL / FUTURE |

Ekraf saat ini mencakup akun premium, berbagai service, jasa aplikasi, dan layanan lain.

Namun, **marketplace, transaksi, payment, order, komisi, review, membership, dan model bisnis belum ditetapkan.**

---

## 5. Target Users

| User Role | Need | Status |
|---|---|---|
| Mahasiswa Informatika | Mengenal HIMATIFA, struktur, bidang, aktivitas, kontak, social media. | CONFIRMED |
| Publik/External | Memahami identitas, fokus, struktur, aktivitas, kontak. | CONFIRMED |
| Pengurus HIMATIFA | Menjaga representasi dan konten; future dapat mengelola. | CONFIRMED / FUTURE |
| Alumni | Melihat perkembangan, dokumentasi, aktivitas generasi baru. | FUTURE / TBD |
| Future Administrator | Mengelola konten melalui CMS. | FUTURE / TBD |
| Member/service provider | Menawarkan skill melalui ekosistem. | POTENTIAL / TBD |
| Customer/external client | Menemukan/menggunakan produk/jasa. | POTENTIAL / TBD |

---

## 6. User Needs

### 6.1 Mahasiswa Informatika

- Memahami identitas dan positioning HIMATIFA.
- Menemukan struktur dan bidang.
- Mengikuti informasi/aktivitas.
- Menemukan kanal resmi.

### 6.2 Publik/External

- Mendapat gambaran HIMATIFA dengan cepat.
- Melihat identitas dan informasi resmi.
- Memahami struktur/pengelola.
- Menemukan aktivitas, kontak, dan social media.

### 6.3 Pengurus/Content Stakeholder

- Memiliki representasi yang akurat.
- Memiliki struktur informasi yang dapat dipelihara.
- Mendukung transisi pengelolaan masa depan.

> **FUTURE / TBD**  
> Kebutuhan CMS, administrator, role, approval, dan workflow belum ditetapkan.

### 6.4 Future Ekraf, Member, Customer

Ekraf berpotensi membutuhkan kanal produk/jasa; member berpotensi menawarkan skill; customer berpotensi menjadi pengguna layanan.

Semua mekanisme bisnis masih **POTENTIAL/TBD**.

---

## 7. Product Vision

> **CONFIRMED**
>
> “HIMATIFA memiliki wajah digital yang profesional, informatif, mudah diakses, dan dapat dikembangkan menjadi platform organisasi di masa depan.”

### Vision Outcomes

- Representation
- Information
- Credibility
- Foundation

---

## 8. Product Goals

### 8.1 Primary Goals

- Memperkenalkan HIMATIFA.
- Menunjukkan identitas/positioning.
- Menampilkan struktur kepengurusan dan bidang.
- Menampilkan berita/informasi dan dokumentasi.
- Menyediakan kontak dan social media.
- Memberikan pengalaman baik di mobile.
- Menjadi fondasi yang dapat dikembangkan.

### 8.2 Secondary Goals

- Meningkatkan kredibilitas digital.
- Memudahkan pihak eksternal mengenal organisasi.
- Mendokumentasikan aktivitas publik.
- Menjadi awal standardisasi konten digital.

---

## 9. Product Value Proposition

| Audience | Value |
|---|---|
| Mahasiswa | Satu titik akses untuk memahami HIMATIFA dan informasi utamanya. |
| Publik | Representasi digital resmi yang profesional dan mudah dipahami. |
| Pengurus | Media representasi terstruktur dan fondasi future content management. |
| Organisasi | Aset digital resmi yang mendukung kredibilitas dan continuity. |
| Future ecosystem | Fondasi yang dapat diperluas jika kebutuhan terbukti. |

---

## 10. Product Principles

| Principle | Meaning | Status |
|---|---|---|
| Simple First | Fitur karena nilai nyata. | CONFIRMED |
| Professional | Layak sebagai website resmi. | CONFIRMED |
| Maintainable | Mudah dipahami, dirawat, diteruskan. | CONFIRMED |
| Scalable | Bertumbuh bertahap tanpa menghambat future. | CONFIRMED |
| Content-Driven | Nilai berasal dari kualitas konten. | CONFIRMED |
| Mobile-First | Pengalaman mempertimbangkan mobile. | CONFIRMED |
| Accessible | Informasi dapat diakses beragam pengguna/perangkat. | CONFIRMED |
| Secure | Keamanan dasar menjadi bagian desain. | CONFIRMED |
| Easy to Maintain | Mendukung transisi pengelolaan. | CONFIRMED |
| Avoid Unnecessary Complexity | Tidak membangun kompleksitas tanpa justifikasi. | CONFIRMED |

---

## 11. Product Direction

| Stage | Direction | Status |
|---|---|---|
| V1 | Digital Face | CONFIRMED |
| Post-V1 | Information / Content Platform | FUTURE |
| Potential future | Ekraf / Member Skill Ecosystem | POTENTIAL |

> **Catatan:** Future direction bukan commitment implementasi. Setiap capability besar harus divalidasi kembali.

---

## 12. V1 Product Boundary

### 12.1 V1 IS

- Website resmi HIMATIFA.
- Digital face/representasi digital.
- Pusat informasi publik dasar.
- Representasi struktur organisasi.
- Etalase aktivitas.
- Structured content foundation.

### 12.2 V1 IS NOT

- Full organizational management platform.
- Sistem akademik/student information system.
- Sistem administrasi/keuangan.
- Complex membership system.
- Marketplace/transaction platform.
- Operational CMS lengkap.

### 12.3 Feature Boundary

| Capability | V1 | Notes |
|---|---|---|
| Home | Required | Entry point |
| About/Profile | Required | Identitas resmi |
| Organization/Management | Required | Struktur/kepengurusan |
| Division | Required | Bidang/fungsi |
| Contact | Required | Kanal resmi |
| Social Media | Required | Akun resmi |
| News | Phased | Jika konten tersedia dan dapat dipelihara |
| Documentation | Phased | Jika konten tersedia dan dapat dipelihara |
| CMS | Future | Bukan operational V1 |
| Ekraf marketplace | Potential/Future | Business model TBD |
| Member skill marketplace | Potential/Future | Model partisipasi/transaksi TBD |

---

## 13. Future Product Direction

### 13.1 CMS

Potential future capability:

- Content management.
- News/documentation management.
- Organization management.
- Authentication/admin.
- Role/access dasar.
- Publishing workflow jika dibutuhkan.

> **FUTURE / TBD**  
> Detail role, permission, approval, workflow, dan timing belum final.

### 13.2 Ekraf

Peluang digital showcase/marketplace untuk produk/jasa Ekraf.

Belum ditetapkan:

- Siapa seller.
- Verifikasi.
- Transaksi.
- Payment.
- Order.
- Komisi.
- Refund.
- Dispute.
- Review.
- Governance.

**Classification:** POTENTIAL / FUTURE

### 13.3 Member Skill Ecosystem

Anggota berpotensi menawarkan:

- Fotografi.
- Programming.
- Desain.
- Video editing.
- Skill lain.

Bentuk partisipasi belum committed.

---

## 14. Content Ecosystem

### 14.1 Website

Website menjadi representasi resmi dan titik akses informasi terstruktur.

### 14.2 Kompasiana

Sebagian besar berita/berita acara HIMATIFA dipublikasikan melalui Kompasiana HIMATIFA:

`https://www.kompasiana.com/himatifaumsurabaya`

**CONFIRMED NEED**

Kebutuhan produk adalah menghubungkan/mengagregasikan publikasi eksternal bila relevan.

> **TECHNICAL DECISION — NOT PRODUCT DECISION**
>
> Scraping bukan keputusan Product Discovery; tidak tersedianya Public API menjadi konteks technical design.

### 14.3 Social Media

Social media menjadi ekstensi kehadiran digital dan kanal resmi yang diarahkan dari website.

### 14.4 Other External Channels

**POTENTIAL / TBD**

Kanal lain dapat dipertimbangkan jika relevan.

### 14.5 Governance Implication

Ownership, freshness, attribution, dan fallback untuk konten eksternal perlu diputuskan pada fase berikutnya.

---

## 15. Stakeholders

| Stakeholder | Known Role | Decision/Ownership | Status |
|---|---|---|---|
| Ketua Himpunan/leadership | Arahan produk dan scope. | Authority detail TBD. | CONFIRMED / TBD |
| Pengurus HIMATIFA | Penyedia/penjaga informasi. | Content owner detail TBD. | CONFIRMED / TBD |
| Medkom | Penyedia palette/arah visual. | Brand governance detail TBD. | CONFIRMED / TBD |
| Ekraf | Mengelola produk/jasa saat ini. | Digital business model TBD. | CONFIRMED / TBD |
| Solo developer | Pengembangan/maintenance saat ini. | Handover perlu disiapkan. | CONFIRMED |
| Future administrator | Calon pengelola CMS. | Individu/role belum ditetapkan. | FUTURE / TBD |

---

## 16. Organizational Constraints

| Constraint | Implication | Status |
|---|---|---|
| Solo developer | Scope, dokumentasi, maintainability, handover realistis. | CONFIRMED |
| Leadership direction | Tahap awal sederhana/digital face. | CONFIRMED |
| Content ownership | Akurasi bergantung pada pengurus. | CONFIRMED / TBD |
| Leadership transition | Produk harus dapat diteruskan. | CONFIRMED |
| Organizational period | Palette direncanakan sekitar satu periode/tahun. | CONFIRMED |
| Future governance | Ownership jangka panjang belum rinci. | TBD |

### 16.1 Branding Context

Palette dari Medkom:

- `#36a5f4`
- `#002aa7`
- `#ffffff`

Direncanakan sebagai salah satu tema visual untuk satu periode/kurang lebih satu tahun.

Terdapat konsep **Light Mode** dan **Dark Mode**.

> Ini adalah **brand/product context**, bukan technical requirement.

### 16.2 Technology Context

Frontend telah diputuskan menggunakan **Nuxt dan TypeScript**.

Ini dicatat sebagai project context dan tidak menjadi fokus discovery produk.

---

## 17. Assumptions

| Assumption | Status |
|---|---|
| Informasi profil/struktur tersedia untuk V1. | ASSUMPTION |
| Ada pihak berwenang menyetujui informasi. | ASSUMPTION / TBD |
| Media memiliki izin publikasi. | ASSUMPTION |
| Akun social media resmi dapat diidentifikasi. | ASSUMPTION |
| News/documentation tersedia bertahap. | ASSUMPTION |
| Structured content dapat dipelihara tanpa CMS pada V1. | ASSUMPTION |
| Ekraf tetap menjadi aktivitas organisasi. | ASSUMPTION / CONTEXT |

---

## 18. Risks

| Risk | Impact | Response | Status |
|---|---|---|---|
| Scope creep | V1 kompleks/terlambat. | Jaga goal, priority, business value. | CONFIRMED |
| Content availability | Website siap, konten tidak. | Readiness check/content owner. | CONFIRMED |
| Decision delay | Brand/struktur/konten tertahan. | Open Questions/decision owner. | CONFIRMED |
| Maintenance | Website usang. | Struktur sederhana + future CMS. | CONFIRMED |
| Inaccurate information | Kredibilitas turun. | Sumber resmi + update process. | CONFIRMED |
| Solo developer dependency | Knowledge loss. | Dokumentasi/handover. | CONFIRMED |
| Organizational transition | Owner/struktur berubah. | Governance/handover. | CONFIRMED |
| Future complexity | CMS/Ekraf berkembang tanpa dasar. | Discovery ulang sebelum fitur besar. | CONFIRMED |
| External content dependency | Sumber berubah/tidak tersedia. | Ownership/fallback. | POTENTIAL |
| Ekraf business ambiguity | Marketplace prematur. | Validasi business model. | POTENTIAL |

---

## 19. Success Criteria

### 19.1 Product Success

- Website resmi berfungsi sebagai representasi digital.
- Pengunjung memahami identitas.
- Struktur mudah ditemukan.
- Informasi utama mudah diakses.
- Aktivitas dapat ditampilkan.
- Kontak/social media mudah ditemukan.

### 19.2 Experience Success

- Baik digunakan di mobile.
- Navigasi mudah dipahami.
- Langkah menuju informasi utama minimal.
- Konsisten dengan identitas HIMATIFA.

### 19.3 Maintainability Success

- Perubahan informasi dasar tidak memerlukan perubahan arsitektur keseluruhan.
- Konten memiliki struktur jelas.
- Developer berikutnya memahami produk.
- Future CMS tidak memerlukan pembongkaran total V1.

### Bukan Primary Metric

Bukan primary metric:

- Jumlah animasi.
- Jumlah halaman.
- Jumlah library.
- Kompleksitas arsitektur.
- Jumlah fitur.
- Jumlah komponen UI.
- Vanity metrics.

---

## 20. Open Questions

| Area | Question | Status |
|---|---|---|
| Ekraf | Showcase saja, marketplace, atau bentuk lain? | OPEN QUESTION |
| Marketplace | Apa scope dan kategori layanan? | OPEN QUESTION |
| Member participation | Siapa yang dapat menawarkan skill? | OPEN QUESTION |
| Payment | Di platform atau eksternal? | OPEN QUESTION |
| Order flow | Apakah ada request/order dan siapa owner? | OPEN QUESTION |
| Commission | Apakah ada komisi/revenue sharing? | OPEN QUESTION |
| Content ownership | Siapa owner tiap tipe konten? | OPEN QUESTION |
| CMS timing | Kapan kebutuhan CMS dianggap nyata? | OPEN QUESTION |
| CMS governance | Siapa admin dan approval? | OPEN QUESTION |
| Domain | Siapa pemilik dan bagaimana transfer? | OPEN QUESTION |
| Hosting | Siapa owner/penanggung jawab biaya? | OPEN QUESTION |
| Leadership transition | Bagaimana handover antarperiode? | OPEN QUESTION |
| External integration | Kanal mana yang perlu diintegrasikan? | OPEN QUESTION |
| Kompasiana policy | Attribution, freshness, fallback, dan penggunaan publikasi? | OPEN QUESTION |
| Brand | Apakah palette menjadi guideline resmi periode? | PENDING DECISION |
| Light/Dark | Apakah keduanya wajib pada release saat ini? | PENDING DECISION |
| Alumni | Apakah ada kebutuhan khusus pasca-V1? | FUTURE / TBD |

---

## 21. Product Decisions

### 21.1 Confirmed

- Himatifa Platform adalah website resmi HIMATIFA.
- V1 berfokus pada digital face/public website.
- V1 sederhana dan profesional.
- Home, About/Profile, Organization, Division, Contact, Social Media adalah baseline.
- News/Documentation phased sesuai content readiness.
- CMS bukan operational V1.
- Complex academic, membership, payment, chat, native app, dan kompleksitas tanpa business justification di luar V1.
- Structured content foundation dipertahankan.
- Nuxt + TypeScript telah dipilih untuk frontend.
- Palette `#36a5f4/#002aa7/#ffffff` diberikan Medkom sebagai arah visual periode.

### 21.2 Pending Decisions

- Content/decision owner formal.
- Domain/hosting ownership dan handover.
- Governance antarperiode.
- Status final Light/Dark Mode.
- Detail hubungan website dengan Kompasiana.

### 21.3 Future Decisions

- CMS scope/timing.
- Authentication/admin/role/permission/publishing workflow.
- Ekraf business model.
- Member skill ecosystem.
- Payment/order/commission/review/dispute jika marketplace dibutuhkan.
- Alumni dan internal organization services.

---

## 22. Discovery Conclusion

Himatifa Platform bukan proyek untuk mendigitalisasi seluruh organisasi sekaligus.

Produk dimulai sebagai aset digital resmi yang sederhana, profesional, informatif, dan mudah diakses.

Nilai V1 terutama berada pada **representasi dan kualitas konten**, bukan jumlah fitur atau kecanggihan teknis.

Peluang masa depan yang paling jelas adalah **CMS serta ekosistem Ekraf/member skill**. Keduanya belum menjadi commitment V1 karena business model, governance, dan operational requirements belum final.

**Baseline saat ini: V1 tetap digital face; future platform berkembang hanya setelah kebutuhan baru tervalidasi.**

---

## 23. Recommended Next Steps

1. Validasi discovery retrospektif ini bersama stakeholder utama.
2. Tetapkan content owner dan decision owner.
3. Lakukan consistency review Discovery ↔ PRD ↔ SRS ↔ UI/UX.
4. Jika ada perubahan produk nyata, revisi PRD secara terkontrol.
5. Gunakan SRS sebagai baseline software requirement dan SDS untuk technical design.
6. Jangan melakukan rebuild hanya karena discovery dibuat belakangan.
7. Selesaikan V1 digital face sebelum mengevaluasi CMS/Ekraf marketplace.
8. Setelah V1 digunakan, lakukan discovery lanjutan berbasis kebutuhan aktual.
9. Jika Ekraf dikembangkan, lakukan discovery bisnis terpisah sebelum requirement teknis.

---

# 24. Discovery → PRD Alignment

## 24.1 PRD Decisions Supported

| PRD Decision | Discovery Evidence | Assessment |
|---|---|---|
| V1 Digital Face | Problem utama adalah representasi dan akses informasi. | SUPPORTED |
| Simple First | Solo developer + leadership direction. | SUPPORTED |
| Core public pages | Selaras kebutuhan pengguna memahami organisasi. | SUPPORTED |
| News/Documentation phased | Content availability adalah dependency. | SUPPORTED |
| CMS future | Governance/operational need belum final. | SUPPORTED |
| Structured content foundation | Dibutuhkan continuity/future. | SUPPORTED |
| Out of scope complex systems | Tidak ada business need V1. | SUPPORTED |

## 24.2 PRD Areas That May Need Review

| Area | Potential Review | Status |
|---|---|---|
| Stakeholders/governance | Perjelas content/decision owner. | PENDING REVIEW |
| Content ecosystem | Tambahkan Kompasiana sebagai context jika stakeholder menyetujui. | PENDING REVIEW |
| Future direction | Tambahkan Ekraf/member skill sebagai Potential/Future. | PENDING REVIEW |
| Brand context | Catat palette dan Light/Dark concept jika belum ada. | PENDING REVIEW |

## 24.3 Existing PRD Requirements That Remain Valid

Product vision, goals, principles, users, feature priority, V1 boundary, out-of-scope, success metrics, risks, assumptions, CMS future direction, user journey, information architecture, dan release boundary tetap konsisten dengan discovery retrospektif ini.

## 24.4 New Discoveries Affecting Future Versions

- Aktivitas produk/jasa Ekraf.
- Peluang member skill ecosystem.
- Kompasiana sebagai sumber publikasi eksternal utama.
- Kebutuhan governance content ecosystem.
- Palette periode dan konsep Light/Dark.

## 24.5 Does V1 Scope Need to Change?

> **RECOMMENDATION: NO**

Informasi baru tidak memberikan alasan kuat untuk memperluas V1.

Ekraf, marketplace, member services, CMS, dan integrasi eksternal tetap **Future/Potential/TBD**.

---

# 25. Consistency & Classification Check

| Check | Result | Status |
|---|---|---|
| Tujuan produk tetap digital face. | Tidak berubah. | PASS |
| V1 tidak diperluas karena Ekraf. | Dipisahkan Future/Potential. | PASS |
| CMS tetap Future. | Tidak menjadi operational requirement. | PASS |
| News/Documentation phased. | Conditional berdasarkan konten. | PASS |
| TBD tetap TBD. | Tidak diperlakukan final. | PASS |
| Technical solution tidak jadi product requirement. | Nuxt/TS context; scraping bukan decision. | PASS |
| Tidak ada schema/API/architecture prescription. | Tidak disertakan. | PASS |
| Out of scope terkunci. | Dipertahankan. | PASS |
| Discovery tidak menggantikan PRD. | Fokus why/who + alignment. | PASS |

---

# 26. Document Relationship

| Document | Question | Role |
|---|---|---|
| Product Discovery | Why & Who? | Masalah, peluang, user, value, direction. |
| PRD | What? | Product requirements, scope, goals. |
| SRS | What must software satisfy? | Software requirements. |
| UI/UX Specification | How experience/interface structured? | Presentation, interaction, responsive/accessibility. |
| Technical Documentation | How built? | Technology, architecture, implementation. |

---

# 27. Appendix — Classification Legend

| Classification | Meaning |
|---|---|
| **CONFIRMED** | Sudah diputuskan/didukung jelas oleh sumber. |
| **PENDING DECISION** | Perlu keputusan stakeholder. |
| **TBD** | Belum ditentukan; bukan final requirement. |
| **FUTURE** | Sengaja di luar V1. |
| **POTENTIAL** | Peluang belum menjadi commitment. |
| **OPEN QUESTION** | Pertanyaan bisnis/produk yang perlu dijawab. |

---

# 28. Source Notes

**Sumber utama:** `Himatifa_Platform_PRD_v1.0.docx`, status Draft Baseline, tanggal 22 Agustus 2026.

PRD menetapkan V1 sebagai **Public Organizational Website + Structured Content Foundation** dan memisahkan CMS serta kemampuan kompleks ke Post-V1/Future.

### Input Baru yang Digunakan

- Ekraf dan peluang member skill ecosystem.
- Hubungan publikasi dengan Kompasiana.
- Palette Medkom:
  - `#36a5f4`
  - `#002aa7`
  - `#ffffff`
- Konsep Light/Dark Mode.
- Konteks frontend Nuxt + TypeScript.

### Catatan Keterbatasan Sumber

File SRS dan UI/UX Specification tidak tersedia sebagai file terpisah dalam konteks ini.

Karena prinsip **non-invention**, tidak ada klaim bahwa isi keduanya telah diverifikasi langsung.
