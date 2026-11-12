اتصال معراج بات به DeepSeek
================================
در Render > Environment این متغیرها را تنظیم کن:

DEEPSEEK_API_KEY = کلید ساخته‌شده در DeepSeek Platform
DEEPSEEK_MODEL = deepseek-chat  (اختیاری؛ مقدار پیش‌فرض همین است)

Base URL: https://api.deepseek.com

تبدیل صدای ورودی به متن همچنان از Groq Whisper استفاده می‌کند. اگر می‌خواهی میکروفون هم کار کند، یکی از این دو متغیر را تنظیم کن:
GROQ_TRANSCRIBE_API_KEY = کلید Groq فقط برای Whisper
یا GROQ_API_KEY = کلید Groq (سازگاری با تنظیم قبلی)

نکته: DeepSeek API رایگان نیست و بر اساس تعرفه حساب می‌شود. مدل deepseek-chat ورودی تصویری را پشتیبانی نمی‌کند؛ قابلیت تحلیل تصویر در این نسخه با DeepSeek قابل استفاده نیست. ظاهر سایت و قابلیت‌های مستقل V2Fun/Pollinations/Vadoo تغییر نکرده‌اند.
