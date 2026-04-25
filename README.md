# ATM Flow AI 🏧

**Aqlli bankomat monitoring va inkassatsiya marshrut tizimi**

O'zbekiston banklari uchun maxsus ishlab chiqilgan. Bankomatlarning naqd pul holatini real vaqtda kuzatib, inkassatorlar uchun optimal marshrutni avtomatik tuzadi.

---

## Nima qiladi?

| Funksiya | Tavsif |
|---|---|
| 🔴 Real-time monitoring | 18 bankomat holatini kuzatadi |
| 🧠 Aqlli marshrut | 1 kun qolgan ATM + 5km ichidagi ATMlarni birga rejalashtiradi |
| 📏 Masofa hisoblash | Har ikki nuqta orasidagi km va haydash vaqti |
| 📅 Dam olish bashorati | Shanba-Yakshanba uchun +25–50% qo'shimcha pul |
| 📱 QR kod | Google Maps navigatsiyasi uchun |
| 🗺 Interaktiv xarita | Rangli markerlar + ketma-ketlik chiziq |
| 🤖 AI chat | Gemini (bepul) yoki Claude bilan |
| 📊 Grafiklar | 7 kunlik bashorat va tahlillar |

---

## Marshrut algoritmi

```
1. Eng urgent ATM (≤1 kun qolgan) → bosh nuqta
2. Unda 5km ichida ≤4 kun qolgan ATMlar → qo'shiladi
3. Agar 4 ta to'lmasa → radius kengaytiriladi
4. Nearest-Neighbor TSP → optimal ketma-ketlik
5. Bank → A → B → C → D → Bank
6. Har leg: masofa (km) + vaqt (min)
```

---

## Ishga tushirish

```bash
# O'rnatish kerak emas
open atmflow-final.html
```

**Demo:** `admin@bank.uz` / `12345678`

**AI Chat uchun (ixtiyoriy):** ⚙️ tugmasi → [aistudio.google.com/apikey](https://aistudio.google.com/apikey) → bepul key

---

## Texnologiyalar

Vanilla HTML/CSS/JS · Leaflet.js · Chart.js · QRCode.js · Haversine formula · Nearest-Neighbor TSP

---

MIT © 2025 ATM Flow AI
