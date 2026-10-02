# OUR LITTLE UNIVERSE 🌌
*A Private Digital Love Story & Intimate Couple Journal*

Website dokumentasi hubungan eksklusif dengan nuansa **Dark Cinematic Romance**: romantis, intimate, cinematic, elegant, emotional, minimalistic, dan aesthetic.

---

## ✨ Fitur Utama

1. **Pre-loading / Fullscreen Cinematic Opening**:
   - **Scene 1**: Layar gelap pekat dengan titik cahaya tunggal yang perlahan membesar menjadi soft glow.
   - **Scene 2**: *“Two strangers.”* muncul perlahan dengan fade-in, lalu menghilang.
   - **Scene 3**: *“One unexpected story.”* dengan efek fade + slight blur transition.
   - **Scene 4**: *“And somehow…”* dengan cinematic pause.
   - **Scene 5**: *“We became us.”* dengan tipografi serif elegan dan subtle glow.
   - **Scene 6**: Tombol minimalis *“ENTER OUR UNIVERSE →”* dengan glowing border dan transisi zoom/fade cinematic mulus ke halaman utama.

2. **Hero Section**:
   - Headline: *“Somewhere between two strangers, we became us.”*
   - Subtitle: *“A collection of little moments, memories, and stories that became ours.”*
   - Foto editorial utama pasangan dengan rasio cinematic, grain 35mm, soft shadow, dan hover interaktif.
   - Counter otomatis *“Day XXX in our universe”* yang menghitung hari kebersamaan berdasarkan tanggal jadian.
   - Indikator *“SCROLL TO EXPLORE ↓”* dengan animasi mengambang halus.

3. **Sticky Minimal Navigation**:
   - Logo: *“OUR LITTLE UNIVERSE”*
   - Menu: `01 STORY`, `02 TIMELINE`, `03 MOMENTS`.
   - Transisi otomatis dari transparan ke glassmorphism (`backdrop-blur`) saat digeser.
   - Dilengkapi menu mobile fullscreen bergaya editorial mewah.
   - Tombol *“Prologue”* untuk memutar ulang opening cinematic kapan saja.

4. **Section 01 — HOW IT STARTED**:
   - Layout majalah/film journal editorial.
   - Kombinasi tipografi besar, narasi mendalam, koordinat tempat pertemuan pertama, tanggal, foto pendukung, dan quote callout.
   - Animasi scroll bertingkat (*staggered reveals*).

5. **Section 02 — OUR TIMELINE**:
   - Garis tipis vertikal di tengah dengan node bercahaya.
   - Milestone chapter: *The First Hello*, *The First Date*, *We Became Us*, *The Midnight Road Trip*, *Another Chapter*.
   - Cerita singkat dan foto setiap momen penting.

6. **Section 03 — LITTLE MOMENTS**:
   - Cinematic masonry/editorial photo gallery dengan rasio dinamis (portrait, landscape, square).
   - Hover effect: zoom halus, dark overlay, tanggal, dan caption romantis.
   - Fullscreen Lightbox interaktif dengan tombol prev/next, tombol close, dan navigasi keyboard (Esc, panah kiri/kanan).

7. **A Note Written in the Stars (Love Letter)**:
   - Catatan intim/surat cinta editorial dengan tipografi klasik dan soft ambient glow.

8. **Final Section**:
   - Latar kembali ke warna hitam pekat (*deep dark*).
   - Quote penutup: *“And this is only the beginning.”*
   - *“There are still so many moments we haven't lived yet.”*
   - Tombol *“OUR STORY CONTINUES →”* untuk kembali ke awal.
   - Penutup *“Made with love.”* dengan nama pasangan & simbol infinity (∞).

9. **Music Player (♫ OUR SONG)**:
   - Kontrol audio mengambang di pojok kanan bawah dengan visualizer gelombang suara animasi.
   - Fitur play, pause, dan mute.
   - Dilengkapi fallback Web Audio API ambient piano synthesizer jika koneksi offline atau audio diblokir browser, memastikan musik romantis selalu terdengar.

10. **Visual & Suasana**:
    - Palette: `#080808`, `#111111`, warm white, soft beige, champagne gold, muted rose.
    - Tekstur film grain 35mm.
    - Partikel stardust halus berkilau di latar belakang canvas 60fps.
    - Kursor minimalis desktop dengan soft halo trailing.

---

## 🛠️ Cara Menjalankan Website

Proyek ini telah dikonfigurasi dan siap dijalankan:

```bash
# Menjalankan development server
npm run dev

# Membuka di browser:
http://localhost:5173/

# Melakukan build produksi
npm run build
```

---

## 🎨 Cara Kustomisasi Konten & Foto

Semua teks, nama, tanggal, cerita, foto, dan lagu tersimpan rapi dalam satu file terpusat di:

📂 **`src/data/coupleData.js`**

### 1. Mengganti Nama Pasangan & Tanggal
Buka `src/data/coupleData.js`:
```javascript
export const coupleData = {
  partner1: "Wahyu",
  partner2: "Elena",
  anniversaryDate: "2024-05-18", // Format: YYYY-MM-DD (otomatis menghitung hari bersama)
  ...
};
```

### 2. Mengganti Foto dengan Foto Pribadi
Anda bisa:
1. Memasukkan file foto Anda ke dalam folder `public/images/` (contoh: `public/images/hero.jpg`, `public/images/first-date.jpg`).
2. Di dalam `src/data/coupleData.js`, ganti URL gambar menjadi:
   ```javascript
   mainImage: "/images/hero.jpg",
   ```
   Atau tetap menggunakan URL gambar online beresolusi tinggi (Unsplash, Cloudinary, Imgur, dll).

### 3. Mengganti Musik / Lagu Pasangan
Di dalam `coupleData.music`:
```javascript
music: {
  title: "Judul Lagu Favorit Kalian",
  artist: "Nama Artis",
  audioSrc: "/audio/our-song.mp3", // Letakkan file mp3 di folder public/audio/ atau gunakan link direct mp3
}
```

### 4. Mengubah Cerita & Timeline
Cukup edit teks pada bagian `story`, `timeline.milestones`, dan `moments.gallery`. Anda dapat menambah atau mengurangi momen sebanyak yang Anda inginkan.

---

## 📱 Responsivitas

Website ini telah dioptimalkan secara mendalam untuk semua perangkat:
- **Desktop & Laptop**: Tampilan layar lebar editorial mewah dengan kursor kustom dan efek hover halus.
- **Tablet**: Layout proporsional dengan grid 2 kolom.
- **Mobile Smartphone**: Navigasi hamburger eksklusif, tipografi dinamis yang nyaman dibaca, timeline yang tetap rapi, dan galeri sentuh yang mulus.
