# 📅 Jadwal Piket Mingguan Generator

Aplikasi web modern untuk membuat jadwal piket otomatis dengan sistem rotasi yang adil. Sempurna untuk sekolah, kantor, komunitas, atau organisasi yang memerlukan pembagian jadwal piket yang merata.

## ✨ Fitur Utama

- 🎲 **Pembagian Otomatis & Adil** - Algoritma rotasi cerdas memastikan setiap orang mendapat jumlah piket yang merata
- 📊 **Export Multi-Format** - Excel dengan styling, PDF, Copy to Clipboard, dan Print
- 🎨 **Dark/Light Mode** - Tema yang dapat disesuaikan untuk kenyamanan mata
- 📱 **Responsive Design** - Berfungsi sempurna di desktop, tablet, dan mobile
- 📈 **Statistik Real-time** - Lihat distribusi jadwal dan fairness metrics
- 🔄 **Regenerate** - Acak ulang jadwal dengan satu klik
- 💾 **No Dependencies** - 100% standalone, tidak perlu koneksi internet

## 🚀 Demo Langsung

[Live Demo](#) | [Download HTML](https://github.com/yourusername/jadwal-piket-generator)

## 📖 Cara Penggunaan

### 1. Input Data Dasar

```
Masukkan nama-nama petugas piket:
- Pisahkan dengan koma: Ahmad, Budi, Citra, Diana
- Atau dengan enter (satu nama per baris)
- Nama duplikat otomatis dihilangkan
```

### 2. Atur Periode Jadwal

- **Tanggal Mulai**: Pilih tanggal awal periode piket
- **Tanggal Selesai**: Pilih tanggal akhir periode piket
- Default: Awal hingga akhir bulan berjalan

### 3. Pilih Hari Kerja

```javascript
☑ Senin    ☑ Selasa   ☑ Rabu     ☑ Kamis
☑ Jumat    ☑ Sabtu    ☐ Minggu
```
Centang hari-hari yang memerlukan piket

### 4. Generate & Export

- Klik **🎲 Generate** untuk membuat jadwal
- **🔄 Acak Ulang** untuk variasi baru dengan distribusi tetap adil
- **📊 Export Excel** dengan format dan warna profesional
- **📄 Export PDF** untuk dokumen formal
- **📋 Copy** untuk paste ke aplikasi lain

## 🎯 Algoritma Rotasi Adil

Sistem menggunakan algoritma **Fair Rotation with Weekly Reset**:

```javascript
1. Track jumlah piket setiap orang
2. Prioritaskan orang dengan piket paling sedikit
3. Cegah seseorang piket 2x dalam minggu yang sama (jika memungkinkan)
4. Reset pool mingguan untuk variasi
5. Shuffle occasional untuk menghindari pola monoton
```

### Contoh Distribusi (9 orang, 30 hari kerja):

```
Ahmad    : ████ 4 hari
Budi     : ███ 3 hari  
Citra    : ████ 4 hari
Diana    : ███ 3 hari
Eko      : ███ 3 hari
Fajar    : ████ 4 hari
George   : ███ 3 hari
Heri     : ███ 3 hari
Irsyad   : ███ 3 hari
-----------------------
Gap: Max(4) - Min(3) = 1 ✅ Fair
```

## 📊 Format Export Excel

Export Excel menghasilkan file dengan styling profesional:

### Struktur Tabel
```
┌─────────┬──────────┬──────────┬──────────┬──────────┐
│         │ Minggu 1 │ Minggu 2 │ Minggu 3 │ Minggu 4 │
├─────────┼──────────┼──────────┼──────────┼──────────┤
│ Senin   │  AHMAD   │  DIANA   │  GEORGE  │  BUDI    │
│ Selasa  │  BUDI    │  EKO     │  HERI    │  CITRA   │
│ Rabu    │  CITRA   │  FAJAR   │  IRSYAD  │  DIANA   │
│ Kamis   │  DIANA   │  GEORGE  │  AHMAD   │  EKO     │
│ Jumat   │  EKO     │  HERI    │  BUDI    │  FAJAR   │
│ Sabtu   │  FAJAR   │  IRSYAD  │  CITRA   │  GEORGE  │
│ Minggu  │  LIBUR   │  LIBUR   │  LIBUR   │  LIBUR   │
└─────────┴──────────┴──────────┴──────────┴──────────┘
```

### Styling Features
- 🔵 **Header**: Background biru (#4472C4) dengan teks putih bold
- 🔷 **Kolom Hari**: Background biru muda (#B4C7E7)
- 🔄 **Zebra Stripes**: Baris genap biru sangat muda (#DBEEF4)
- 🟡 **Cell LIBUR**: Background kuning muda dengan teks italic
- 📐 **Borders**: Garis hitam untuk semua cell
- ❄️ **Freeze Panes**: Header dan kolom hari tetap terlihat saat scroll

## 🛠️ Instalasi

### Opsi 1: Penggunaan Lokal
```bash
1. Download file index.html
2. Buka dengan browser apapun (Chrome, Firefox, Edge, Safari)
3. Bookmark untuk akses cepat
```

### Opsi 2: Deploy ke GitHub Pages
```bash
# Clone atau buat repository baru
git init jadwal-piket-generator
cd jadwal-piket-generator

# Copy file HTML
# Save sebagai index.html

# Push ke GitHub
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/yourusername/jadwal-piket-generator.git
git push -u origin main

# Enable GitHub Pages
# Settings → Pages → Source: Deploy from branch → main
```

### Opsi 3: Web Server
Upload `index.html` ke hosting apapun (Netlify, Vercel, atau server tradisional)

## 💻 Teknologi

```javascript
{
  "HTML5": "Struktur semantic dan form controls",
  "CSS3": {
    "features": [
      "CSS Variables untuk theming",
      "Grid & Flexbox untuk layout",
      "Gradients & Animations",
      "Media queries untuk responsive"
    ]
  },
  "JavaScript": {
    "type": "Vanilla ES6+",
    "libraries": [
      "xlsx.js - Export Excel",
      "jsPDF - Generate PDF",
      "ExcelJS - Advanced Excel styling"
    ],
    "patterns": [
      "State management",
      "Event delegation",
      "Async/await"
    ]
  }
}
```

## 📱 Use Cases

### 🏫 **Sekolah/Kampus**
- Jadwal piket kelas harian
- Roster guru jaga
- Jadwal pengawas ujian
- Piket laboratorium

### 🏢 **Kantor/Perusahaan**
- Jadwal piket kebersihan
- Roster customer service
- Shift kerja karyawan
- Jadwal standby IT

### 🏘️ **Komunitas/RT-RW**
- Jadwal ronda malam
- Piket pos keamanan
- Jadwal imam masjid
- Roster jaga pos COVID

### 🏥 **Rumah Sakit/Klinik**
- Jadwal jaga dokter
- Roster perawat
- Piket apoteker
- Jadwal cleaning service

## 📸 Screenshots

### Desktop View - Light Mode
```
┌────────────────────────────────────────────────────┐
│  📅 Jadwal Piket Mingguan Generator           ☀️/🌙 │
├────────────────────────────────────────────────────┤
│                                                     │
│  📝 Daftar Nama                                    │
│  ┌────────────────────────────────────┐           │
│  │ Ahmad, Budi, Citra, Diana, Eko ... │           │
│  └────────────────────────────────────┘           │
│  Total: 9 nama unik                               │
│                                                     │
│  📅 Periode: [01/01/2025] - [31/01/2025]         │
│                                                     │
│  📆 Hari Kerja: ☑ Sen ☑ Sel ☑ Rab ☑ Kam ☑ Jum    │
│                                                     │
│  [🎲 Generate] [🔄 Acak Ulang] [🗑️ Reset]        │
│                                                     │
├────────────────────────────────────────────────────┤
│  📊 Statistik                                      │
│  ┌────┬────┬────┬────┐                           │
│  │ 9  │ 4  │ 22 │3.5 │                           │
│  │Nama│Ming│Hari│Avg │                           │
│  └────┴────┴────┴────┘                           │
│                                                     │
│  📆 Jadwal Piket Januari 2025                     │
│  ┌─────────────────────────────────┐              │
│  │ Tabel jadwal dengan warna       │              │
│  └─────────────────────────────────┘              │
│                                                     │
│  [📊 Excel] [📄 PDF] [📋 Copy] [🖨️ Print]        │
└────────────────────────────────────────────────────┘
```

### Mobile View
```
┌─────────────────┐
│ 📅 Generator    │
│      ☀️/🌙      │
├─────────────────┤
│ Input Names     │
│ [............]  │
│                 │
│ Date Range      │
│ [Start] [End]   │
│                 │
│ Work Days       │
│ ☑☑☑☑☑☑☐        │
│                 │
│ [🎲 Generate]   │
├─────────────────┤
│ Results         │
│ • Stats         │
│ • Schedule      │
│ • Export        │
└─────────────────┘
```

## 🔧 Konfigurasi & Customization

### Mengubah Warna Theme
```css
:root {
  --primary-gradient: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  --success-gradient: linear-gradient(135deg, #00c851, #00a152);
  /* Sesuaikan warna sesuai branding */
}
```

### Modifikasi Algoritma Rotasi
```javascript
// Di fungsi generateWeeklySchedule()
// Ubah logika prioritas sesuai kebutuhan
if (weekNumber % 2 === 0) {
    state.allNames = shuffleArray([...state.allNames]);
}
```

## 🐛 Troubleshooting

| Problem | Solution |
|---------|----------|
| Excel tidak ter-style | Browser mungkin tidak support ExcelJS, akan fallback ke export simple |
| Generate tidak jalan | Pastikan minimal ada nama sebanyak hari kerja per minggu |
| Print layout berantakan | Gunakan Chrome/Edge untuk hasil print terbaik |
| Dark mode tidak tersimpan | Fitur localStorage belum diimplementasi (future update) |

## 📝 Changelog

### Version 1.1.0 (Current)
- ✅ Fixed syntax error in export functions
- ✅ Added ExcelJS for advanced Excel styling
- ✅ Improved fair rotation algorithm
- ✅ Added zebra striping for better readability
- ✅ Enhanced mobile responsiveness

### Version 1.0.0
- Initial release
- Basic scheduling functionality
- Simple export features

## 🚧 Roadmap

- [ ] Save/Load jadwal dengan localStorage
- [ ] Multiple shift per hari
- [ ] Blacklist dates (tanggal merah)
- [ ] Preferensi personal (request hari tertentu)
- [ ] History jadwal sebelumnya
- [ ] Email notification
- [ ] Integration dengan Google Calendar API
- [ ] PWA support untuk offline usage
- [ ] Multi-language support

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

MIT License - Bebas digunakan untuk keperluan apapun

```
MIT License

Copyright (c) 2025 David Mario

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
```

## 👨‍💻 Author

**David Mario**
- Email: davidmario484@gmail.com
- GitHub: [@davidmario](https://github.com/davidmario)

## 🙏 Acknowledgments

- Terinspirasi dari kebutuhan pembagian jadwal piket yang adil dan transparan
- Thanks to all contributors and users
- Icons from emoji standard
- Libraries: xlsx.js, jsPDF, ExcelJS teams

## ❓ FAQ

**Q: Apakah bisa untuk jadwal shift (pagi/siang/malam)?**
A: Versi saat ini fokus pada jadwal harian. Fitur multi-shift dalam roadmap.

**Q: Bisakah export ke Google Calendar?**
A: Belum tersedia, tapi ada dalam roadmap untuk update mendatang.

**Q: Apakah data tersimpan?**
A: Belum ada fitur save permanen. Refresh = data hilang. Pastikan export dulu.

**Q: Support berapa maksimal nama?**
A: Technically unlimited, tapi untuk performa optimal disarankan < 100 nama.

---

📢 **Punya saran atau menemukan bug?** [Open an issue](https://github.com/yourusername/jadwal-piket-generator/issues)
