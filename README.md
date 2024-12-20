Berikut adalah README yang mencakup **Frontend (Next.js)** dan **Backend (NestJS)** untuk organisasi GitHub:

---

# **GridWiz Indonesia** 🚴‍♂️

Platform **Website Profile Company** untuk GridWiz Indonesia.

---

## **Deskripsi Proyek**

Proyek ini adalah pengembangan platform yang terdiri dari **Frontend** menggunakan **Next.js** dan **Backend** menggunakan **NestJS**. Proyek ini dirancang untuk menyediakan antarmuka pengguna yang modern serta API yang scalable dan secure.

---

## **Teknologi Utama**

### **Frontend**

- **Framework**: [Next.js](https://nextjs.org/)
- **Styling**: Tailwind CSS
- **State Management**: Context API / Redux (opsional)

### **Backend**

- **Framework**: [NestJS](https://nestjs.com/)
- **Database**: PostgreSQL
- **ORM**: TypeORM / Prisma
- **Autentikasi**: JWT (JSON Web Tokens)

---

## **Cara Menjalankan Proyek Secara Lokal**

### **Langkah 1: Clone Repository**

Clone repository frontend dan backend:

```bash
git clone https://github.com/gridwiz/gridwiz-frontend.git
git clone https://github.com/gridwiz/gridwiz-backend.git
```

---

### **Frontend (Next.js)**

1. **Masuk ke Folder Frontend**:

   ```bash
   cd gridwiz-frontend
   ```

2. **Instal Dependencies**:

   ```bash
   npm install
   ```

3. **Konfigurasi Environment Variables**:  
   Buat file `.env.local` dengan isi berikut:

   ```env
   NEXT_PUBLIC_API_URL=http://localhost:5000/api
   ```

4. **Jalankan Aplikasi**:

   ```bash
   npm run dev
   ```

5. **Akses Aplikasi**:  
   Buka [http://localhost:3000](http://localhost:3000) di browser Anda.

---

### **Backend (NestJS)**

1. **Masuk ke Folder Backend**:

   ```bash
   cd gridwiz-backend
   ```

2. **Instal Dependencies**:

   ```bash
   npm install
   ```

3. **Konfigurasi Environment Variables**:  
   Buat file `.env` dengan isi berikut:

   ```env
   DATABASE_URL=postgresql://username:password@host:port/dbname
   JWT_SECRET=your_jwt_secret
   PORT=5000
   ```

4. **Jalankan Database** (opsional):  
   Pastikan PostgreSQL berjalan di mesin lokal atau remote.

5. **Jalankan Aplikasi**:

   ```bash
   npm run start:dev
   ```

6. **Akses API**:  
   Backend akan berjalan di [http://localhost:5000](http://localhost:5000).

---

## **Struktur Folder**

### **Frontend (Next.js)**

```
gridwiz-frontend/
├── public/          # File statis (gambar, ikon, dll.)
├── src/
│   ├── components/  # Komponen UI yang dapat digunakan kembali
│   ├── pages/       # Halaman aplikasi (Next.js routing otomatis)
│   ├── styles/      # Styling global (Tailwind CSS atau custom CSS)
│   └── utils/       # Fungsi utilitas atau helper
├── .env.local       # Environment variables
├── next.config.js   # Konfigurasi Next.js
├── package.json
└── README.md
```

### **Backend (NestJS)**

```
gridwiz-backend/
├── src/
│   ├── modules/     # Modul-modul untuk fitur aplikasi
│   ├── controllers/ # Controller untuk route HTTP
│   ├── services/    # Logika bisnis aplikasi
│   ├── entities/    # Definisi entitas database
│   └── config/      # Konfigurasi aplikasi
├── .env             # Environment variables
├── ormconfig.json   # Konfigurasi TypeORM (opsional)
├── package.json
└── README.md
```

---

## **Deployment**

### **Frontend (Next.js)**

Frontend dapat di-deploy menggunakan platform seperti [Vercel](https://vercel.com/) atau Nginx di VPS.

### **Backend (NestJS)**

Backend dapat di-deploy di server VPS menggunakan Nginx sebagai reverse proxy atau dengan Docker untuk lingkungan terisolasi.

---

## **Kontribusi**

Kontribusi sangat dihargai!

1. Fork repository ini.
2. Buat branch fitur baru:
   ```bash
   git checkout -b feature/nama-fitur
   ```
3. Commit perubahan Anda:
   ```bash
   git commit -m "Menambahkan fitur baru"
   ```
4. Push ke branch Anda:
   ```bash
   git push origin feature/nama-fitur
   ```
5. Ajukan pull request.

---

## **Lisensi**

Proyek ini dilisensikan di bawah [MIT License](LICENSE).

---

## **Kontak**

- **Email**: gridwizenergyandmobility@gmail.com
- **Website**: [https://gridwizenm.com/](https://gridwizenm.com/)

---

README ini mencakup instruksi untuk **Frontend** dan **Backend**, serta struktur folder untuk membantu pengembang memahami arsitektur proyek. Jika ada penyesuaian tambahan, beri tahu saya!
