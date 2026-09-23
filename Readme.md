# 📊 NKP Kinerja 2026 - Dashboard Monitoring Hasil Pemeriksaan BPK

Sistem Pemantauan dan Tindak Lanjut Hasil Pemeriksaan BPK (Badan Pemeriksa Keuangan) Kementerian Koordinator Bidang Pangan berbasis web application serverless yang dibangun di atas Google Apps Script dan Google Sheets.

---

## 📸 Fitur Utama

- 🔐 **Autentikasi & Manajemen Sesi:** Multi-role login (Administrator dan Penanggung Jawab / PIC) dengan fitur pemilihan pengguna dinamis.
- 📈 **Dashboard Interaktif & Analytics:** 
  - Ringkasan statistik (Total Temuan Unik, Total Tindak Lanjut, PIC yang telah mengisi, dan Persentase Progress Keseluruhan).
  - Grafik Visualisasi Chart.js (*Bar Chart* Distribusi Tindak Lanjut per PIC & *Doughnut Chart* Status Progress).
  - Kartu Progress per PIC dengan kalkulasi persentase penyelesaian otomatis.
- 📝 **Ruang Isian (CRUD Management):**
  - Penambahan temuan baru dengan pembuatan **Nomor Temuan Otomatis**.
  - Dukungan struktur data bertingkat (**Parent Temuan & Sub-Tindak Lanjut**).
  - Pengeditan dan penghapusan data secara interaktif tanpa reload halaman.
  - Penanda status visual (*Selesai*, *Dalam Proses*, dan *Belum Ditindaklanjuti*).
- 📑 **Rekapitulasi & Pencarian Data:**
  - Penyaringan data berdasarkan PIC dan kata kunci pencarian.
  - Tampilan *accordion* untuk detail rincian temuan.
- 📥 **Ekspor Laporan ke Excel:** Ekspor data laporan lengkap sesuai format standar dinas secara langsung ke format `.xlsx` menggunakan SheetJS.
- 📱 **Desain Modern & Responsive:** UI/UX bergaya dashboard modern (Plus Jakarta Sans, Lucide Icons, Glassmorphism top header, dan Sidebar Overlay untuk perangkat mobile).

---

## 🛠️ Teknologi yang Digunakan

* **Backend / Server-Side:** Google Apps Script (`Code.gs`)
* **Database / Storage:** Google Sheets
* **Frontend / Client-Side:** HTML5, CSS3 (CSS Variables, Flexbox, CSS Grid), JavaScript (ES6+)
* **Pustaka & Asset:**
  * Chart.js (v4.4.0) — Grafik visualisasi data.
  * SheetJS / xlsx (v0.18.5) — Ekspor data ke file Excel.
  * Lucide Icons — Ikon UI responsif.
  * Google Fonts (Plus Jakarta Sans) — Tipografi UI.

---

## 📁 Struktur Repositori

```text
.
├── Code.gs         # Backend Google Apps Script (Logika Database, Login, CRUD)
├── Index.html      # Frontend App Shell (UI/UX, Script Client-side, & Styling)
└── README.md       # Dokumentasi Proyek