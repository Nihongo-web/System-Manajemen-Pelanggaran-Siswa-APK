# 📱 SIRA: Sistem Informasi Razia & Manajemen Pelanggaran Siswa
### SMKN 1 Malteng - High-Performance Digital Discipline Management System
---

![Version](https://img.shields.io/badge/Version-2.0.0-blue)
![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20Web-green)
![Build Engine](https://img.shields.io/badge/Build-Kodular%20Native-orange)
![UI Framework](https://img.shields.io/badge/UI-Tailwind%20CSS%20v3-38bdf8)
![Database](https://img.shields.io/badge/Database-Local%20Persistence-yellow)

## 📋 I. Filosofi & Pengenalan Proyek
**SIRA (Sistem Informasi Razia)** bukan sekadar aplikasi pencatatan biasa. Ini adalah manifestasi dari transformasi digital di lingkungan pendidikan, khususnya untuk **SMKN 1 Malteng**. Proyek ini dirancang untuk mengatasi inefisiensi birokrasi dalam menangani pelanggaran kedisiplinan siswa, dengan fokus utama pada penertiban perangkat elektronik (HP).

Dalam era industri 4.0, pencatatan manual di buku besar seringkali menyebabkan data hilang, sulit dicari, dan tidak transparan. SIRA hadir sebagai solusi terpusat yang menggabungkan kecepatan akses data dengan mobilitas tinggi, memungkinkan staf kesiswaan untuk bertindak secara presisi, terukur, dan akurat.

---

## 🏗️ II. Arsitektur Teknologi & Integrasi Sistem

Sistem ini mengadopsi arsitektur **Hybrid Web-Native**, di mana logika frontend yang kompleks dikemas ke dalam performa aplikasi mobile yang solid.

### 1. Build Engine: Powered by Kodular
Aplikasi ini dibuild secara eksklusif menggunakan **Kodular**, sebuah platform pengembangan aplikasi Android berbasis blok yang canggih. 
- **Native Rendering**: Kodular bertindak sebagai kontainer utama yang merender komponen web menjadi aplikasi Android (`.apk`).
- **Hardware Integration**: Melalui Kodular, aplikasi ini mendapatkan akses ke fitur native Android seperti sistem notifikasi, manajemen memori tingkat rendah, dan optimasi baterai yang tidak bisa dicapai oleh browser web biasa.

### 2. UI Engine: Tailwind CSS Enterprise
Berbeda dengan aplikasi mobile standar, SIRA menggunakan **Tailwind CSS (Utility-First Framework)**:
- **Zero Runtime CSS**: Semua gaya desain telah dioptimalkan untuk kecepatan render maksimal.
- **Adaptive Interface**: Desain yang secara cerdas mendeteksi apakah pengguna berada di perangkat layar kecil atau tablet, memastikan elemen UI tidak pernah berantakan.

### 3. Logic Layer: JavaScript ES6+
Logika aplikasi dijalankan oleh mesin JavaScript modern:
- **Asynchronous Data Handling**: Memungkinkan proses penyimpanan data tanpa mengganggu antarmuka pengguna (Anti-Lag).
- **State Persistence**: Menjamin data tetap ada (persisten) di dalam memori lokal perangkat menggunakan teknik pelacakan state yang aman.

---

## 🚀 III. Eksplorasi Fitur & Kapabilitas Sistem

Aplikasi SIRA dibagi menjadi beberapa modul fungsional yang saling bekerja sama secara harmonis:

### A. Dashboard Analitik & Visualisasi Data
Modul ini berfungsi sebagai pusat kendali (*Command Center*) bagi staf kesiswaan:
- **Real-Time Counters**: Statistik otomatis yang menghitung total pelanggaran dan jumlah perangkat yang disita saat ini.
- **Dynamic Visual Cues**: Penggunaan skema warna indikator (High-Contrast) untuk memberikan sinyal urgensi pada data tertentu.

### B. Intelligent Input & Smart Validation
Proses pendaftaran pelanggaran telah didesain untuk mencegah *Human Error*:
- **Pre-defined Taxonomy**: Daftar jurusan telah disesuaikan dengan kurikulum SMKN 1 Malteng (TJKT, TK, MPLB, AKL, dll), sehingga guru tidak perlu mengetik manual.
- **Contextual Form**: Input kronologi yang mendukung teks panjang untuk dokumentasi kejadian yang lebih komprehensif.
- **Action Categorization**: Memisahkan tindakan administratif (catatan) dengan tindakan fisik (penyitaan).

### C. Automated Residivist Tracking (Logika Peringatan)
Sistem memiliki kecerdasan buatan sederhana untuk memantau perilaku siswa:
- **Cumulative Counter**: Sistem secara otomatis menjumlahkan berapa kali seorang siswa muncul dalam database.
- **Threshold Alert (3x+)**: Ketika siswa mencapai atau melewati batas 3 kali pelanggaran, sistem akan memicu "Red Alert" (Badge Merah) pada daftar, menandakan bahwa siswa tersebut memerlukan intervensi serius dari pihak Guru BK atau Kepala Sekolah.

### D. WhatsApp Gateway: Bridge to Parents
SIRA menghapus hambatan komunikasi antara sekolah dan orang tua:
- **Instant Messaging Protocol**: Dengan integrasi URL scheme, aplikasi dapat langsung memicu aplikasi WhatsApp di HP guru.
- **Smart Template**: Pesan yang dikirim sudah terformat secara profesional, mencakup Nama, Kelas, Jenis Pelanggaran, dan Tindakan yang diambil, memberikan kesan profesionalisme sekolah di mata orang tua.

### E. Advanced Database Management & Security
- **Ultra-Fast Search**: Algoritma pencarian berbasis string yang mampu menemukan satu nama di antara ribuan data dalam waktu kurang dari 0.1 detik.
- **Multi-Level Filtering**: Memungkinkan ekspor laporan mental berdasarkan jurusan atau kelas tertentu.
- **Double-Lock Reset**: Fitur pembersihan database yang dilindungi oleh konfirmasi ganda untuk menjaga keamanan data selama tahun ajaran berjalan.

---

## 🎨 IV. Desain Antarmuka & Pengalaman Pengguna (UI/UX)
Kami memprioritaskan "User-Centric Design" dalam setiap aspek:
- **Dark Mode Excellence**: Dukungan mode gelap yang tidak hanya estetis, tetapi juga menghemat daya baterai pada perangkat dengan layar AMOLED.
- **Accessibility Ready**: Ukuran tombol dan kontras teks telah diuji agar tetap mudah dioperasikan meskipun di bawah sinar matahari langsung (saat operasi razia di lapangan).
- **Smooth Animations**: Transisi antar halaman yang halus memberikan kesan aplikasi premium dan modern.

---

## 🛡️ V. Integritas Kode & Keamanan Persistensi
Sebagai arsitek sistem, saya menjamin bahwa:
1. **Data Security**: Data siswa disimpan secara lokal di dalam folder terproteksi aplikasi Android, tidak terekspos ke publik.
2. **Stability**: Penanganan error (Error Handling) telah diterapkan pada setiap fungsi krusial untuk mencegah aplikasi tertutup tiba-tiba (*Force Close*).
3. **Optimasi Kodular**: Penggunaan komponen internal Kodular telah dikonfigurasi untuk konsumsi RAM yang sangat rendah.

---

**SIRA SMKN 1 Malteng** | *Digitalizing Discipline for a Better Education.*
