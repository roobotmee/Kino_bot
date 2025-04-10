# 🎬 Seen Kino Bot

📦 **Seen Kino Bot** — bu Telegram uchun mo‘ljallangan keng qamrovli kino bot bo‘lib, foydalanuvchilarga filmlarni kod orqali izlash, yuklab olish, baholash va tavsiyalar olish imkonini beradi. Adminlar esa filmlarni, kanallarni, foydalanuvchilarni boshqarishlari va statistikani kuzatishlari mumkin.

🔗 **Demo**: [@seen_kino_bot](https://t.me/seen_kino_bot)

---

## 🚀 Asosiy Funktsiyalar

### 👤 Foydalanuvchilar Uchun

- 🔍 **Film qidirish**: Nom yoki maxsus kod orqali izlash
- 🎯 **Film tavsiyalari**: Har kuni sizga film tavsiyalari
- ⭐ **Reyting tizimi**: Filmlarga baho berish va izoh yozish
- 🏆 **Eng yuqori baholangan filmlar**: Eng yaxshi filmlarni ko‘rish
- 🔗 **Oson ulashish**: Film linklarini do‘stlar bilan bo‘lishish

### 👨‍💼 Administratorlar Uchun

- 🎬 **Film boshqaruvi**: Film qo‘shish, tahrirlash, o‘chirish
- 🚫 **Foydalanuvchi boshqaruvi**: Bloklash / blokdan chiqarish, statistika ko‘rish
- 📢 **Kanal boshqaruvi**: Majburiy obuna uchun kanal ulash / ajratish
- 📬 **Xabar yuborish**: Hammani xabardor qilish
- 🔗 **Maxsus linklar**: Qo‘shimcha havolalarni boshqarish
- 📊 **Statistika**: Bot ishlash statistikasi
- 📝 **Matnlar sozlovi**: Bot javoblarini tahrirlash

---


📌 Majburiy Obuna va Zayavka Kanali
📣 Majburiy Kanalga Obuna
Botdan to‘liq foydalanish uchun foydalanuvchilar belgilangan kanallarga obuna bo‘lishlari majburiy. Admin panel orqali kanal linklarini ulash mumkin.

🔗 Kanal linklari data/links/ papkasida saqlanadi.

✅ Obuna tekshiruvi avtomatik tarzda amalga oshadi.

⛔ Obuna qilinmagan foydalanuvchilarga bot cheklov qo‘yadi.

📥 Zayavka (Join Request) Kanali
Bot foydalanuvchi kanalga a'zo bo‘lmagan taqdirda, unga zayavka havolasini yuboradi. Bu orqali foydalanuvchi "kanalga qo‘shilish" so‘rovini yuboradi.

📁 Zayavkalar data/zayavka/ papkasida saqlanadi.

🤖 Bot avtomatik tarzda foydalanuvchi Join Request yuborganligini aniqlaydi.

🔗 Kanalni ulash (adminlar uchun)
Admin panelga kiring: /panel yoki /admin

💬 "Kanallar" bo‘limiga o‘ting

Ulanmoqchi bo‘lgan kanal havolasini yuboring

Bot avtomatik tarzda havolani channels.txt va links/ papkalariga saqlaydi

💡 Eslatma: Kanalga adminlik huquqi berilgan bo‘lishi kerak, aks holda bot foydalanuvchini a’zo qila olmaydi va holatini tekshira olmaydi.


## 💬 Buyruqlar

| Buyruq | Tavsifi |
|--------|---------|
| `/start` | Botni boshlash va menyuni ko‘rish |
| `/rand` | Tasodifiy film olish |
| `/dev` | Dasturchi haqida |
| `/help` | Mavjud buyruqlar ro‘yxati |
| `/panel` yoki `/admin` | Admin panelga kirish (faqat adminlar uchun) |

---

## 🛠 Admin Panel Bo‘limlari

- 📊 Statistika
- 🎬 Film qo‘shish / 🗑️ Film o‘chirish
- 👨‍💼 Adminlar / 💬 Kanallar
- 🔴 Foydalanuvchini bloklash / 🟢 Blokdan chiqarish
- ✍️ Xabar yuborish / 📬 Xabar forward qilish
- 🤖 Bot holati / 📝 Matn sozlamalari

---

## 🧩 Texnik Tafsilotlar

### 🗄 Ma'lumotlar Bazasi (SQLite)

- `user_id`: Foydalanuvchi ma'lumotlari va status
- `data`: Film ma'lumotlari
- `settings`: Bot konfiguratsiyasi
- `texts`: Moslashtirilgan javoblar

### 📁 Katalog Struktura

```plaintext
data/
├── links/         # Kanal havolalari
├── zayavka/       # Obuna so‘rovlari
├── requests/      # Foydalanuvchi so‘rovlari
├── ratings/       # Film reytinglari
├── user_views/    # Foydalanuvchi ko‘rgan filmlar
├── additional.txt # Qo‘shimcha havolalar
├── users.txt      # Foydalanuvchilar ro‘yxati
├── admins.txt     # Adminlar ro‘yxati
├── channels.txt   # Kanal ro‘yxati
└── ...            # Boshqa sozlamalar
🔄 Holat Boshqaruvi (FSM)
Bot FSM (Finite State Machine) yordamida foydalanuvchi amallarini boshqaradi:

Film qo‘shish

Matnlar tahriri

Kanallar boshqaruvi

🧰 O‘rnatish va Ishga Tushirish
📋 Talablar
Python 3.7+

aiogram

sqlite3

psutil

⚙️ Sozlash
Repozitoriyani klonlang

Kutubxonalarni o‘rnating:

bash
Copy
Edit
pip install -r requirements.txt
bot.py faylida bot tokenini kiriting

Admin ID’ni belgilang

Botni ishga tushiring:

bash
Copy
Edit
python bot.py
🔐 Xavfsizlik
✅ Majburiy kanalga obuna

🔑 Admin autentifikatsiyasi

🚫 Foydalanuvchilarni bloklash

📴 Botni yoqish/o‘chirish imkoniyati

👨‍💻 Dasturchi
Bot muallifi: @RooBotmee
Agar sizga shunday yoki boshqa turdagi Telegram bot kerak bo‘lsa, murojat qiling.

📢 Dasturchi kanali: @CodeIsmoilov
