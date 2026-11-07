# VELORA MUSIC — Official Download Website

Website resmi pusat download aplikasi **VELORA MUSIC**.

Desain: Modern Editorial + Liquid Glass + Swiss Minimalist + Apple-inspired SaaS.

---

## Struktur

```
velora-music/
├── index.html    # Website lengkap (HTML + CSS + JS)
└── README.md     # Dokumentasi ini
```

Satu file `index.html` — tidak butuh build, tidak butuh Node, tidak butuh backend.

---

## Fitur

- Splash screen dengan animasi logo
- Header sticky + navigasi + mobile menu
- Hero section premium
- **Download Center**
  - VELORA 5.0.0 **RECOMMENDED** (badge jelas)
  - VELORA 4.3.2 **STABLE**
  - Download langsung dari link APK (tanpa redirect GitHub)
  - Countdown visual 5 detik + status sukses
  - Anti double-download
- Windows / PC section (Coming Soon — tombol disabled)
- Support Developer → Saweria
- Contact & Community (Telegram, WhatsApp, TikTok)
- About VELORA
- Developer & Support Team
- Footer + watermark AryaProject
- Open Graph + Twitter Card (preview saat share di WA/Telegram/Discord)
- Favicon SVG + theme-color
- Smooth scroll, scroll-reveal, micro-interactions
- Responsive (mobile-first)
- `prefers-reduced-motion` dihormati

---

## Cara menjalankan

### Lokal
Buka `index.html` langsung di browser.

### Deploy (gratis)
Cocok untuk:
- **GitHub Pages**
- **Vercel**
- **Netlify**
- **Cloudflare Pages**

Cukup upload `index.html` (atau seluruh folder). Tidak ada step build.

#### GitHub Pages cepat
1. Buat repository baru
2. Upload `index.html`
3. Settings → Pages → Source: Deploy from a branch → `main` / root
4. Setelah live, update meta `og:url` di `<head>` sesuai domain Anda

---

## Konfigurasi (penting)

Semua link terpusat di objek `CONFIG` di dalam `<script>` (bagian bawah `index.html`):

```js
const CONFIG = {
  telegram: "",                                    // isi: "https://t.me/username"
  whatsappDev: "https://wa.me/6281246679050",
  whatsappMaintainer: "https://wa.me/6281234200500",
  tiktok: "",                                      // isi: "https://www.tiktok.com/@username"
  saweria: "https://saweria.co/OfficialG1",
  apk: {
    recommended: "https://github.com/aryaexeuyf/Image/releases/download/3.0.0/Levora_2026-5.0.0.recoedition.apk",
    stable: "https://github.com/aryaexeuyf/Image/releases/download/3.0.0/Levora_2026-4.3.2.stable.edition.apk"
  }
};
```

- Telegram & TikTok masih kosong → tombol akan memberi peringatan sampai diisi.
- WhatsApp sudah mengarah ke nomor Developer.
- Link APK sudah terpasang sesuai spesifikasi.

---

## Metadata / Link Preview

Saat link dibagikan di WhatsApp, Telegram, Discord, dll:

- **Title:** VELORA MUSIC — Your Music, Your Atmosphere
- **Description:** deskripsi profesional singkat
- **Image:**  
  `https://raw.githubusercontent.com/aryaexeuyf/Levora-music/main/file_000000006b188211bb23832c28b40a3a.png`

Pastikan setelah deploy, `og:url` diganti ke domain asli agar preview stabil.

---

## Kontak (dari website)

| Peran        | Kontak              |
|--------------|---------------------|
| Developer    | +62 812-4667-9050   |
| Maintainer   | +62 812-3420-0500   |

**Support Team:** Kenzi · Syifa'ur · Vick Firmansyah · Reyvan · Akbar

---

## Catatan teknis

- Pure HTML5 + CSS3 + Vanilla JavaScript
- Tidak ada dependency berbayar / berat
- Kompatibel GitHub Pages & Vercel
- External link memakai `rel="noopener noreferrer"`
- Tombol Windows tidak punya `href` dan tidak bisa diklik

---

**The project was carried out by developer AryaProject.**  
VELORA MUSIC © 2026 · Developed by AryaProject.
