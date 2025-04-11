# 🎬 Kino Bot - Telegram uchun aqlli kino bot

📦 **Kino Bot** — bu Telegram foydalanuvchilari uchun kinolarni izlash, ko‘rish, baholash va tavsiya olish imkonini beruvchi aqlli botdir. Bot **Python** va **Aiogram 3.x** asosida yozilgan bo‘lib, foydalanuvchi va adminlar uchun qulay interfeysga ega.

---

## 📌 Umumiy ma'lumot

Kino Bot sizga quyidagilarni taklif qiladi:
- 🔍 Kino qidirish (nom yoki maxsus kod orqali)
- 🎯 Kunlik tavsiyalar
- ⭐ Reyting asosida eng yaxshi filmlarni ko‘rish
- 📝 Izoh yozish va ulashish
- 👨‍💼 Adminlar uchun kuchli boshqaruv paneli

---

## 🌟 Asosiy imkoniyatlar

### 👤 Foydalanuvchilar uchun
- 🔍 Kino qidirish (nom yoki kod bo‘yicha)
- 🎲 Tasodifiy kino olish
- ⭐ Baholash va izoh yozish
- 📊 Reytinglar asosida kino topish
- 📎 Kino linklarini do‘stlar bilan ulashish

### 👨‍💼 Adminlar uchun
- 🎬 Film qo‘shish, o‘chirish, tahrirlash
- ⛔ Foydalanuvchini bloklash / 🔓 Blokdan chiqarish
- 📢 Reklama va umumiy xabar yuborish
- 📊 Bot statistikasi
- 📌 Kanalga majburiy obuna sozlamalari
- 📝 Matnlarni sozlash

---

## 🛠 Texnik jihatlar

### 📚 Texnologiyalar

| Komponent            | Texnologiya      |
|----------------------|------------------|
| Dasturlash tili      | Python 3.10+      |
| Framework            | Aiogram 3.x       |
| Ma'lumotlar bazasi   | SQLite 3          |
| Hosting              | Linux server      |

### 📦 Kutubxonalar

aiogram==3.0.0b7
sqlite3
asyncio
logging
python-dotenv
🏗 Loyihaning tuzilishi
bash
Copy
Edit
├── main.py
├── config.py
├── database/
│   ├── db_engine.py
│   ├── models.py
├── handlers/
│   ├── start.py
│   ├── search.py
│   ├── admin.py
├── keyboards/
│   ├── inline.py
│   ├── reply.py
├── utils/
│   ├── helpers.py
│   ├── logger.py
├── .env
💻 Foydalanuvchi interfeysi
🚀 Boshlang'ich xabar
python
Copy
Edit
🎬 *Assalomu alaykum, {user_name}!* 🤖

✨ *KinoBotga xush kelibsiz!* Kinolar dunyosiga sayohatga tayyormisiz?

Quyidagi imkoniyatlardan foydalaning:
🔍 *Kino qidirish* - Nom yoki kod bo'yicha izlash
🎲 *Tasodifiy kino* - Kunlik tavsiya
⭐ *Top reyting* - Eng yaxshi baholangan filmlar
📚 *Yo'riqnoma* - Botdan foydalanish qo'llanmasi

📌 *Eslatma:* Botdan to'liq foydalanish uchun quyidagi kanalga a'zo bo'ling: @kino_kanal
⌨️ Inline tugmalar
python
Copy
Edit
keyboard = InlineKeyboardMarkup(row_width=2)
buttons = [
    InlineKeyboardButton("🔍 Kino qidirish", callback_data="search"),
    InlineKeyboardButton("🎲 Tasodifiy", callback_data="random"),
    InlineKeyboardButton("⭐ Top 10", callback_data="top10"),
    InlineKeyboardButton("📊 Mening statistikam", callback_data="mystats")
]
keyboard.add(*buttons)
⚙️ Admin paneli
🛡 Buyruqlar
/admin – Admin panelga kirish

/panel – Asosiy boshqaruv oynasi

/dashboard – Statistik va sozlamalar

📋 Admin imkoniyatlari
➕ Kino qo‘shish

➖ Kino o‘chirish

✏️ Kino tahrirlash

👥 Foydalanuvchilar ro‘yxati

⛔ Bloklash / 🔓 Blokdan chiqarish

📢 Xabar yuborish

📊 Statistika ko‘rish

⚙️ Sozlamalarni boshqarish

🗃️ Ma'lumotlar bazasi
users jadvali
Maydon	Tavsifi
UID	Foydalanuvchi ID
Telegram ID	Telegramdagi ID
Ism	Foydalanuvchi ismi
Familiya	Foydalanuvchi familiyasi
Yaratilgan sana	Ro‘yxatdan o‘tgan vaqt
Oxirgi faollik	Oxirgi ishlatgan vaqt
Status	Foydalanuvchi holati
movies jadvali
Maydon	Tavsifi
ID	Kino ID
Kino kodi	Maxsus kod
Nomi	Kino nomi
Tavsifi	Kino haqida izoh
Reyting	Foydalanuvchilar bahosi
Yuklangan sana	Qo‘shilgan sana
ratings jadvali
Maydon	Tavsifi
ID	Baholash ID
Foydalanuvchi	Kim baholadi
Kino ID	Qaysi kinoga
Baho	Berilgan baho
Sharh	Izoh
Sana	Baholash vaqti
🔒 Xavfsizlik tizimi
✅ Kanalga majburiy a’zolik

🔑 Admin autentifikatsiyasi

🚫 Foydalanuvchi cheklovlari

🕵️ Harakat monitoringi

🧩 Parol va IP cheklovlar

🛡 SHA-256 bilan shifrlash

💾 Muntazam backup

🔐 SQL injectiondan himoya

📊 Statistika tizimi
python
Copy
Edit
stats = {
    "users": {
        "total": 1245,
        "active": 876,
        "new_today": 42
    },
    "movies": {
        "total": 567,
        "views_today": 1234,
        "top_movie": {"id": 12, "title": "Interstellar", "views": 256}
    },
    "system": {
        "uptime": "4d 12h 23m",
        "load": "34%"
    }
}
🚀 Qo‘shimcha funksiyalar
🔎 Aqlli qidiruv
Xatoliklarni tuzatish

Sinonimlarni aniqlash

Avtoto‘ldirish imkoniyati

🎭 Shaxsiy tavsiyalar
Ko‘rilgan kinolarga qarab

Baholar asosida

Do‘stlar faoliyati asosida

📅 Voqealar taqvimi
Yangi chiqqan kinolar

Maxsus premyeralar

Kino tanlovlari

🔗 Muhim havolalar
👨‍💻 Dasturchi: @roobotmee

🌐 Vebsayt: roobotmee.uz

🤖 Demo Bot: @seen_kino_bot

📜 Litsenziya
MIT Litsenziyasi — batafsil LICENSE.md faylida.

💡 Rivojlanish rejasi
✅ Asosiy funksiyalar

✅ Admin panel

🔄 Multi-til qo‘llab-quvvatlash

🔄 Playlistlar

🔄 Telegram WebApp integratsiyasi

🎉 Kino Bot — har kuni yangi filmlar va qulay interfeys bilan sizni kutmoqda!

go
Copy
Edit

Agar istasang, bu faylni `.md` formatida tayyorlab ham bera olaman — yoki GitHub sahifangga qo‘yish bo‘yich
