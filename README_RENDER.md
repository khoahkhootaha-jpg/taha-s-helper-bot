# Taha's Helper Bot — آماده استقرار روی Render

## تنظیمات Render
- Runtime: Python 3
- Build Command: `pip install -r requirements.txt`
- Start Command: `gunicorn app:app`
- Plan: Free

## Environment Variables
در Render این دو متغیر را اضافه کن:

- `GROQ_API_KEY` = کلید Groq خودت
- `POLLINATIONS_API_KEY` = کلید Pollinations (اختیاری؛ فقط برای ساخت تصویر)

کلیدها را داخل GitHub یا فایل کد قرار نده.

## نکته مهم درباره Free
Render برای سرویس رایگان بعد از 15 دقیقه بدون درخواست، سرویس را متوقف می‌کند و درخواست بعدی آن را دوباره بالا می‌آورد. همچنین فایل‌های محلی مثل تاریخچه و فایل‌های آپلودشده روی Free پایدار نیستند و با restart/redeploy/spin-down ممکن است از بین بروند.


## MiniMax video generation
Add `MINIMAX_API_KEY` in Render Environment. Optional settings: `MINIMAX_API_BASE=https://api.minimax.io`, `MINIMAX_VIDEO_MODEL=MiniMax-H3`, `MINIMAX_VIDEO_RESOLUTION=768P`. The video generator is configured for 5-second clips. See `README_MINIMAX_FA.txt` for the complete environment list.
