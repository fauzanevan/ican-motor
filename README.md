# ICAN Motor — Katalog & Simulasi Kredit

Website React + Vite + Tailwind untuk katalog dan simulasi kredit motor Honda.

## Deploy ke GitHub + Vercel

1. Upload isi folder project ini ke repository GitHub.
2. Di Vercel pilih **Add New → Project** dan import repository tersebut.
3. Framework: **Vite**.
4. Root Directory: `./`.
5. Build command: `npm run build`.
6. Output directory: `dist`.

Tidak perlu Environment Variable untuk menjalankan versi sederhana ini.

## Mengubah profil/dealer

Edit `src/data/siteConfig.ts`.

## Mengubah gambar

Ganti file di `public/assets/` dengan nama yang sama.

## Catatan admin

Password admin pada versi sederhana ini adalah pengunci UI, bukan sistem autentikasi aman. Karena kode React dikirim ke browser, password dapat ditemukan oleh orang yang membongkar source aplikasi. Untuk admin sungguhan gunakan backend/authentication.
