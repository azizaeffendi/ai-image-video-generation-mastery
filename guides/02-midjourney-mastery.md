# 🔵 Midjourney v6 — Panduan Lengkap dari Nol ke Master

## Setup Awal

### 1. Cara Akses Midjourney
```
1. Buka discord.com dan buat akun (gratis)
2. Pergi ke midjourney.com → klik "Join the Beta"
3. Pilih plan: Basic ($10) / Standard ($30) / Pro ($60) / Mega ($120)
4. Mulai generate di server Discord atau di midjourney.com/imagine (web UI)
```

### 2. Perintah Dasar
```
/imagine     → Generate gambar dari prompt
/describe    → Upload gambar, Midjourney analisis dan buat promptnya
/blend       → Gabungkan 2-5 gambar
/info        → Cek status akun dan penggunaan GPU
/prefer      → Set preferensi default (mis: selalu pakai --v 6.1)
/settings    → Ubah setting default
```

---

## PROMPT ANATOMY — Formula Lengkap

```
[SUBJEK] + [DETAIL SUBJEK] + [AKSI/POSE] + [ENVIRONMENT/LATAR] + 
[LIGHTING] + [MOOD/ATMOSPHERE] + [PHOTOGRAPHY/ART STYLE] + 
[CAMERA & LENS] + [PARAMETERS]
```

### Contoh Breakdown Prompt Profesional

**SALAH (terlalu singkat):**
```
/imagine indonesian woman professional
```

**BENAR (detail dan komprehensif):**
```
/imagine young Indonesian businesswoman, 28 years old, confident expression,
wearing smart casual blazer, working on laptop, modern co-working space in Jakarta,
floor-to-ceiling windows with city view, warm afternoon golden hour lighting,
professional corporate photography style, candid moment, shot on Canon EOS R5,
85mm f/1.4 lens, shallow depth of field, warm color grading --ar 4:5 --v 6.1 --style raw --q 2
```

---

## PARAMETER MASTERCLASS

### Aspect Ratio (--ar)
```
--ar 1:1      → Square (Instagram feed, profile picture)
--ar 4:5      → Portrait (Instagram feed optimal)
--ar 9:16     → Vertical (Stories, TikTok, Reels)
--ar 16:9     → Landscape (YouTube thumbnail, banner)
--ar 3:2      → Photo standard
--ar 21:9     → Cinematic ultrawide
--ar 2:3      → Portrait print
```

### Style Parameters
```
--style raw          → Lebih realistis, kurang "artistic AI look"
--style cute         → Softer, more kawaii
--stylize 0          → Sangat literal mengikuti prompt
--stylize 100        → Default Midjourney (balanced)
--stylize 750        → Lebih artistic, lebih interpretasi
--stylize 1000       → Paling artistic, paling jauh dari prompt
```

### Consistency Parameters — KUNCI KONSISTENSI
```
--seed [0-4294967295]  → Angka seed mengunci "DNA" gambar
                         Prompt sama + seed sama = hasil sangat mirip
                         Cara cari seed: reaksi ✉️ ke gambar Midjourney

--cref [image URL]     → Character Reference — pertahankan wajah/karakter
--cw [0-100]           → Character Weight
                         0  = hanya pakai style dari reference
                         50 = balanced (RECOMMENDED)
                         100 = sangat mirip reference (mungkin kaku)

--sref [image URL]     → Style Reference — tiru gaya visual
--sw [0-1000]          → Style Weight (default 100)
```

---

## 200 PROMPT TEMPLATES TERKATEGORISASI

### 📸 PORTRAIT & PEOPLE

**1. Professional Business Portrait**
```
[gender] Indonesian professional, [age] years old, warm genuine smile,
wearing [outfit], [background environment], professional studio lighting,
corporate headshot style, shot on Phase One IQ4 150MP, --ar 4:5 --style raw --v 6.1
```

**2. Lifestyle Content Creator**
```
young Indonesian content creator, authentic candid moment, [activity],
[environment], natural soft lighting, UGC-style photography, iPhone-quality feel,
relatable and approachable, warm color grading --ar 9:16 --style raw
```

**3. AI Influencer / Brand Ambassador**
```
photorealistic AI model, [ethnicity] features, [age], [expression],
wearing [brand style], [location], magazine editorial photography,
Vogue-quality lighting, ultra detailed, 8K resolution --ar 4:5 --style raw --q 2
```

**4. Before & After Transformation**
```
BEFORE: tired looking [person], dull skin, casual outfit, poor lighting
AFTER: glowing confident [person], radiant skin, stylish outfit, studio lighting
split image composition, transformation comparison --ar 16:9
```

### 🏢 PRODUCT & COMMERCIAL

**5. Product Hero Shot**
```
[product name and description], floating in air, clean white studio background,
dramatic side lighting with subtle shadow, commercial product photography,
shot on Hasselblad, ultra detailed, reflective surface --ar 1:1 --style raw
```

**6. Product in Lifestyle Context**
```
[product] being used by [person description] in [lifestyle setting],
natural candid moment, lifestyle photography, warm inviting atmosphere,
soft natural window lighting, Instagram-worthy aesthetic --ar 4:5
```

**7. Food Photography**
```
[dish name], overhead flat lay, rustic wooden table surface, fresh ingredients scattered,
natural window light from left, food styling, warm inviting tones,
shot on Canon 5D Mark IV, 50mm lens, f/2.8, restaurant quality --ar 1:1
```

**8. Fashion & E-Commerce**
```
[clothing item] on [body type] model, clean minimal background, full body shot,
even studio lighting, sharp focus on clothing details, e-commerce product photography,
white seamless background --ar 3:4 --style raw
```

### 🌆 ENVIRONMENT & BACKGROUND

**9. Modern Jakarta Cityscape**
```
modern Jakarta skyline at golden hour, SCBD business district, glass skyscrapers,
warm orange glow, slight haze, cinematic wide shot, shot on DJI Mavic 3,
aerial photography, Instagram-worthy --ar 16:9
```

**10. Cozy Indonesian Café**
```
cozy specialty coffee shop interior, Jakarta aesthetic, exposed brick walls,
rattan furniture, tropical plants, warm Edison bulb lighting, bohemian modern style,
wide angle interior photography, inviting atmosphere --ar 16:9 --style raw
```

### 🎨 ARTISTIC & CREATIVE

**11. Digital Illustration Style**
```
[scene/character], digital illustration style, [color palette], 
detailed character design, Behance portfolio quality, 
professional concept art, inspired by [artist/style] --ar 4:5
```

**12. Cinematic Movie Poster**
```
movie poster composition, [main character/scene], dramatic lighting,
cinematic color grading, epic atmosphere, Hollywood blockbuster style,
strong visual hierarchy, text placeholder area at bottom --ar 2:3
```

### 🤖 AI & TECH VISUALS

**13. AI Technology Abstract**
```
abstract representation of artificial intelligence, neural network visualization,
glowing blue data streams, futuristic tech aesthetic, dark background,
sci-fi concept art, high contrast, neon accents --ar 16:9
```

**14. Futuristic Business**
```
futuristic business professional, holographic interface, data visualization,
corporate tech environment, blue purple color palette, 
clean minimal aesthetic, concept art --ar 16:9
```

---

## TEKNIK ADVANCED

### Character Consistency Workflow (Step by Step)

```
STEP 1 — Buat Master Character
/imagine [deskripsi karakter detail] --ar 1:1 --style raw --v 6.1

STEP 2 — Pilih gambar terbaik
Klik U1/U2/U3/U4 untuk upscale gambar yang dipilih

STEP 3 — Copy URL gambar
Klik gambar → Open in browser → Copy URL

STEP 4 — Pakai sebagai reference
/imagine [karakter] [situasi baru] --cref [URL step 3] --cw 75

STEP 5 — Buat berbagai pose dan situasi
Gunakan URL yang sama untuk semua variasi
Karakter akan tetap konsisten!

CONTOH WORKFLOW:
Pertemuan 1: Create master character sheet (5-8 gambar dari berbagai angle)
Pertemuan 2+: Semua konten menggunakan --cref dari master sheet
```

### Style Transfer untuk Brand

```
TUJUAN: Semua konten punya "look and feel" yang sama

STEP 1: Kumpulkan 5 gambar yang represent visual brand Anda
STEP 2: Upload semua ke imgur atau hosting gambar
STEP 3: Buat "style reference prompt":
/imagine [konten baru] --sref [URL1] [URL2] [URL3] [URL4] [URL5] --sw 200

TIPS:
- Semakin banyak reference, semakin kuat style lock
- --sw 200-400 biasanya sweet spot
- Kombinasikan dengan --style raw untuk hasil lebih natural
```

---

## NEGATIVE PROMPTS — Apa yang Harus Dihindari

```
--no watermark, text, signature, logo, ugly, distorted, blurry, low quality,
bad anatomy, extra limbs, deformed hands, weird fingers, out of frame,
duplicate, multiple people (jika mau 1 orang), background people, 
amateur photography, grain, noise, overexposed, underexposed
```

---

## TIPS PRO YANG JARANG DIAJARKAN

### 1. Paraphrase dengan ChatGPT
```
Sebelum prompt ke Midjourney, minta ChatGPT:
"Improve this Midjourney prompt for maximum quality and photorealism:
[prompt Anda]"
```

### 2. Gunakan Real Camera & Lens Names
```
"Shot on Sony A7R V" → lebih baik dari "high quality camera"
"85mm f/1.4 lens" → depth of field yang jelas
"ISO 100, f/8, 1/250s" → kontrol exposure yang akurat
```

### 3. Reference Real Photographers
```
"Photography style of Annie Leibovitz" → portrait yang powerful
"Inspired by Steve McCurry" → photojournalism yang emosional
"Architecture photography like Iwan Baan" → building shots yang menawan
```

### 4. Color Palette Spesifik
```
Jangan: "warm colors"
Terbaik: "warm amber tones, #F4A261 and #E76F51 color palette, sunset warmth"
```

### 5. Lighting yang Presisi
```
"Rembrandt lighting" → dramatic portrait lighting
"Butterfly lighting" → beauty/fashion lighting
"Golden hour lighting" → warm outdoor
"Overcast soft diffused lighting" → flat, even exposure
"Backlit silhouette" → dramatic effect
```