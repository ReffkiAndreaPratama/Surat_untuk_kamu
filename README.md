# 💖 RomCom — Romantic Web App

Sebuah halaman web romantis yang dibuat dengan React, Tailwind CSS, dan Framer Motion. Cocok dijadikan hadiah digital untuk orang tersayang — penuh animasi, musik, dan pesan cinta.

---

## ✨ Fitur

| Fitur | Deskripsi |
|---|---|
| 🎬 **Hero Section** | Tampilan pembuka sinematik dengan animasi heartbeat dan teks gradient |
| 💌 **Love Message** | Kartu kutipan cinta dengan animasi slide masuk bergantian |
| 🌹 **Romantic Cards** | Tiga kartu bertema Cinta, Kenangan, dan Harapan dengan efek hover |
| ❤️ **Love Button** | Tombol interaktif yang memunculkan ledakan hati saat diklik |
| ⏳ **Countdown** | Hitung mundur / hitung maju real-time untuk momen spesial (hari jadian, pertama bertemu, anniversary) |
| 📸 **Gallery** | Grid foto kenangan dengan lightbox, navigasi prev/next, dan fitur upload foto sendiri |
| 🎵 **Music Player** | Pemutar musik latar romantis dengan animasi equalizer, auto-play saat interaksi pertama |
| 💫 **Floating Hearts** | Hati-hati melayang di latar belakang secara terus-menerus |
| ✨ **Sparkle Effect** | Efek bintang kecil yang muncul mengikuti kursor |
| 🌌 **Parallax Background** | Latar belakang dengan orb cahaya yang bergerak mengikuti scroll |

---

## 🛠️ Tech Stack

- **React 19** — UI library
- **Vite** — build tool & dev server
- **Tailwind CSS 3** — utility-first styling
- **Framer Motion** — animasi dan transisi
- **Google Fonts** — Dancing Script, Playfair Display, Inter

---

## 🚀 Cara Menjalankan

### Prasyarat

- Node.js >= 18
- npm >= 9

### Instalasi

```bash
# Clone repositori
git clone <url-repo>
cd romcom

# Install dependensi
npm install
```

### Development

```bash
npm run dev
```

Buka [http://localhost:5173](http://localhost:5173) di browser.

### Build untuk Produksi

```bash
npm run build
```

Output akan tersimpan di folder `dist/`.

### Preview Build

```bash
npm run preview
```

---

## 📁 Struktur Proyek

```
romcom/
├── public/
│   ├── gallery1.png – gallery6.png   # Foto default galeri
│   ├── icons.svg
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── HeroSection.jsx           # Halaman pembuka
│   │   ├── LoveMessageSection.jsx    # Kartu kutipan cinta
│   │   ├── RomanticCards.jsx         # Kartu Cinta / Kenangan / Harapan
│   │   ├── LoveButton.jsx            # Tombol interaktif dengan efek ledakan hati
│   │   ├── CountdownSection.jsx      # Timer hitung mundur/maju
│   │   ├── GallerySection.jsx        # Galeri foto dengan lightbox
│   │   ├── MusicPlayer.jsx           # Pemutar musik latar
│   │   ├── FloatingHearts.jsx        # Animasi hati melayang
│   │   ├── SparkleEffect.jsx         # Efek sparkle mengikuti kursor
│   │   └── ParallaxBackground.jsx    # Latar belakang parallax
│   ├── App.jsx                       # Root component
│   ├── App.css
│   ├── index.css                     # Global styles & CSS variables
│   └── main.jsx
├── index.html
├── tailwind.config.js
├── vite.config.js
└── package.json
```

---

## 🎨 Kustomisasi

### Ganti Tanggal Momen Spesial

Edit array `EVENTS` di `src/components/CountdownSection.jsx`:

```js
const EVENTS = [
  {
    label: 'Hari Jadian',
    icon: '💑',
    date: new Date('2024-02-14T00:00:00'), // ← ganti tanggal
    color: '#FF6B9D',
  },
  // ...
]
```

### Ganti Foto Galeri

Ganti file `public/gallery1.png` hingga `gallery6.png` dengan foto milikmu, atau gunakan tombol **Upload Foto** langsung di halaman.

### Ganti Pesan Cinta

Edit array `QUOTES` di `src/components/LoveMessageSection.jsx` untuk mengubah kutipan yang ditampilkan.

### Ganti Musik

Ganti nilai `MUSIC_URL` di `src/components/MusicPlayer.jsx` dengan URL file audio pilihanmu:

```js
const MUSIC_URL = 'https://example.com/your-song.mp3'
```

---

## 📜 Lisensi

Proyek ini bebas digunakan untuk keperluan pribadi. Dibuat dengan 💖.
