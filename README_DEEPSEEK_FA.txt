نسخه Gemini ربات Taha's Helper Bot

برای اجرا:
1) متغیر GEMINI_API_KEY را تنظیم کن.
2) وابستگی‌ها را نصب کن: pip install -r requirements.txt
3) اجرا: gunicorn app:app

مدل پیش‌فرض چت، تحلیل تصویر و تبدیل صدا gemini-2.5-flash است.
برای تغییر مدل از متغیرهای GEMINI_MODEL، GEMINI_VISION_MODEL و GEMINI_TRANSCRIBE_MODEL استفاده کن.
ساخت تصویر/ویدیو با Pollinations و ساخت سه‌بعدی با V2Fun جداگانه باقی مانده‌اند.
