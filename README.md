# Document Tracker

Sistem pelacakan dokumen yang dikembangkan berdasarkan 3,5 tahun pengalaman praktis dalam mengelola dan memantau dokumen perusahaan.

## 1. Project Brief

### 1.1 Problem Statement

Kondisi data saat ini memiliki beberapa permasalahan, seperti data yang kotor, tidak lengkap, tidak diperbarui, dan permasalahan lainnya. Hal ini dapat berdampak pada kepatuhan terhadap regulasi serta proses pengambilan keputusan oleh pemangku kepentingan terkait.

Pengguna juga mengalami kesulitan dalam melakukan pelacakan dokumen. Data mentah yang tersedia saat ini belum dapat dijadikan acuan dalam pengambilan keputusan maupun untuk mengawasi dokumen yang berpotensi melanggar regulasi apabila tidak diperbarui.

### 1.2 Tujuan

Membuat tracker SOP yang dapat dijadikan sebagai **Single Source of Truth** yang andal.

### 1.3 Scope

1. Mengumpulkan master data dokumen kebijakan dan SOP.
2. Membuat tracker dokumen.
3. Mengklasifikasikan dokumen berdasarkan tanggal, status, dan prioritas.
4. Membuat *action log* untuk proses pembaruan.
5. Membuat *data dictionary* dan *business rules*.
6. Membuat dashboard ringkas untuk monitoring.
7. Menyusun UAT.

### 1.4 Out of Scope

- Membuat sistem persetujuan otomatis secara penuh.
- Mengintegrasikan sistem secara langsung dengan SharePoint, ERP, atau DMS.
- Mengubah isi SOP asli perusahaan.
- Mengakses dokumen internal yang bersifat rahasia.
- Mengirimkan pengingat otomatis melalui email atau Power Automate.
- Membuat fitur login pengguna dan *role-based access*.
- Melakukan audit hukum atau regulasi secara formal.

### 1.5 Pengguna Utama

Tim yang bertanggung jawab atas tata kelola perusahaan.

### 1.6 Asumsi

1. Setiap dokumen hanya memiliki satu `Document ID` yang unik.
2. Format status yang akan digunakan distandarkan.
3. Siklus peninjauan dokumen dihitung dalam satuan bulan.
4. Setiap dokumen memiliki minimal satu pemilik atau PIC.
5. Proses pembaruan dianggap berlangsung secara berkala, bukan *ad hoc*.
6. Tracker akan digunakan oleh pengguna internal nonteknis yang terbiasa menggunakan Excel atau Google Sheets.

### 1.7 Batasan

1. Solusi awal hanya dibuat menggunakan Excel atau Google Sheets, bukan sistem aplikasi penuh.
2. Tidak terdapat integrasi otomatis dengan email, SharePoint, atau ERP.
3. Waktu pengerjaan portofolio terbatas sehingga solusi harus cukup sederhana untuk dibuat secara mandiri.
4. Tidak terdapat akses ke *enterprise approval workflow*.
5. File harus tetap mudah dibuka dan dipahami oleh recruiter.
6. Solusi harus dapat dijelaskan tanpa melanggar NDA atau kerahasiaan perusahaan.
7. Dashboard harus dibangun dari data yang tersedia, bukan data langsung milik perusahaan.

### 1.8 Manfaat yang Diharapkan

Pemangku kepentingan dapat mengambil keputusan berdasarkan tracker SOP yang telah dirancang.
