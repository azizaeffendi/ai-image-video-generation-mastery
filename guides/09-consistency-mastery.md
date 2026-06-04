# 🔑 Teknik Konsistensi — Karakter, Style & Brand

## Mengapa Konsistensi itu Kritis

```
BRAND YANG TIDAK KONSISTEN:       BRAND YANG KONSISTEN:
Random style tiap post             Langsung dikenali tanpa nama
Karakter berbeda-beda             Karakter yang terasa "hidup"
Tidak ada brand recognition       Audience merasa kenal = lebih percaya
Hard to stand out                 Instantly recognizable
```

---

## METODE 1: Character Reference (Midjourney --cref)

### Full Workflow Step-by-Step

**FASE 1: Buat Character Bible**
```
Tujuan: 8-12 gambar master karakter dari berbagai angle

Generate dengan prompt:
"[deskripsi karakter lengkap], character reference sheet, 
multiple angles, front view, side view, 3/4 view, 
white background, consistent lighting --ar 16:9 --style raw"

Simpan URL gambar terbaik sebagai "master reference"
```

**FASE 2: Develop Situational Variations**
```
Variasi yang perlu dibuat:
□ Expression sheet: happy, serious, thinking, surprised
□ Outfit variations: casual, formal, sporty
□ Environment variations: office, outdoor, home, urban
□ Activity variations: working, presenting, talking, walking

Template:
/imagine [karakter] [ekspresi/outfit/environment]
--cref [URL master] --cw [75] --v 6.1 --style raw
```

**FASE 3: Build Asset Library**
```
Organisasikan di folder:
/character-assets/
  /master-sheets/          → Reference utama
  /expressions/            → 10+ ekspresi berbeda
  /outfits/                → 5+ outfit variations
  /environments/           → 10+ background settings
  /poses/                  → 15+ pose variations
  /combined/               → Ready-to-post combinations
```

---

## METODE 2: LoRA di Stable Diffusion (Paling Powerful)

### Apa itu LoRA?
```
LoRA = Low-Rank Adaptation
Bayangkan seperti "addon" yang melatih AI untuk mengenali
karakter/style/objek SPESIFIK milik Anda.

Setelah ditraining: Karakter/style bisa muncul persis sama
di ribuan gambar berbeda dengan zero effort per gambar.
```

### Training LoRA — Step by Step

**STEP 1: Persiapkan Dataset**
```
Kumpulkan 15-30 foto reference:
- Variasi pose, angle, ekspresi
- Background berbeda (bukan semua sama)
- Lighting berbeda
- Resolusi minimal 512x512, ideal 1024x1024

UNTUK KARAKTER ORANG:
- Foto wajah closeup: 10+ foto
- Full body: 5+ foto
- 3/4 angle: 5+ foto
- Pastikan wajah jelas dan tidak blur

UNTUK STYLE/OBJECT:
- Tangkap elemen kunci yang membedakan style
- Minimal 20 gambar dengan variasi konteks
```

**STEP 2: Training di Google Colab (Gratis)**
```
1. Buka: github.com/kohya-ss/sd-scripts (Kohya LoRA Trainer)
2. Gunakan Colab notebook yang sudah disiapkan komunitas
3. Upload dataset Anda
4. Set parameter training:
   - Steps: 1000-2000 untuk karakter, 500-1000 untuk style
   - Learning rate: 1e-4 (default, aman)
   - Batch size: 1-2 (sesuai VRAM Colab)
5. Training ~30-60 menit di Colab
6. Download file .safetensors
```

**STEP 3: Gunakan LoRA**
```
Di ComfyUI atau Automatic1111:
<lora:nama_lora_anda:0.8>

Contoh prompt:
a photo of [trigger word] woman, professional headshot, 
studio lighting <lora:my_character_lora:0.8>

Angka 0.8 = strength (0.5-1.0 biasanya optimal)
```

---

## METODE 3: Style Consistency System

### Brand Visual System dengan AI

```
KOMPONEN BRAND VISUAL YANG PERLU DIKONSISTENSIKAN:

1. COLOR PALETTE
   → Tentukan 3-5 warna brand
   → Masukkan hex code ke setiap prompt: "color palette: #F4A261 #E76F51 #2A9D8F"

2. LIGHTING STYLE
   → Pilih 1-2 jenis lighting yang jadi signature
   → Contoh: "always soft natural window lighting, slightly warm" 
   → Simpan sebagai template yang selalu ditambahkan

3. PHOTOGRAPHY STYLE
   → Tentukan: cinematic / editorial / documentary / clean commercial
   → Masukkan ke setiap prompt sebagai konstanta

4. MOOD/ATMOSPHERE
   → "Warm, optimistic, professional yet approachable"
   → Terjemahkan ke kata-kata visual yang konsisten

5. FRAMING PREFERENCE
   → Portrait? Landscape? Rule of thirds?
   → Aspect ratio yang konsisten per platform
```

### Style Lock Template
```
Buat "Style Constant" yang selalu ditambahkan ke setiap prompt:

STYLE CONSTANT TEMPLATE:
[Your specific style words], [your lighting preference], 
[your color aesthetic], [your photography style], 
[your mood], [your camera reference]
--ar [your ratio] --style raw --sref [your style reference URLs]

Simpan ini sebagai shortcut atau Midjourney /prefer
```

---

## METODE 4: AI Brand Photography System

### Konsep: Satu Model untuk Semua Kebutuhan

```
TRADISIONAL:
Foto produk → Sewa fotografer → Sewa model → Studio → Editing
Biaya: Rp 5-30 juta per sesi
Waktu: 1-2 minggu

DENGAN AI:
Buat AI model brand Anda → Generate ratusan foto → Konsisten 100%
Biaya: $10-50/bulan
Waktu: 1-2 jam
```

### Workflow Lengkap

```
HARI 1: Foundation
□ Buat master AI model (Midjourney atau Leonardo)
□ Generate 20+ foto untuk berbagai situasi
□ Buat style reference collection

HARI 2: Content Library
□ Generate 50+ foto dengan konsistensi terjaga
□ Kategorisasi: produk, lifestyle, portrait, action

MINGGUAN: Content Production
□ Generate batch 20-30 gambar baru per minggu
□ Post jadwal: 2-3 konten/hari dari library
□ Total: 60-90 konten/bulan dari $10-30 cost
```

---

## TROUBLESHOOTING KONSISTENSI

### Masalah & Solusi

| Masalah | Kemungkinan Penyebab | Solusi |
|---------|---------------------|--------|
| Wajah berubah setiap generate | Tidak pakai --cref | Tambahkan --cref URL + --cw 75-85 |
| Style terlalu bervariasi | Prompt tidak konsisten | Buat style constant template |
| Background tidak konsisten | Tidak spesifik | Describe background dengan detail |
| Kualitas tidak stabil | --q tidak diset | Tambahkan --q 2 |
| Terlalu random | --chaos terlalu tinggi | Kurangi --chaos atau set ke 0 |
| Tidak bisa reproduce | Tidak catat seed | Catat --seed dari gambar yang bagus |