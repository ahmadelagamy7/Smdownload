
# Telegram Video Bot (Render)

هذا المشروع بوت تيليجرام بسيط ينزّل فيديوهات من روابط عامة (يوتيوب/إنستجرام/فيسبوك/X/تيك توك/بينترست/ريديت) ويرسلها في المحادثة.

**مهم:** يعمل على حد الحجم الافتراضي 50MB الخاص بـ Bot API. يمكن تغيير الحد عبر المتغيّر `MAX_MB`.

## الإعداد
1) أنشئ بوت من @BotFather وخذ `BOT_TOKEN`.
2) ارفع الملفات إلى GitHub Repo (مثلاً `telegram-video-bot`).

## النشر على Render
1) أنشئ خدمة جديدة: New → Web Service.
2) اربط الريبو من GitHub.
3) اختر Environment = Python.
4) ضع الأوامر:
   - **Build Command**
     ```
     pip install -r requirements.txt
     ```
   - **Start Command**
     ```
     python bot.py
     ```
5) أضف Environment Variables:
   - `BOT_TOKEN` = توكن البوت
   - `MAX_MB` = 50 (اختياري)

## ملاحظات
- بدون FFmpeg قد تفشل بعض الروابط التي تتطلب دمج صوت/فيديو؛ نحاول اختيار صيغة "تقدمية" لتفادي ذلك.
- استخدم البوت للمحتوى العام أو المصرّح به فقط.
