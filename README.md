# AI-24 (2026) — Project Kelompok 2

🔗 **Website live:** [LombaLink](https://lombalink-ten.vercel.app) · [KantinKilat](https://kantinkilat.vercel.app) — lihat `LINK-WEB.md`.

Folder project ini disiapkan supaya **teman bisa langsung lanjut mengerjakan di OpenCode**
tanpa perlu bertanya lagi dari nol.

---

## Cara lanjutin di OpenCode (untuk teman)

1. **Copy / clone folder ini** ke laptop masing-masing.
   - Kalau mau lewat GitHub: git clone repo kelompok dulu, lalu taruh folder ini di dalamnya.
2. Buka **OpenCode** → **Open Project** / **New Session** → pilih folder `AI-24-2026`.
3. Buka file **`PROMPT-LANJUTAN.md`**, copy isinya, paste ke chat OpenCode.
4. AI akan langsung tahu: siapa kita, apa tugasnya, apa yang sudah jadi, dan apa yang harus dilakukan.

> Kalau mau lanjut di folder repo aslinya, buka folder `Kelompok-2-AI` dan
> copy juga file `KONTEKS.md` + `PROMPT-LANJUTAN.md` ke root-nya.

---

## Isi folder ini

```
AI-24-2026/
├── README.md              ← kamu baca ini
├── KONTEKS.md             ← ringkasan lengkap: tugas, keputusan, status
├── PROMPT-LANJUTAN.md     ← prompt siap copy-paste ke OpenCode
├── web-lombalink/         ← landing page + GA4 + panduan deploy
└── web-kantinkilat/       ← landing page + GA4 + panduan deploy
```

---

## 3 repository yang dipakai

| Repo | Pemilik | Isi | Akses Heka |
|---|---|---|---|
| [`cera-tine/AI-s`](https://github.com/cera-tine/AI-s) | Heka (pribadi) | Chatbot + catatan riset pribadi | Owner |
| [`RizkiBSD/Kelompok-2-AI`](https://github.com/RizkiBSD/Kelompok-2-AI) | Rizki | **Repo utama kelompok** — riset, 50 masalah, 5 konsep, dan 2 web HTML di `Heka/web-*` | Collaborator ✅ |
| [`sharkeee-20/Ecommerce`](https://github.com/sharkeee-20/Ecommerce) | Anshar | Web Ecommerce (Next.js) milik Anshar | Collaborator ✅ |

**Catatan penting:**
- Anshar **bukan anggota kelompok**, jadi folder `Anshar/` di repo Rizki sudah **dihapus**.
- Web HTML (LombaLink & KantinKilat) **cukup ada di repo Rizki**, di folder `Heka/`.
- Kamu (Heka) sudah terdaftar sebagai **contributor** di repo Rizki **dan** repo Anshar.

---

## Status singkat

| Hal | Status |
|---|---|
| 50 permasalahan + 5 konsep inti | ✅ Selesai, di `TUGAS BERSAMA/` repo Rizki |
| Web LombaLink | ✅ Selesai, di `Heka/web-lombalink/` repo Rizki |
| Web KantinKilat | ✅ Selesai, di `Heka/web-kantinkilat/` repo Rizki |
| GA4 measurement ID | ⏳ Masih placeholder `G-XXXXXXXXXX` |
| Formspree endpoint | ⏳ Masih placeholder |
| Deploy Vercel | ⏳ Belum berhasil (repo Rizki punya Rizki — tinggal import dari dashboard) |
| Video promosi | ⏳ Belum dibuat |
| Upload ke IG / respons konsumen | ⏳ Belum |

---

## Yang paling sering ditanya teman

**Q: Kenapa aku pegang 2 web?**
A: Kelompok cuma 4 orang, jadi aku ambil 2 konsep: LombaLink (skor 4,30) dan
KantinKilat (skor 3,75). Nanti yang paling banyak respons konsumen yang dikembangkan bareng.

**Q: GA4-nya sudah jalan?**
A: Kodenya sudah, tapi ID-nya masih `G-XXXXXXXXXX`. Ganti di baris 13 & 18 tiap `index.html`.

**Q: Bisa deploy dari repo aku sendiri?**
A: Bisa, tapi sebaiknya langsung dari repo Rizki karena kamu sudah collaborator di sana.
Root directory: `Heka/web-lombalink` dan `Heka/web-kantinkilat`.
