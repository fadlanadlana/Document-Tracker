# Document-Tracker
A document tracking system yang dikembangkan berdasarkan 3,5 tahun pengalaman praktis dalam mengelola dan memantau dokumen perusahaan.
**1 Project brief **
1.1 Problem statement 
Kondisi Saat ini tabel memiliki permasalahan berupa isi data yang kotor, tidak lengkap, tidak diperbaharui dan permasalahan lainya. Hal ini dapat berdampak pada kepatuhan terhadap regulasi dan juga pengambilan keputusan oleh pemangku kepentingan yang relevan. Pengguna akan kesulitan juga untuk melakukan tracking dokumen. Saat ini data raw tidak dapat dijadikan acuan untuk membuat keputusan dan tidak bisa mengawasi dokumen yang berpotensi melanggar regulasi jika tidak di Update.
**1.2 tujuan******
Membuat Tracker SOP yang dapat dijadikan sebagai Single Source of Truth yang andal
**1.3 scope **
  1. Mengumpulkan master data dokumen kebijakan/sop
  2. Membuat tracker dokumen
  3. mengklasifikasiakan dokumen sesuai tanggal, status dan prioritas
  4. membuat action log untuk pembaruan proses
  5. membuat datadictionaruy dan business rule
  6. membuat dashboard ringkas untuk monitoring
  7. menyusun UAT
1.4 **out-of-scope** 
Membuat sistem approval otomatis penuh, Integrasi langsung ke SharePoint / ERP / DMS, Mengubah isi SOP asli perusahaan, Mengakses dokumen internal rahasia, Mengirim reminder otomatis via email/Power Automate, Login user dan role-based access, Audit legal/regulatory formal
**1.5 pengguna utama**
Tim yang mengatur Tata Kelola perusahaan
**1.6 asumsi**
  1. Setiap dokumen hanya punya 1 document ID unik.
  2. Format status yang ingin dibangun akan distandarkan.
  3. Review cycle dokumen dianggap dalam hitungan bulan.
  4. Setiap dokumen punya minimal satu owner atau PIC.
  5. Proses renewal dianggap terjadi secara berkala, bukan ad hoc.
  6. Tracker akan dipakai oleh user internal non-teknis yang familiar dengan Excel/Sheets.
**1.7 Batasan**
  1. Solusi awal hanya dibuat di Excel/Google Sheets, bukan sistem aplikasi penuh.
  2. Tidak ada integrasi otomatis ke email, SharePoint, atau ERP.
  3. Waktu pengerjaan portofolio terbatas, jadi solusi harus cukup sederhana untuk dibuat sendiri.
  4. Kamu tidak punya akses ke approval workflow enterprise.
  5. File harus tetap mudah dibuka dan dipahami recruiter.
  6. Solusi harus bisa dijelaskan tanpa melanggar NDA atau kerahasiaan kerja.
  7. Dashboard harus dibangun dari data yang tersedia, bukan data live perusahaan.
**1.8 Manfaat yang diharapkan**
  Pemangaku kepentingan dapat mengabil keputusan berdasarkan tracker SOP yang sudah di rancang 
