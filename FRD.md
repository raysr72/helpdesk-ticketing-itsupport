# Functional Requirement

| ID | MODUL / FITUR | PERILAKU SISTEM |
| :--- | :--- | :--- |
| FR-01 | Autentikasi & Manajemen Pengguna | Sistem menyediakan halaman login terpusat yang memvalidasi *username*, *password*, dan hak akses peran (*Role-Based Access Control* / RBAC) untuk Superadmin/Manajer IT, Admin/Staff IT Support, dan User/Staff Divisi Lain, serta memungkinkan Superadmin mengelola data akun pengguna. |
| FR-02 | Manajemen Data Master | Superadmin dan Admin dapat melakukan operasi CRUD (*Create, Read, Update, Delete*) pada data master yang mencakup: Kategori Tiket (beserta bobot tingkat kompleksitas/kesulitan), Data Divisi, dan Data Master Pengguna. |
| FR-03 | Pembuatan & Pengelolaan Tiket (Ticketing) | User (Staff Divisi lain) dapat membuat laporan kendala baru dengan mengisi formulir lengkap (judul, kategori, deskripsi kendala, divisi, dan lampiran file pendukung), yang kemudian divalidasi, diklaim, dan dikelola statusnya oleh Staff IT Support (*In-Progress, Pending, Resolved, Closed*). |
| FR-04 | Saluran Komunikasi *Real-Time* (Live Chat) | Sistem menyediakan fitur *live chat* terpusat pada setiap halaman detail tiket yang aktif guna memfasilitasi komunikasi dua arah secara *real-time* antara Pelapor dan Staff IT Support yang bertugas. |
| FR-05 | Integrasi Notifikasi WhatsApp Bot | Sistem secara otomatis mengirimkan pesan melalui bot WhatsApp kepada pihak terkait (Pelapor atau Staff IT Support) setiap kali terdapat pembaruan status tiket atau pesan masuk baru. |
| FR-06 | Perhitungan Poin KPI Otomatis | Sistem secara otomatis menghitung dan mencatat perolehan poin KPI bagi Staff IT Support pada *leaderboard* berdasarkan kategori atau tingkat kompleksitas tiket yang berhasil diselesaikan dan divalidasi. |
| FR-07 | Pelaporan & Log Aktivitas (Reporting & Audit) | Sistem menyediakan fitur rekapitulasi laporan KPI staff IT, log aktivitas tiket secara keseluruhan, serta riwayat pesan (*chat log*) untuk keperluan audit Manajer IT. |

# Non-Functional Requirement

| ID | KATEGORI | PARAMETER KEBUTUHAN NON-FUNGSIONAL |
| :--- | :--- | :--- |
| NFR-01 | Usability (Kegunaan) | Antarmuka sistem harus dirancang intuitif dan responsif (*user-friendly*) agar mudah dioperasikan oleh seluruh staf lintas divisi tanpa memerlukan pelatihan teknis tingkat lanjut. |
| NFR-02 | Performance (Performa) | Sistem harus mampu memproses pengiriman pesan *live chat*, pembaruan status tiket, dan kalkulasi poin KPI secara instan (*real-time*) tanpa jeda yang signifikan dalam kondisi jaringan standar. |
| NFR-03 | Security (Keamanan) | Penerapan kontrol akses berbasis peran (*Role-Based Access Control* / RBAC) yang ketat; perlindungan sesi pengguna dan pencegahan akses ke halaman manajemen tanpa autentikasi yang sah.|
| NFR-04 | Reliability & Availability (Keandalan & Ketersediaan) | Basis data harus dirancang terstruktur secara relasional untuk menjamin konsistensi data tiket, riwayat *chat*, relasi lampiran (*attachment*), dan akumulasi poin KPI tanpa risiko duplikasi atau anomali data. |
| NFR-05 | Integration (Integrasi Sistem) | Sistem harus terhubung secara stabil dengan API WhatsApp Gateway/Bot untuk memastikan pengiriman notifikasi *real-time* berjalan lancar dengan mekanisme penanganan kegagalan pengiriman (*retry mechanism*). |