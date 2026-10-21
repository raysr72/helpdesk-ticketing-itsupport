# Business Requirement Document (BRD)

## Sistem Helpdesk Ticketing IT Support

---

## Business Background
Pengembangan Sistem Ticketing IT dilatarbelakangi oleh belum terintegrasinya pelaporan kendala IT yang memicu keterlambatan penanganan dan penyelesaian masalah, serta belum adanya mekanisme objektif untuk mengukur kinerja (Key Performance Indicator / KPI) staff IT Support berdasarkan tingkat kompleksitas pekerjaan. Sistem ini dirancang untuk mengotomatisasi alur pelaporan hingga validasi tiket, sekaligus menyelaraskan tingkat kesulitan penanganan masalah dengan perhitungan poin KPI agar efisiensi operasional dan transparansi penilaian kinerja dapat terwujud.

## Problem Statement

- **Proses Pelaporan Kendala:** Pelaporan kendala IT oleh staff pada masing-masing divisi masih dilakukan secara tidak terstruktur (manual melalui grup chat WhatsApp), sehingga berisiko terlambat ditangani atau tidak terdokumentasi dengan baik.
- **Koordinasi dan Komunikasi:** Proses komunikasi antara pelapor, tim IT Support, dan Manajer IT sering kali terhambat akibat tidak tersedianya satu saluran koordinasi terpusat pada setiap tiket.
- **Monitoring Progres Tiket Pelaporan:** Pelapor, Staff IT Support, dan Manajer IT kesulitan memantau status perbaikan kendala IT secara real-time karena belum ada alur pelacakan terintegrasi.
- **Transparansi KPI:** Penilaian kinerja staff IT Support masih kurang objektif dan belum sesuai dengan beban kerja atau kompleksitas kendala yang ditangani akibat tidak tersedianya indikator perhitungan poin yang transparan.

## Project Objectives
- Menyediakan platform terpusat untuk pelaporan kendala IT yang dialami oleh staff dari berbagai divisi.
- Menyediakan saluran komunikasi interaktif (live chat) yang terikat langsung pada setiap tiket kendala guna mempercepat koordinasi.
- Mengotomatisasi pengiriman notifikasi pembaruan progres menggunakan integrasi Bot WhatsApp.
- Meningkatkan akurasi serta transparansi pemberian penilaian KPI untuk Staff IT Support secara objektif berdasarkan tingkat kompleksitas tiket.

## Project Scope

### In-Scope
- **Manajemen Data Pengguna:** Pengelolaan hak akses berbasis peran untuk Superadmin (Manajer IT), Admin (Staff IT Support), dan User (Staff Divisi Lain).
- **Manajemen Data Master:** Pengelolaan kategori tiket berdasarkan tingkat kompleksitas, data divisi, dan data master pengguna.
- **Manajemen Siklus Tiket & Komunikasi:** Pembuatan, klaim tugas dengan mekanisme database locking, pembaruan status seperti In-Progress, Pending, Resolved, Closed, serta fasilitas live chat real-time.
- **Automasi Notifikasi WhatsApp Bot:** Automasi pengiriman notifikasi pembaruan kendala via Bot WhatsApp.
- **Pelaporan & Audit:** Rekapitulasi laporan KPI staff IT, log aktivitas tiket, serta riwayat pesan chat log.

### Out-of-Scope
- Integrasi perangkat keras pemantauan server eksternal secara mandiri di luar pelaporan manual sistem.
- Penilaian KPI untuk divisi di luar IT Support.

## Business Process Flow

- **Proses Saat Ini (As-Is):**
Pelaporan kendala, validasi penanganan, dan komunikasi antara staff IT dengan divisi terkait masih dilakukan secara manual melalui aplikasi pesan instan grup (WhatsApp Group), sehingga rentan terlewat dan tidak memiliki rekam jejak audit yang terstruktur.
- **Proses Usulan (To-Be):** Seluruh alur pelaporan kendala, pelacakan status secara real-time, komunikasi live chat terpusat, validasi akhir manajer, hingga kalkulasi poin KPI dilakukan secara terpusat dan terotomatisasi melalui Sistem Helpdesk Ticketing.