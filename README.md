# 🤖 DeepAI Telegram Bot

بوت تيليجرام للدردشة مع الذكاء الاصطناعي باستخدام DeepAI API، مع دعم كامل للغة العربية وسجل محادثات لكل مستخدم.

## ✨ المميزات
- 💬 محادثة ذكية مع الذكاء الاصطناعي
- 🧠 حفظ سجل المحادثة لكل مستخدم على حدة
- 🌍 دعم اللغة العربية في الواجهة
- 🖼️ يدعم توليد الصور وتحريرها (عبر DeepAI Tools)
- ⚡ ردود فورية مع مؤشر "جاري الكتابة"
- 📜 أوامر للتحكم الكامل: `/clear` و `/history`

## 🚀 التثبيت والتشغيل

### 1. استنساخ المشروع
\`\`\`bash
git clone https://github.com/YOUR_USERNAME/deepai-telegram-bot.git
cd deepai-telegram-bot
\`\`\`

### 2. إنشاء بيئة افتراضية
\`\`\`bash
python3 -m venv venv
source venv/bin/activate  # Linux/Mac
# أو
venv\\Scripts\\activate   # Windows
\`\`\`

### 3. تثبيت المكتبات
\`\`\`bash
pip install -r requirements.txt
\`\`\`

### 4. إعداد المتغيرات
انسخ `.env.example` إلى `.env` وعدّل القيم:
\`\`\`bash
cp .env.example .env
nano .env
\`\`\`

- `TELEGRAM_BOT_TOKEN`: احصل عليه من [@BotFather](https://t.me/BotFather)
- `DEEPAI_API_KEY`: مفتاح DeepAI (موجود افتراضياً في المشروع)

### 5. تشغيل البوت
\`\`\`bash
python bot.py
\`\`\`

## 📌 الأوامر
| الأمر | الوصف |
|------|-------|
| `/start` | بدء المحادثة |
| `/help` | عرض المساعدة |
| `/clear` | مسح سجل المحادثة |
| `/history` | عرض آخر 10 رسائل |

## 🐳 النشر باستخدام Docker (اختياري)
\`\`\`bash
docker build -t deepai-bot .
docker run -d --env-file .env --name deepai-bot deepai-bot
\`\`\`

## ☁️ النشر على Railway / Render
1. ارفع المشروع على GitHub.
2. اربط المستودع مع Railway أو Render.
3. أضف متغيرات البيئة من لوحة التحكم.
4. سيتم تشغيل البوت تلقائياً.

## ⚠️ تنبيه
هذا المشروع يستخدم API غير رسمي من DeepAI. قد يتوقف عن العمل في أي وقت إذا قامت الشركة بتغيير سياساتها.

## 📄 الترخيص
MIT License
