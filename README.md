# 🌐 MBC Laboratory Web - Contact & Developer Showcase

Website ini dikembangkan sebagai bagian dari **Technical Test MBC Laboratory – Divisi Cyber Security**. Proyek ini merupakan aplikasi web full-stack dengan tampilan frontend responsif, backend Node.js untuk pengiriman email, serta dukungan HTTPS melalui konfigurasi SSL.

---

## 📁 Struktur Proyek


project-root/

├── backend/ # Server Express.js

│ ├── index.js # Entry point backend

│ ├── .env # Konfigurasi variabel lingkungan

│ └── package.json # Dependency list

│

├── frontend/

│ ├── contact.html # Halaman contact

│ ├── contact.css # Styling halaman contact

│ ├── developer.html # Halaman developer

│ ├── developer.css # Styling halaman developer

│ ├── divisi.html # Halaman divisi & layanan

│ ├── divisi.css # Styling halaman divisi

│ └── assets/ # Gambar/logo (seperti mbclab1.png)

│

├── certs/ # Folder sertifikat SSL

│ ├── cert.pem # SSL Certificate

│ └── key.pem # SSL Private Key

│

└── README.md # Dokumentasi proyek


---

## ⚙️ Instalasi Lokal

### 1. Clone Repositori

```bash
git clone https://github.com/username/mbc-lab-contact-app.git
cd mbc-lab-contact-app
```

### 2. Install Backend Dependencies


cd backend

npm install express

npm install cors

npm install nodemailer

### 3. Buat File .env
Di dalam folder backend/, buat file .env seperti ini:

env

PORT=3000

EMAIL_USER=your-email@gmail.com

EMAIL_PASS=your-app-password (Gunakan App Password jika menggunakan Gmail + 2FA. Jangan gunakan password Gmail biasa.)

EMAIL_RECEIVER=receiver@example.com

### 4. Jalankan dengan SSL (HTTPS)

node index.js https

(Akses di: https://localhost:3000)


---

## 💌 Fungsi Backend
- Dibuat dengan Express.js

- Endpoint POST /send-email

- Menggunakan Nodemailer untuk kirim email ke admin

- Support HTTPS (SSL), CORS, dan validasi form

---

---

## ✉️ Format Data yang Dikirim dari Frontend

{

  "name": "Nama Pengirim",

  "email": "email@example.com",

  "title": "Subjek Pesan",

  "message": "Isi Pesan"

}

---


---

## 🧩 Fitur
- Google Maps Embed untuk lokasi

- Informasi developer + portofolio

- Tampilan responsive menggunakan HTML + CSS

- Form dengan validasi bawaan HTML5

---



