# Test Scenarios — SiapKerja: Eksplor Lowongan JKP

*Dokumen ini tersedia dalam Bahasa Indonesia dan English version below.*
...
## 🇮🇩 Bahasa Indonesia

### 📅 Tanggal penyusunan: 9 Juli 2025  
### 📌 Modul: Eksplor Lowongan JKP  
### 🧪 Tujuan: Menguji fungsi eksplorasi lowongan pekerjaan dari program Jaminan Kehilangan Pekerjaan (JKP) di aplikasi SiapKerja

Deskripsi : Dokumen ini berisi daftar test scenario untuk fitur eksplorasi lowongan pekerjaan pada aplikasi SiapKerja, khususnya lowongan yang tersedia melalui program JKP (Jaminan Kehilangan Pekerjaan).

| Scenario ID | Deskripsi Skenario                          | Tujuan Pengujian                                                           |
|-------------|----------------------------------------------|----------------------------------------------------------------------------|
| TS001       | Pencarian lowongan berdasarkan keyword       | Memastikan lowongan yang relevan muncul sesuai kata kunci pencarian       |
| TS002       | Tampilan detail lowongan pekerjaan           | Memastikan halaman detail menampilkan informasi lengkap dan benar         |
| TS003       | Penanganan saat tidak ada lowongan tersedia  | Memastikan sistem menampilkan pesan/error yang sesuai saat data kosong    |
| TS004       | Tombol "Lamar Sekarang" pada detail lowongan | Memastikan tombol muncul dan dapat diklik untuk melanjutkan proses lamaran|
| TS005       | Navigasi balik ke daftar lowongan            | Memastikan user dapat kembali ke halaman daftar tanpa error               |
| TS006       | Pencarian tanpa input (kosong)               | Memastikan sistem tidak error dan memberikan hasil default atau instruksi |
| TS007       | Filter lokasi atau kategori lowongan         | Memastikan filter berfungsi sesuai pilihan user                           |

---

## 🇬🇧 English Version

### 📅 Created on: July 9, 2025  
### 📌 Module: Job Vacancy Exploration (JKP)  
### 🧪 Purpose: To validate the job exploration feature under the JKP program in SiapKerja application

Description : This document contains a list of test scenarios for the job vacancy exploration feature in the SiapKerja application, specifically vacancies available through the JKP (Job Loss Guarantee) programme.

| Scenario ID | Scenario Description                        | Test Objective                                                           |
|-------------|----------------------------------------------|--------------------------------------------------------------------------|
| TS001       | Search job listings using keywords           | Ensure relevant listings appear based on entered keywords               |
| TS002       | View job vacancy details                     | Ensure the details page displays complete and correct information       |
| TS003       | Handle empty job listing results             | Ensure system displays correct message when no jobs are found           |
| TS004       | "Apply Now" button on job detail page        | Ensure the button appears and is clickable to proceed with application  |
| TS005       | Navigate back to job list from detail view   | Ensure user can return to listing page without error                    |
| TS006       | Search with empty input                      | Ensure no crash and default results or instructions are shown           |
| TS007       | Filter jobs by location or category          | Ensure filter works based on selected user criteria                     |

---

## 🗒️ Catatan / Notes

- Semua skenario diasumsikan dijalankan oleh user yang sudah login.  
  _All scenarios assume the user is logged in._
- Pengujian dilakukan berbasis UI publik (tanpa akses sistem internal).  
  _Testing is conducted based on public UI (no internal system access)._  
- Test case terperinci tersedia di `test-cases.xlsx` atau akan disusulkan.  
  _Detailed test cases available in `test-cases.xlsx` or upcoming._
