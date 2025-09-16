# 🎲 Random Team Generator & Schedule Maker

Ahmad Fauzi
Budi Santoso
Citra Dewi
Diana Putri
Eko Prasetyo

```

2. **Atur Parameter**
- Jumlah Tim: 3
- Anggota per Tim: 2 (atau kosongkan untuk bagi rata)

3. **Generate!**
- Klik tombol "Generate Tim"
- Hasil langsung muncul dengan visualisasi menarik

### Mode Tim/Kelompok

**Use Case:** Pembagian kelompok presentasi, tim project, kelompok belajar

1. Pilih tab "Mode Tim/Kelompok"
2. Masukkan daftar nama (bisa copy-paste dari Excel)
3. Tentukan jumlah tim yang diinginkan
4. (Opsional) Tentukan jumlah anggota per tim
5. Pilih template penamaan
6. Klik "Generate Tim"

### Mode Jadwal Piket

**Use Case:** Jadwal piket harian, shift kerja, roster bulanan

1. Pilih tab "Mode Jadwal Piket"
2. Masukkan nama petugas
3. Set periode jadwal:
- Tanggal mulai
- Tanggal selesai
- Include/exclude weekend
4. Pilih template (Hari/Shift/Custom)
5. Klik "Generate Jadwal"

## 🏷️ Template Penamaan

| Template | Hasil | Use Case |
|----------|-------|----------|
| **Default** | Tim 1, Tim 2, Tim 3... | Pembagian kelompok umum |
| **Hari** | Senin, Selasa, Rabu... | Jadwal piket mingguan |
| **Minggu** | Minggu 1, Minggu 2... | Jadwal bulanan |
| **Bulan** | Januari, Februari... | Jadwal tahunan |
| **Shift** | Shift Pagi, Siang, Malam | Jadwal kerja shift |
| **Custom** | Sesuai input user | Nama tim khusus |

## 💾 Export Data

### Format Export yang Tersedia:

1. **📋 Copy Text**
```

=== HASIL PEMBAGIAN TIM ===
Tim 1: Ahmad, Budi, Citra
Tim 2: Diana, Eko, Fajar

```

2. **📊 Copy Table** - Format tab-separated untuk Excel

3. **💾 Download CSV** - File .csv dengan encoding UTF-8

4. **📅 Download Calendar (.ics)** - Untuk import ke:
- Google Calendar
- Microsoft Outlook
- Apple Calendar

5. **🖨️ Print** - Layout optimized untuk cetak

## 🛠️ Instalasi & Deployment

### Opsi 1: Local Usage

1. Download file `index.html`
2. Double-click untuk membuka di browser
3. Bookmark untuk akses cepat

### Opsi 2: GitHub Pages (Recommended)

1. **Fork/Clone Repository**
```bash
git clone https://github.com/yourusername/team-generator.git
```

2. **Push ke GitHub**
   ```bash
   git add index.html README.md
   git commit -m "Initial commit"
   git push origin main
   ```
3. **Enable GitHub Pages**
   * Settings → Pages
   * Source: Deploy from branch
   * Branch: main / (root)
   * Save
4. **Access Your App**
   ```
   https://yourusername.github.io/team-generator/
   ```

### Opsi 3: Web Server

Upload `index.html` ke web server manapun (Apache, Nginx, dll)

## 📱 Contoh Use Case

### 🏫 Pendidikan

* Pembagian kelompok diskusi
* Jadwal piket kelas
* Tim untuk praktikum
* Kelompok presentasi

### 🏢 Perkantoran

* Jadwal piket kebersihan
* Shift kerja karyawan
* Tim project
* Roster jaga malam

### 🏘️ Komunitas

* Jadwal ronda RT/RW
* Tim panitia acara
* Kelompok arisan
* Jadwal imam masjid

### 🏠 Keluarga

* Jadwal tugas rumah
* Pembagian kamar hotel
* Tim masak saat gathering
* Jadwal jaga orang sakit

## 📸 Screenshots

### Desktop View

```
┌─────────────────────────────────────┐
│     🎲 Random Team Generator        │
│                                     │
│  ┌──────┐  ┌──────┐  ┌──────┐     │
│  │ Tim 1│  │ Tim 2│  │ Tim 3│     │
│  │      │  │      │  │      │     │
│  │ • A  │  │ • D  │  │ • G  │     │
│  │ • B  │  │ • E  │  │ • H  │     │
│  │ • C  │  │ • F  │  │ • I  │     │
│  └──────┘  └──────┘  └──────┘     │
│                                     │
│  [Export CSV] [Copy] [Print]       │
└─────────────────────────────────────┘
```

### Mobile View

```
┌─────────────┐
│ 🎲 Generator│
├─────────────┤
│ Input Names │
│ [........]  │
│             │
│ Teams: [3]  │
│ Members:[2] │
│             │
│ [Generate]  │
├─────────────┤
│ Results:    │
│ • Tim 1     │
│ • Tim 2     │
│ • Tim 3     │
└─────────────┘
```

## 🔧 Teknologi

* **HTML5** - Struktur aplikasi
* **CSS3** - Styling dengan gradients, animations, flexbox/grid
* **Vanilla JavaScript** - Logika aplikasi tanpa framework
* **No Dependencies** - 100% standalone, tidak perlu library eksternal
* **Responsive Design** - Mobile-first approach
* **Local Storage Ready** - Untuk fitur save/load (future update)

## 📄 Lisensi

MIT License - Bebas digunakan untuk keperluan apapun

```
MIT License

Copyright (c) 2024 [Your Name]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 👨‍💻 Author

**[David Mario]**

* Email: davidmario484@gmail.com

## 🙏 Acknowledgments

* Terinspirasi dari kebutuhan pembagian tim yang adil
* Thanks to all contributors
* Icon dari emoji standard
