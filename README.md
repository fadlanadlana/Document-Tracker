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

## 2. Stakeholder Analysis
### 2.1 Stakeholder Mapping
<img width="1423" height="799" alt="image" src="https://github.com/user-attachments/assets/ff7aa8a1-8db6-40a7-93b7-a1cb351e0e5a" />

### 2.2 Stakeholder Engagement

| Stakeholder Role | Quadrant | Engagement Strategy |
|---|---|---|
| Process Excellence Lead | Manage Closely | Workshop, design review, UAT, weekly coordination |
| Operational Risk Manager | Manage Closely | Workshop, design review, UAT, weekly coordination |
| Finance Operations Manager | Manage Closely | Workshop, design review, UAT, weekly coordination |
| HR Operations Manager | Manage Closely | Workshop, design review, UAT, weekly coordination |
| IT Operations Manager | Manage Closely | Workshop, design review, UAT, weekly coordination |
| Procurement Manager | Manage Closely | Workshop, design review, UAT, weekly coordination |
| Financial Control Lead | Manage Closely | Workshop, design review, UAT, weekly coordination |
| Treasury Lead | Manage Closely | Workshop, design review, UAT, weekly coordination |
| People Development Lead | Manage Closely | Workshop, design review, UAT, weekly coordination |
| Enterprise Risk Lead | Manage Closely | Workshop, design review, UAT, weekly coordination |
| Business Continuity Lead | Manage Closely | Workshop, design review, UAT, weekly coordination |
| Corporate Planning Manager | Manage Closely | Workshop, design review, UAT, weekly coordination |
| Service Delivery Lead | Manage Closely | Workshop, design review, UAT, weekly coordination |
| Vendor Management Lead | Manage Closely | Workshop, design review, UAT, weekly coordination |
| Director of Operations | Keep Satisfied | Executive update, consultation on key decisions, milestone review |
| Chief Risk Officer | Keep Satisfied | Executive update, consultation on key decisions, milestone review |
| Division Head | Keep Satisfied | Executive update, consultation on key decisions, milestone review |
| Governance Admin | Keep Informed | User update, training, UAT communication, operational notice |
| PMO Analyst | Keep Informed | User update, training, UAT communication, operational notice |
| Application Support Lead | Keep Informed | User update, training, UAT communication, operational notice |
| HR Policy Lead | Keep Informed | User update, training, UAT communication, operational notice |
| System Migration Team/Lead | Keep Informed | User update, training, UAT communication, operational notice |
| General Employee/User | Monitor | General announcement or low-frequency update |
| Administrative Support dari unit non-pilot | Monitor | General announcement or low-frequency update |
| Observer dari unit di luar scope | Monitor | General announcement or low-frequency update |

### 2.3 RACI Matrix

(TO BE FILLED)

## 3. As-Is Analysis
### 3.1 As-Is diagram 
<img width="9248" height="4328" alt="image" src="https://github.com/user-attachments/assets/1d8c3852-a205-40ba-bea2-4ae7a37c535a" />

SOP renewal dijalankan 5 peran secara berurutan:

1. Governance Admin/PMO Analyst — mengumpulkan daftar dokumen dari legacy Excel, cek expiry date manual, identifikasi dokumen yang perlu diperbarui, lalu tetapkan action item ke owner.
2. Document Owner/PIC — menerima assignment, menyusun draft revisi (atau lapor no change), perbaiki draft sesuai komentar, update tracker & simpan evidence manual.
3.Stakeholder Reviewer — review draft, kirim komentar/revisi/rejection bila belum ditindaklanjuti.
4.Approver/Process Owner — menerima permintaan approval, setujui atau kembalikan untuk diperbaiki.
5. Governance Admin/Document Control — publikasikan dokumen versi terbaru, lampirkan approval & completion evidence, update tracker manual, selesai.

### 3.2 To be Process

<img width="7908" height="3968" alt="image" src="https://github.com/user-attachments/assets/7e7fb127-b3c7-44fb-8b5e-97612583cca7" />

