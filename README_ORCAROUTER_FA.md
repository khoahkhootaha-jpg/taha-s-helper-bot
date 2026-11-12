# راهنمای اتصال Taha Helper Bot به OrcaRouter

این نسخه، API اصلی چت و تحلیل تصویر را از Groq به OrcaRouter منتقل می‌کند.

## متغیرهای Render

در Render → سرویس برنامه → Environment این موارد را تنظیم کن:

- `ORCAROUTER_API_KEY`: کلید API که در OrcaRouter ساخته‌ای (محرمانه)
- `ORCAROUTER_MODEL`: `z-ai/glm-5.3-flash-free`
- `ORCAROUTER_VISION_MODEL`: `z-ai/glm-5.3-flash-free`
- `POLLINATIONS_API_KEY`: در صورت استفاده از تولید تصویر/ویدیو
- `V2FUN_API_KEY`: در صورت استفاده از تولید سه‌بعدی
- `VADOO_API_KEY`: در صورت استفاده از سرویس ویدیویی Vadoo

Base URL به‌صورت پیش‌فرض روی `https://api.orcarouter.ai/v1` تنظیم شده است.
در صورت نیاز می‌توان آن را با `ORCAROUTER_BASE_URL` تغییر داد.

## نکته درباره میکروفون

چت متنی و تحلیل تصویر از OrcaRouter استفاده می‌کنند. مسیر تبدیل صدای ضبط‌شده به متن در این نسخه همچنان از Groq Whisper استفاده می‌کند؛ بنابراین برای فعال ماندن تبدیل گفتار به متن، متغیر اختیاری `GROQ_TRANSCRIBE_API_KEY` را جداگانه در Render تنظیم کن. اگر آن را تنظیم نکنی، چت متنی کار می‌کند اما مسیر `/api/transcribe` پیام می‌دهد که کلید جداگانه لازم است.

## استقرار

Build Command:
`pip install -r requirements.txt`

Start Command:
`gunicorn app:app`

کلیدها را در GitHub یا داخل کد قرار نده. اگر کلید قبلی جایی عمومی شده، آن را در داشبورد OrcaRouter باطل و یک کلید جدید بساز.
