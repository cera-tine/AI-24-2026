# KONTEKS LENGKAP — AI-24 (2026), Kelompok 2

Dibaca oleh AI di OpenCode sebelum mengerjakan apa pun.

---

## 1. Siapa kita

- Kelompok 2, mata kuliah AI, angkatan 2026.
- Anggota yang sudah aktif: **Heka** (user ini), **Firlana**, **Rizki**, **Anshar**.
- Athaya belum push apa pun.
- Anshar **bukan anggota kelompok** — repo Ecommerce-nya hanya ditumpangi sebagai contributor.
- Git user: `Zefanya Heka Herista` / GitHub: **`cera-tine`**.
- User = **Heka**. Anggap ini project pribadinya, bukan orang asing.

---

## 2. Instruksi asli dari Rizki (WA, terjemahan)

> Tiap orang pilih **1 konsep dari 5**, lalu buat **web** (boleh dibantu AI) + **promosi**
> (disarankan video animasi), upload ke IG/dll. Video, data, dan hasil prompting
> di-push ke **folder GitHub masing-masing**. Minggu ini mulai bikin promo + web pakai AI.
> Minggu depan mulai pengembangan. **Web yang paling banyak respons konsumennya**
> yang akan dikembangkan bareng untuk dikumpulkan.

Karena kelompok cuma 4 orang, Heka mengambil **2 konsep** supaya ada 2 kandidat
yang bisa dibandingkan responsnya. Ini disetujui dan aman.

---

## 3. 5 konsep resmi (dari `Rizki-1/persempitan-scope-5-konsep-bisnis.md`)

| Peringkat | Konsep | Ide asli | Skor |
|---|---|---|---|
| 1 | ShiftKu | Part-time fleksibel terpusat | 4,40 |
| 2 | **LombaLink** | Info akademik + partner lomba | **4,30** ← Heka |
| 3 | Teduh | Konseling terjangkau | 4,25 |
| 4 | BukuLoop | Preloved buku/barang kuliah | 3,80 |
| 5 | **KantinKilat** | Kantin anti-antri | **3,75** ← Heka |

Kriteria penilaian: K1 kekuatan bukti masalah (25%), K2 ukuran pasar & frekuensi (20%),
K3 kelayakan teknis (20%), K4 diferensiasi (20%), K5 kemudahan eksekusi (15%).

---

## 4. Riset yang jadi dasar

- **50 permasalahan mahasiswa** hasil gabungan riset Heka (30 sumber), Firlana (44 sumber),
  Rizki (30 sumber) →total **104 sumber**.
- Dipetakan ke **5 permasalahan inti** → 5 produk: Dompet Siaga, Kompas Peluang,
  Detak, Teman Skripsi, Peta Kampus.
- **LombaLink ≈ Kompas Peluang.**
- Data kunci yang dipakai di web LombaLink:
  - **80%** dari 350 mahasiswa FILKOM UB pernah bingung cari partner lomba.
  - **48%** kesulitan cari magang relevan jurusan.
  - Sumber: `Rizki-1/riset-informasi-akademik-terpusat.md`, `Rizki-1/sumber-30.csv`, jurnal IWIMA (68 responden).
- Verifikasi: 50/50 masalah tercatat (23 masuk 5 inti + 19 gugur + 8 di luar scope).
  Hanya #45 yang sengaja dipakai dua kali.

**Peringatan:** jangan hapus angka/klaim ini. Itu yang bikin web kredibel kalau ditanya dosen.
Kalau ditanya, sebutkan ukuran sampelnya (350 mahasiswa / 68 responden).

---

## 5. Yang SUDAH dikerjakan

### Repo `RizkiBSD/Kelompok-2-AI` (branch `main`)
- `TUGAS BERSAMA/Hasil Prompting Gabungan 50 Permasalahan Mahasiswa (...).md` — 50 masalah,
  20 konsep, mapping 50→5, 5 kartu inti, analisis kompetitor, 104 sumber.
- `Heka/web-lombalink/` — `index.html`, `PANDUAN.md`, `vercel.json`.
- `Heka/web-kantinkilat/` — `index.html`, `PANDUAN.md`, `vercel.json`.
- `Rizki-1/persempitan-scope-5-konsep-bisnis.md` — 10 ide → 5 konsep.
- Folder `Anshar/` **sudah dihapus** (Anshar bukan anggota kelompok).

### Isi web
Keduanya **landing page promosi + CTA**, 1 file HTML (HTML+CSS+JS jadi satu), responsif:
- **LombaLink:** hero → masalah → 4 fitur (Pencari Partner = unggulan, ada AI-flavored skill-matching)
  → cara kerja → tabel perbandingan → CTA → form daftar.
- **KantinKilat:** hero + mockup HP → masalah → 4 fitur → cara kerja → manfaat dua sisi
  → CTA → form daftar.

### GA4 (sudah terpasang, belum diisi ID)
- Snippet gtag.js di **baris 13** (`src=...id=G-XXXXXXXXXX`) dan **baris 18** (`gtag('config', ...)`).
- Event otomatis: `nav_daftar`, `hero_daftar`, `hero_lihat_fitur`/`hero_lihat_cara`,
  `cta_daftar`, `scroll_25/50/75/100`, `lihat_seksi`, `form_start`,
  `form_submit_attempt`, `form_success`, `form_error`.
- Metrik paling penting: **`form_success`** = jumlah pendaftar nyata.

---

## 6. Yang BELUM dikerjakan (prioritas)

1. **GA4 ID** — minta ke Rizki atau buat sendiri di analytics.google.com.
   Ganti 2 baris di tiap `index.html`. Kalau dapat 2 ID, pakai ID berbeda per web.
2. **Formspree** — daftar di formspree.io, ganti
   `https://formspree.io/f/GANTI-DENGAN-ENDPOINT-KAMU` (baris 532 / 557).
   Sebelum diganti, form sengaja menolak submit.
3. **Deploy Vercel** — import `RizkiBSD/Kelompok-2-AI`, Root Directory
   `Heka/web-lombalink` lalu `Heka/web-kantinkilat`, Framework Preset **Other**,
   Build Command & Output Directory dikosongkan.
4. **Tes GA4** — buka web, klik tombol, cek GA4 → Reports → **Realtime**.
   Jangan sebar link sebelum ini lolos.
5. **Cek tampilan HP** — traffic dari IG, jadi versi mobile yang paling penting.
6. **Video promosi** — 2 video pendek 15–30 detik (teks animasi pakai AI sudah cukup).
7. **Share ke IG/WA** — pakai UTM:
   `?utm_source=instagram&utm_medium=social&utm_campaign=lombalink`
8. **Push video + hasil prompting** ke folder `Heka/` di repo Rizki.
9. **Lapor ke Rizki dengan angka** — contoh: "LombaLink 47 pendaftar, KantinKilat 22".
   Ini penentu web mana yang dikembangkan bareng minggu depan.

---

## 7. Keputusan yang sudah diambil (jangan diulang)

- Install payment gateway (Midtrans/SumoPod) → **TIDAK**. Cukup mock checkout / pre-order.
- Next.js untuk 2 web ini → **TIDAK**. HTML satu file sengaja dipilih supaya gampang
  diedit manual & deploy tanpa build.
- Menggabungkan repo Anshar ke repo Rizki → **TIDAK**. Tetap 3 repo terpisah;
  Heka jadi contributor di repo Rizki dan repo Anshar.
- Mengembalikan `Heka/tes-30-topik` dan dokumen v1 yang dihapus user → **TIDAK**, karena
  user menghapusnya dengan sengaja ("butuhnya 1 aja").
- Branch tidak boleh pakai spasi → pakai `tugas-bersama`, bukan "TUGAS BERSAMA".
- Filename Windows tidak boleh pakai `*` → `(Athaya belum push)`.

---

## 8. Biaya

Vercel Hobby, GitHub publik, GA4, Formspree (50 kiriman/bulan) → **gratis, Rp 0**.

---

## 9. Aturan gaya bicara dengan user

- Pakai **Bahasa Indonesia**, santai tapi jelas.
- User sering bertanya bertahap dan perlu langkah konkret, bukan teori panjang.
- Kalau ada yang phải diganti manual, sebut **nomor baris** dan **path file** yang persis.
- Jangan beri kode GA4 palsu sebagai ID asli — selalu tandai placeholder.
