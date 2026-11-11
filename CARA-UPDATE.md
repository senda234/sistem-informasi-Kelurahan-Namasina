# 📋 Cara Update Konten Tanpa Ganti QR Code

## Isi folder yang perlu di-upload ke Netlify:
```
📁 Siaga Info/
├── index.html     ← tampilan (tidak perlu diubah)
├── data.json      ← DATA (ini yang diubah kalau ada perubahan)
└── LOGO.jpeg      ← logo KKN
```

---

## 🔧 Setup Awal (sekali saja)

### Langkah 1 — Buat akun GitHub (gratis)
1. Buka https://github.com/signup
2. Daftar dengan email

### Langkah 2 — Upload folder ke GitHub
1. Login GitHub → klik tombol hijau **"New"** (buat repository baru)
2. Nama repo: `siaga-namasina` → klik **"Create repository"**
3. Klik **"uploading an existing file"**
4. Drag ketiga file: `index.html`, `data.json`, `LOGO.jpeg`
5. Klik **"Commit changes"**

### Langkah 3 — Hubungkan ke Netlify
1. Buka https://netlify.com → Login/daftar
2. Klik **"Add new site"** → **"Import an existing project"**
3. Pilih **GitHub** → pilih repo `siaga-namasina`
4. Klik **"Deploy"** — tunggu selesai
5. Kamu dapat URL seperti: `https://namasina-siaga.netlify.app`
6. **Buat QR code dari URL ini** — QR code tidak perlu diganti lagi selamanya!

---

## ✏️ Cara Update Data (setelah setup)

### Kalau mau ubah jam, nama staf, nomor darurat, dll:

1. Buka https://github.com
2. Masuk ke repo `siaga-namasina`
3. Klik file **`data.json`**
4. Klik ikon pensil ✏️ (pojok kanan atas)
5. Edit isi yang mau diubah
6. Klik **"Commit changes"** (tombol hijau)
7. Tunggu 1-2 menit → website otomatis terupdate!

**QR code tetap sama, URL tidak berubah. ✅**

---

## 📝 Panduan Edit data.json

### Ubah jam pelayanan:
```json
"jam": [
  ["Senin",   "08.00 – 15.30"],
  ["Jumat",   "08.00 – 11.30"],
  ["Sabtu",   "Tutup"]
]
```

### Tambah nomor darurat baru:
```json
"darurat": [
  ["110", "Polisi"],
  ["112", "Nomor Baru"]
]
```

### Tambah jenis surat baru:
```json
"surat": {
  "Nama Surat": ["Syarat 1", "Syarat 2", "Syarat 3"]
}
```

> ⚠️ Jangan hapus tanda `"` `{` `}` `[` `]` `,` karena bisa error.
> Kalau ragu, hubungi mahasiswa KKN yang buat sistem ini.
