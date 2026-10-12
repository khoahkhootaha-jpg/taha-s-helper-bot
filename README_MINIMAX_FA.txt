Taha's Helper Bot Updated — راهنمای Environment Variables

برای Render این متغیرها را در Environment وارد کن. کلیدها را داخل چت یا فایل عمومی قرار نده.

ضروری برای چت:
- GROQ_API_KEY = کلید Groq فعلی پروژه
- MINIMAX_API_KEY = کلید API مربوط به MiniMax (برای ویدیو)

متغیرهای ویدیوی MiniMax:
- MINIMAX_API_BASE = https://api.minimax.io
- MINIMAX_VIDEO_MODEL = MiniMax-H3
- MINIMAX_VIDEO_RESOLUTION = 768P

متغیرهای اختیاری/باقی‌مانده از پروژه:
- GROQ_MODEL = openai/gpt-oss-120b (اگر مدل فعلی‌ات چیز دیگری است، مقدار فعلی را نگه دار)
- GROQ_VISION_MODEL = qwen/qwen3.8-27b (مقدار فعلی خودت را ترجیح بده)
- POLLINATIONS_API_KEY = فقط اگر ساخت تصویر Pollinations را استفاده می‌کنی
- POLLINATIONS_IMAGE_MODEL = اختیاری
- POLLINATIONS_VIDEO_MODEL = اختیاری، برای مسیر قدیمی Pollinations
- VADOO_API_KEY = مسیر قدیمی Vadoo؛ برای MiniMax لازم نیست
- VADOO_LANGUAGE = اختیاری، مسیر قدیمی Vadoo
- VADOO_VOICE = اختیاری، مسیر قدیمی Vadoo
- VADOO_THEME = اختیاری، مسیر قدیمی Vadoo

نکته:
- کلید MiniMax به‌تنهایی کافی نیست؛ فایل app.py نیز برای ساخت و بررسی وضعیت ویدیو تغییر داده شده است.
- ویدیوی MiniMax از API رسمی به‌صورت task ساخته می‌شود و تا آماده‌شدن لینک، وضعیت بررسی می‌شود.
- این نسخه برای شروع ویدیوهای 5 ثانیه‌ای با رزولوشن 768P تنظیم شده تا با محدوده API سازگار باشد. ساخت ویدیو ممکن است هزینه داشته باشد؛ قبل از استفاده، موجودی و قیمت حساب MiniMax را بررسی کن.
- طراحی HTML/CSS و چیدمان صفحه عمداً تغییر داده نشده است.
