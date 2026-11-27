# 🔗 Link website yang sudah live

| Web | URL | Status |
|---|---|---|
| **LombaLink** (file HTML dari chat ini) | https://lombalink-ten.vercel.app | ✅ Live, terverifikasi |
| **KantinKilat** (file HTML dari chat ini) | https://kantinkilat.vercel.app | ✅ Live, terverifikasi |

## Catatan penting

- `https://lombalink.vercel.app` **bukan** web kita — domain itu masih dipakai project lain
  (React/Vite) yang tidak ada di akun Vercel `cera-tine`. Karena itu deploy kita dapat
  alamat `lombalink-ten.vercel.app`.
- Kalau project lama itu dihapus oleh pemiliknya, domain `lombalink.vercel.app` bisa
  di-alias ke deployment kita.
- Kedua web masih memakai placeholder:
  - GA4: `G-XXXXXXXXXX` (baris 13 & 18 di tiap `index.html`)
  - Formspree: `https://formspree.io/f/GANTI-DENGAN-ENDPOINT-KAMU`

## Cara edit manual lewat GitHub + OpenCode

1. Buka https://github.com/cera-tine/AI-24-2026
2. Masuk folder `web-lombalink/` atau `web-kantinkilat/`
3. Klik ikon pensil → edit `index.html` → **Commit changes**
4. Vercel **tidak** otomatis deploy dari repo ini (karena deploy-nya dari CLI,
   bukan Git integration). Setelah edit, jalankan ulang:

```cmd
cd "C:\Users\Hype GLK\Downloads\web-lombalink"
npx vercel deploy --prod --yes
```

Atau buka folder project `AI-24-2026` di OpenCode, lalu paste `PROMPT-LANJUTAN.md`
dan minta AI helps deploy ulang.
