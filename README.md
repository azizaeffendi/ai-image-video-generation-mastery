<div align="center">

# 🎨 AI Image & Video Generation Mastery

**Panduan Terlengkap — Generate gambar & video AI yang konsisten, berkualitas, dan siap dimonetisasi**

[![Midjourney](https://img.shields.io/badge/Midjourney-v6-black?style=for-the-badge)](https://midjourney.com)
[![DALL-E](https://img.shields.io/badge/DALL--E-3-412991?style=for-the-badge&logo=openai)](https://openai.com)
[![Stable Diffusion](https://img.shields.io/badge/Stable%20Diffusion-XL-orange?style=for-the-badge)](https://stability.ai)
[![Runway](https://img.shields.io/badge/Runway-Gen3-blue?style=for-the-badge)](https://runwayml.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)
[![Made in Indonesia](https://img.shields.io/badge/Made%20in-Indonesia-red?style=for-the-badge)](https://github.com/azizaeffendi)

<br/>

> **Banyak orang bisa generate gambar AI. Sangat sedikit yang bisa generate KONSISTEN dan BERKUALITAS. Panduan ini mengajarkan KEDUANYA — plus cara menghasilkan uang darinya.**

```
┌──────────────────────────────────────────────────────────────────┐
│              AI CONTENT CREATION ECOSYSTEM                       │
├─────────────────────────┬────────────────────────────────────────┤
│  🖼️ IMAGE GENERATION    │  🎬 VIDEO GENERATION                   │
│  ─────────────────      │  ──────────────────                    │
│  Midjourney v6          │  Runway Gen-3 Alpha                   │
│  DALL-E 3               │  Kling AI                             │
│  Stable Diffusion XL    │  Sora (OpenAI)                        │
│  Leonardo AI            │  Pika Labs                            │
│  Adobe Firefly          │  HeyGen (AI Avatar)                   │
│  Ideogram               │  Luma Dream Machine                   │
├─────────────────────────┼────────────────────────────────────────┤
│  🎙️ AI VOICE            │  🎵 AI MUSIC & SOUND                  │
│  ElevenLabs             │  Suno AI                              │
│  Murf AI                │  Udio                                 │
│  PlayHT                 │  Soundraw                             │
└─────────────────────────┴────────────────────────────────────────┘
```

[🖼️ Image Guides](#-panduan-per-tools) · [🎬 Video Guides](#-video-generation) · [🔑 Consistency](#-teknik-konsistensi) · [💰 Monetisasi](#-cara-menghasilkan-uang)

</div>

---

## 🌟 Apa yang Akan Kamu Pelajari

```
Level 1 — BASIC:       Generate gambar sederhana dengan prompt basic
Level 2 — INTERMEDIATE: Teknik advanced prompt + konsistensi karakter
Level 3 — ADVANCED:    Workflow otomasi + video generation + brand system
Level 4 — MASTER:      Monetisasi + membangun bisnis dari AI content
```

---

## 📚 Daftar Isi

| # | Topik | File | Level |
|---|-------|------|-------|
| 01 | Perbandingan Semua Tools AI | [tools-comparison.md](guides/01-tools-comparison.md) | Semua |
| 02 | Midjourney — Panduan Lengkap | [midjourney-mastery.md](guides/02-midjourney-mastery.md) | Basic–Master |
| 03 | DALL-E 3 & ChatGPT Image | [dalle-guide.md](guides/03-dalle-guide.md) | Basic–Advanced |
| 04 | Stable Diffusion — Open Source | [stable-diffusion.md](guides/04-stable-diffusion.md) | Intermediate–Master |
| 05 | Leonardo AI — Konsistensi Karakter | [leonardo-ai.md](guides/05-leonardo-ai.md) | Intermediate |
| 06 | Runway Gen-3 — Video AI | [runway-video.md](guides/06-runway-video.md) | Intermediate–Advanced |
| 07 | Kling AI — Video Realistis | [kling-ai.md](guides/07-kling-ai.md) | Intermediate |
| 08 | HeyGen — AI Avatar & Talking Head | [heygen-avatar.md](guides/08-heygen-avatar.md) | Basic–Advanced |
| 09 | Teknik Konsistensi — Karakter & Style | [consistency-mastery.md](guides/09-consistency-mastery.md) | Advanced |
| 10 | Prompt Formula 200+ | [prompt-library.md](guides/10-prompt-library.md) | Semua |
| 11 | Hook Visual — Stop The Scroll | [visual-hooks.md](guides/11-visual-hooks.md) | Intermediate |
| 12 | Workflow Otomasi dengan AI | [automation-workflow.md](guides/12-automation-workflow.md) | Advanced |
| 13 | Cara Menghasilkan Uang | [monetization.md](guides/13-monetization.md) | Semua |

---

## 🛠️ Panduan Per Tools

### 🔵 MIDJOURNEY v6 — Raja AI Image

**Terbaik untuk**: Artistic quality, photorealism, brand imagery

**Pricing**: $10-$120/bulan

**Prompt Formula Dasar**:
```
[SUBJEK] + [AKSI/POSE] + [ENVIRONMENT] + [LIGHTING] + [STYLE] + [PARAMETERS]

Contoh:
young Indonesian woman, confident smile, modern Jakarta office background,
natural soft window lighting, professional portrait photography style,
shot on Sony A7R V, f/1.8, --ar 4:5 --v 6.1 --style raw --q 2
```

**Parameter Wajib Dikuasai**:
```
--v 6.1          → Versi terbaru (terbaik)
--ar 16:9        → Aspect ratio (16:9 untuk video/YouTube, 4:5 untuk Instagram, 1:1 square)
--style raw      → Lebih realistis, less artistic
--q 2            → Quality tertinggi
--cref [URL]     → Character Reference — kunci konsistensi karakter!
--sref [URL]     → Style Reference — tiru gaya visual
--cw 50          → Character Weight (0-100, seberapa mirip dengan reference)
--s 0-1000       → Stylize (0=literal, 1000=sangat artistic)
--chaos 0-100    → Variasi hasil (0=konsisten, 100=sangat random)
--seed [angka]   → Lock seed untuk hasil yang bisa direproduksi
--no [elemen]    → Negative prompt ("--no text, watermark, blurry")
```

---

### 🟢 DALL-E 3 — Terintegrasi ChatGPT

**Terbaik untuk**: Text-in-image, precise instructions, iterasi cepat

**Pricing**: Gratis (limited) via ChatGPT, atau API $0.04-0.12/image

**Cara Terbaik Menggunakan DALL-E 3**:
```
Gunakan ChatGPT sebagai "prompt enhancer":

Pesan ke ChatGPT:
"Aku ingin generate gambar dengan DALL-E untuk [TUJUAN].
Subjek: [deskripsi]
Style: [gaya]
Mood: [suasana]
Tolong buat prompt DALL-E yang sangat detail dan optimized."

ChatGPT akan buat prompt jauh lebih baik dari yang kamu tulis sendiri!
```

**Kelebihan DALL-E 3**:
- Paling baik dalam memasukkan TEXT di dalam gambar
- Mengikuti instruksi paling akurat
- Integrasi langsung di ChatGPT
- API paling mudah diintegrasikan ke aplikasi

---

### 🟠 STABLE DIFFUSION — Open Source Gratis

**Terbaik untuk**: Custom model, lokal, unlimited, kontrol penuh

**Pricing**: GRATIS (self-hosted) atau via API

**Tools untuk Run Stable Diffusion**:
```
ComfyUI     → Paling powerful, node-based workflow (Recommended)
Automatic1111 → Paling populer, feature lengkap
InvokeAI    → UI yang friendly, bagus untuk pemula
Fooocus     → Sangat mudah, mirip Midjourney tapi gratis
```

**Model Terbaik 2024-2026**:
```
SDXL 1.0          → Base model terbaik dari Stability AI
Juggernaut XL     → Terbaik untuk foto realistis
DreamShaper XL    → Versatile, semua gaya
RealVisXL         → Hyper realistis
Animagine XL      → Anime style
```

---

## 🎬 Video Generation

### Platform Perbandingan

| Platform | Terbaik Untuk | Harga | Kualitas | Durasi Max |
|----------|--------------|-------|---------|-----------|
| **Runway Gen-3** | Sinematik, efek | $15-95/bulan | ⭐⭐⭐⭐⭐ | 10 detik |
| **Kling AI** | Realistis, motion alami | $8-66/bulan | ⭐⭐⭐⭐⭐ | 5-10 detik |
| **Sora (OpenAI)** | Konsistensi tinggi | $20+/bulan | ⭐⭐⭐⭐⭐ | 20 detik |
| **Pika Labs** | Animasi, kreatif | $8-28/bulan | ⭐⭐⭐⭐ | 3-10 detik |
| **Luma Dream Machine** | Natural motion | Gratis/berbayar | ⭐⭐⭐⭐ | 5 detik |
| **HeyGen** | AI Avatar, talking head | $24-120/bulan | ⭐⭐⭐⭐ | Unlimited |
| **Descript** | Edit video dengan teks | $15-30/bulan | Tool edit | Unlimited |

---

## 🔑 Teknik Konsistensi

### Konsistensi Karakter di Midjourney

```
MASALAH: Setiap generate Midjourney menghasilkan wajah yang berbeda
SOLUSI: --cref (Character Reference)

STEP 1: Buat "master character sheet"
Generate wajah karakter yang kamu suka, save URL gambar tersebut

STEP 2: Gunakan --cref di semua prompt selanjutnya
/imagine prompt: [karakter kamu] di [situasi baru] --cref [URL master] --cw 85

STEP 3: Fine-tune dengan --cw (character weight)
--cw 0   → Hanya ambil style, abaikan wajah
--cw 50  → Keseimbangan (RECOMMENDED untuk variasi pose)
--cw 100 → Ikuti persis wajah (kadang hasilnya kaku)
```

### Konsistensi Style Brand

```
UNTUK BRAND VISUAL YANG KONSISTEN:

1. Buat "Style Bible" — 5-10 gambar yang represent visual brand kamu
2. Upload ke Midjourney
3. Gunakan --sref [URL1] [URL2] ... untuk reference multiple gambar
4. --sw (style weight) untuk kontrol seberapa kuat reference-nya

Contoh brand photography yang konsisten:
--sref [URL foto brand 1] [URL foto brand 2] --sw 300 --style raw
```

### Konsistensi di Stable Diffusion (LoRA)

```
LoRA = Low-Rank Adaptation — "add-on" untuk melatih karakter/style spesifik

CARA KERJA:
1. Kumpulkan 15-30 foto reference karakter/style yang kamu inginkan
2. Train LoRA (bisa di Google Colab gratis atau via Civitai)
3. Load LoRA saat generate: <lora:nama_lora:0.8>

HASIL: Karakter PERSIS sama di ribuan gambar berbeda
COCOK UNTUK: Brand mascot, konsisten character story, brand photography
```

---

## 💡 Visual Hooks — Stop The Scroll

### 10 Formula Visual Hook yang Viral

**1. BEFORE-AFTER SPLIT**
```
Kiri: situasi "sebelum" yang relate | Kanan: transformasi "sesudah" yang mengagumkan
Tools: Canva split frame + AI generated "after"
```

**2. EXTREME CLOSEUP**
```
Zoom sangat dekat ke detail yang tidak biasanya terlihat
Prompt: macro photography, extreme close-up [subjek], hyper detailed, 8K
```

**3. IMPOSSIBLE SCENARIO**
```
Sesuatu yang tidak mungkin di dunia nyata tapi terlihat realistis
Contoh: "manusia berjalan di bawah air sambil minum kopi"
```

**4. UNEXPECTED PERSPECTIVE**
```
POV tidak biasa: worm's eye view, bird's eye, first person POV
Prompt: worm eye view, [subjek] dari bawah, wide angle distortion
```

**5. JUXTAPOSITION**
```
Dua hal yang kontras dalam satu frame
Contoh: mewah vs sederhana, modern vs tradisional, besar vs kecil
```

**6. TEXT-IN-IMAGE HOOK**
```
Teks yang terpasang di dalam gambar (DALL-E 3 paling baik untuk ini)
"Ini yang Terjadi Jika Kamu [action]" — teks langsung di gambar
```

**7. CINEMATIC ATMOSPHERE**
```
Film-like quality yang membuat orang berhenti
Prompt: cinematic photography, [scene], golden hour, anamorphic lens flare,
        film grain, shot on ARRI Alexa, professional color grading
```

**8. FACE CLOSE-UP WITH EMOTION**
```
Wajah manusia menarik atensi paling kuat (human face bias)
Ekspresi: shock, joy, confusion — emosi yang terstimulasi
```

**9. PATTERN INTERRUPT**
```
Sesuatu yang tidak sesuai ekspektasi viewer di bidang tersebut
Di feed yang penuh foto produk: tunjukkan orang nyata menggunakannya
```

**10. HYPER-REAL DETAIL**
```
Gambar yang terlalu sempurna sampai terlihat "unreal"
Prompt: hyperrealistic photography, [subjek], ultra high detail, 
        studio lighting, commercial photography style
```

---

## 💰 Cara Menghasilkan Uang dari AI Image & Video

### Model Bisnis Terbukti

| Model | Potensi/Bulan | Skill Level | Modal Awal |
|-------|--------------|-------------|-----------|
| Jual Midjourney Prompts | Rp 5-30 juta | Pemula | Rp 150rb |
| Stock Photo AI (Shutterstock/Adobe) | Rp 2-20 juta | Pemula | Rp 150rb |
| Custom AI Art untuk Klien | Rp 10-50 juta | Menengah | Rp 500rb |
| Print-on-Demand (Kaos, Poster) | Rp 5-30 juta | Pemula | Rp 0 |
| AI Video untuk Bisnis | Rp 20-100 juta | Menengah | Rp 1 juta |
| AI Content Agency | Rp 50-500 juta | Advanced | Rp 5 juta |
| Online Course tentang AI | Rp 30-200 juta | Menengah | Rp 2 juta |

→ Detail lengkap di [guides/13-monetization.md](guides/13-monetization.md)

---

## 📜 Lisensi

MIT © [azizaeffendi](https://github.com/azizaeffendi)

---

<div align="center">

**Muhammad Aziz A Effendi**
*Full-Stack Developer · AI Marketing Engineer · Indonesia*

[![GitHub](https://img.shields.io/badge/GitHub-@azizaeffendi-181717?style=flat-square&logo=github)](https://github.com/azizaeffendi)

Berikan ⭐ — ini gratis tapi butuh waktu untuk membuatnya berkualitas!

</div>