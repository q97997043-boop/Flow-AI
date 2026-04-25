<div align="center">

***FLOW AI***

**AI-powered ATM Cash Forecasting & Monitoring Platform**

[![HTML5](https://img.shields.io/badge/HTML5-only-E34F26?style=flat-square&logo=html5&logoColor=white)](.)
[![AI](https://img.shields.io/badge/AI-Gemini%20%7C%20Claude-4285F4?style=flat-square&logo=google&logoColor=white)](.)
[![Maps](https://img.shields.io/badge/Maps-Leaflet.js-199900?style=flat-square&logo=leaflet&logoColor=white)](.)
[![License](https://img.shields.io/badge/License-MIT-00E5C3?style=flat-square)](LICENSE)
[![Mobile](https://img.shields.io/badge/Mobile-Ready-success?style=flat-square)](.)

*O'zbekiston banklaridagi ATMlarning naqd pul holatini real vaqtda kuzatish va AI yordamida bashorat qilish tizimi.*

</div>

---

## Nima qiladi?

Har kuni **340,000+** odam O'zbekistondagi bankomatlarga borib, naqd pul topa olmay qaytadi. ALGORX bu muammoni bartaraf etish uchun yaratilgan:

- 🔮 **7 kunlik AI bashorat** — qaysi bankomat qachon tugashini oldindan bilasiz
- 🗺️ **Real-time xarita** — barcha ATM holati bir ekranda
- 📊 **Tranzaksiya tahlili** — haftalik va soatlik yuklanish naqshlari
- 🛣️ **Inkassatsiya optimizatsiyasi** — AI marshrut tartibini o'zi tuzadi
- 🤖 **AI chat** — o'zbek tilida savol-javob

---

## Tez boshlash

> **Hech qanday o'rnatish kerak emas.** Faqat faylni brauzerda oching.

```bash
git clone https://github.com/username/algorx.git
cd algorx

# Oddiy usul
open algorx-final.html

# Yoki lokal server (AI API uchun tavsiya etiladi)
python3 -m http.server 8080
# → http://localhost:8080/algorx-final.html
```

**Demo kirish:**
```
Email : admin@bank.uz
Parol : 12345678
```

---

## AI Ulash

ALGORX ikkita AI provayderni qo'llab-quvvatlaydi. Chat panelidagi **⚙️** tugmasini bosib ulang:

| Provayder | Narx | Key format | Olish joyi |
|---|---|---|---|
| 🔵 Google Gemini Flash | **Bepul** | `AIza...` | [aistudio.google.com/apikey](https://aistudio.google.com/apikey) |
| 🟠 Anthropic Claude | $5 kredit | `sk-ant-...` | [console.anthropic.com/keys](https://console.anthropic.com/keys) |

Key formatiga qarab tizim **avtomatik** provayderini tanib oladi.

---

## Fayl tuzilmasi

```
algorx/
├── algorx-final.html           ← Admin dashboard (barcha funksiyalar)
├── uzbekistan-atm-map.html     ← Ommaviy mijozlar xaritasi
├── algorx-prezentatsiya.html   ← Investor pitch qo'llanmasi
└── README.md
```

---

## Dashboard panellari

| Panel | Tavsif |
|---|---|
| 🏠 **Dashboard** | Xarita, statistika, AI insights, ogohlantirishlar |
| 🗺️ **Xarita** | ATM markerlar, Google Maps / Yandex navigatsiya |
| 📋 **ATM Ro'yxati** | Filtr, qidiruv, ko'rish, xaritaga o'tish |
| 📈 **Bashorat** | 7/14/30 kunlik grafik, inkassatsiya kalendari, AI tahlil |
| 📊 **Hisobotlar** | Oylik tahlil, PDF print, CSV export |
| 🔔 **Ogohlantirishlar** | Kritik holatlar, hal qilish tugmasi |
| ⚙️ **Sozlamalar** | Chegaralar, bildirishnomalar, foydalanuvchilar |

### Per-ATM Analytics Panel

Xaritada har qanday markerni bosing → o'ngdan panel slayd bilan chiqadi:

```
📈 Bashorat   →  7 kunlik naqd pul kamayishi + kritik sana belgilanadi
📅 Haftalik   →  Eng yuqori tranzaksiya kuni yashil bilan ta'kidlanadi
🕐 Soatlik    →  Band soatlar, "shu vaqtda inkassatsiya qilinmasin" tavsiyasi
```

ATM turi (bozor · metro · aeroport · filial) ga qarab **har xil profil** yaratiladi.

---

## Texnologiyalar

```
Frontend   →  Vanilla HTML / CSS / JavaScript  (zero build, zero npm)
Xarita     →  Leaflet.js 1.9.4  +  CartoDB Voyager tiles
Grafiklar  →  Chart.js 4.4.1
AI         →  Google Gemini Flash 2.0  /  Anthropic Claude Sonnet 4
Shriftlar  →  Syne · DM Sans · IBM Plex Mono  (Google Fonts)
```

---

## Mobil qurilmalar

To'liq responsive — telefon va planshetlarda ishlaydi:

| Element | Mobil ko'rinish |
|---|---|
| Navigatsiya | Pastki bottom nav bar (5 tugma) |
| Sidebar | Hamburger `☰` → slayd menyu |
| Analytics panel | Pastdan bottom sheet |
| AI Chat | To'liq ekran |
| Statistika kartalar | 2 ustunli grid |

---

## Xavfsizlik

API key **localStorage** da faqat brauzeringizda saqlanadi — hech qanday serverga yuborilmaydi.

```gitignore
# .gitignore
.env
config.local.js
```

> Production muhiti uchun API keyni backend proxy orqali yuborishni tavsiya etamiz.

---

## Hissa qo'shish

PR va Issuelar doimo xush kelibsiz:

```bash
git checkout -b feature/yangi-funksiya
git commit -m "feat: yangi funksiya qo'shildi"
git push origin feature/yangi-funksiya
```

---

## Litsenziya

[MIT](LICENSE) · © 2025 ALGORX

---

<div align="center">

**O'zbekiston bank sektori uchun 🇺🇿**

[Issues](../../issues) · [Discussions](../../discussions)

</div>
