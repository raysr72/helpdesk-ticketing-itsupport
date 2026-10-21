# Helpdesk Ticketing IT Support System

Dokumentasi dari perancangan sistem manajemen kendala IT digital yang mentransformasikan proses manual menjadi arsitektur aplikasi web terintegrasi, transparan, dan berbasis metrik kinerja.

## Disclaimer Pivasi

*Catatan:* Repositori ini murni menampilkan dokumentasi perancangan sistem dan analisis bisnis. Seluruh *source code*, konfigurasi server, serta kunci API tidak disematkan untuk mematuhi kebijakan privasi, hak kekayaan intelektual, serta perjanjian kerahasiaan dengan pihak mitra terkait.

## Latar Belakang & Analisis Masalah

- Profil Studi Kasus: Divisi IT Support PT. XYZ Group** merupakan studi kasus nyata penanganan operasional teknologi internal yang memerlukan modernisasi alur kerja layanan bantuan (*IT Helpdesk*).

- Pain Points :

1. **Ketiadaan Pelacakan & Struktur:** Hambatan operasional akibat penggunaan grup pesan WhatsApp yang tidak memiliki arsip riwayat terstruktur dan rentan tidak ter-dokumentasinya laporan masuk.
2. **Transparansi & Monitoring Rendah:** Keterbatasan visibilitas bagi manajer dalam mengaudit durasi penanganan kendala serta memvalidasi kualitas kerja staf.
3. **Akurasi Insentif / KPI:** Kompleksitas perhitungan beban kerja manual yang sering kali menimbulkan ketidaksesuaian pada evaluasi Key Performance Indicator (KPI) bulanan.

## Panduan

Dokumen ini disusun secara sistematis untuk menunjukkan alur kerja dan analisis bisnis menjadi spesifikasi teknis serta perancangan sistem. Dokumen ini dapat ditelusuri melalui urutan alur berikut :

1. Business Requirements Document (BRD): Meninjau batasan ruang lingkup proyek, objektif bisnis, dan alur kerja operasional sistem penanganan insiden IT. [BRD](BRD.md)
2. Functional Requirement Document (FRD): Menilai daftar kebutuhan fungsional (FR) dan parameter non-fungsional (NFR) untuk spesifikasi teknis perangkat lunak. [FRD](FRD.md)
3. Pemodelan Sistem (System Modeling): Mempelajari perancangan alur proses (*Flowchart*), batasan sistem (*Diagram Konteks*), dekomposisi aliran data (*DFD Level 1*), hingga struktur basis data relasional (*ERD*). [System Modeling](system-modeling.md)

## Fitur Utama

- **Tiket Pelaporan Kendala:** Mekanisme pengajuan dan pelacakan status kendala formal yang menggantikan pola pelaporan informal sebelumnya.
- **Live Chat & Monitoring:** Saluran komunikasi terpusat pada tiket untuk memfasilitasi koordinasi cepat antara pelapor dan teknisi.
- **Notifikasi WhatsApp Bot:** Pengiriman pesan pemberitahuan otomatis guna mempercepat arus informasi pembaruan status penanganan kendala.
- **Validasi & Monitoring Poin KPI:** Sistem penilaian objektif berbasis tingkat kesulitan tiket untuk memastikan keadilan insentif staf IT.
- **Manajemen Pengguna:** Pembatasan hak akses berbasis peran (Superadmin, Admin, User) guna menjaga integritas proses validasi dan manajemen data.