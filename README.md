# ICAN Motor — Katalog & Simulasi Kredit

Website React + Vite + Tailwind untuk katalog dan simulasi kredit motor Honda.

## Konsep data sederhana
Repository GitHub dipakai sebagai tempat menyimpan:
- `public/assets/` → logo, foto sales, banner, gambar motor.
- `src/data/siteConfig.ts` → nama dealer, nama sales, WhatsApp, logo/foto yang dipakai.
- `src/App.tsx` → tampilan dan data simulasi kredit.

Ini adalah **static data store berbasis Git**, bukan database server. Setiap perubahan di GitHub akan ikut ter-deploy oleh Vercel.

## Jalankan lokal
```bash
npm install
npm run dev
```

## Build production
```bash
npm run build
```

## Deploy Vercel
Import repository GitHub ke Vercel. Framework preset: Vite. Build command: `npm run build`. Output directory: `dist`.

## Catatan keamanan
Password mode admin pada kode lama tidak aman untuk dijadikan sistem admin sungguhan. Versi ini mengambil password dari environment variable `VITE_ADMIN_PASSWORD`, tetapi nilai VITE tetap terkirim ke browser. Jadi fitur tersebut hanya cocok sebagai pengunci UI sederhana, **bukan autentikasi aman**. Untuk admin sungguhan gunakan backend/authentication.
