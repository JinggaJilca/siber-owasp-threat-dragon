# Threat Modeling: Aplikasi Web Berbagi Dokumen

Dokumentasi pemodelan ancaman (*Threat Modeling*) untuk **Aplikasi Web Berbagi Dokumen** menggunakan metodologi **STRIDE** (*Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, Elevation of Privilege*) dengan **OWASP Threat Dragon**.

* **Versi Arsitektur:** `v1.0 - Initial Architecture`
* **Metodologi:** STRIDE
* **Diagram Utama:** `DFD v1.0 - Sistem Berbagi Dokumen & Manajemen Tautan`

---

## Gambaran Umum Sistem

Aplikasi Web Berbagi Dokumen memfasilitasi pertukaran file secara terkontrol antara pihak internal dan eksternal organisasi. Sistem memisahkan penyimpanan atribut deskriptif file di **Database Metadata** dengan konten fisik file di **Object Storage**. Pemilik file dapat membuat tautan berbagi berdurasi **24 jam** yang dapat diakses oleh penerima tanpa perlu *login*, meninjau daftar tautan aktif, serta mencabut tautan sebelum masa berlakunya habis. Seluruh aktivitas pembuatan, pencabutan, dan penggunaan tautan dicatat dalam log audit yang dapat dipantau oleh Admin Organisasi tanpa memberikan akses langsung ke isi file.

---

## Cara Akses Model Ancaman

Anda dapat meninjau diagram DFD dan daftar analisis ancaman STRIDE pada repositori ini melalui salah satu metode berikut:

### Opsi 1: Menggunakan OWASP Threat Dragon Web (Direkomendasikan)
1. Buka aplikasi web **OWASP Threat Dragon** (versi daring atau *instance* lokal yang berjalan di perangkat Anda).
2. Pilih metode masuk menggunakan akun **GitHub** dan berikan otorisasi akses repositori.
3. Pilih akun/organisasi pemilik repositori ini, lalu pilih nama repositori beserta cabang (*branch*) utama (`main`).
4. Pilih berkas model ancaman yang terdaftar untuk membuka kanvas **DFD Level 1 - Sistem Berbagi Dokumen & Manajemen Tautan**.
5. Klik setiap elemen pada diagram (*Actor*, *Process*, *Data Store*, atau *Data Flow*) untuk melihat detail ancaman STRIDE dan mitigasinya pada panel sebelah kanan.
