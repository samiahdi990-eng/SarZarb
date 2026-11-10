# سرضرب - نسخه آغازین

این پروژه یک نمونه اولیه قابل اجرا از بازی سرضرب است:
- نمای بازی سه‌بعدی‌نما با زمین شطرنجی و موانع مثلثی
- هر لمس صفحه یک حرکت به راست و لمس بعدی یک حرکت به چپ
- ۱۰۰ توپ نمایشی که کم نمی‌شود
- ۲۵۰ لیول، ۱۰ فصلِ ۲۵ لیولی، فینال و چرخ شانس
- منوی انتخاب لیول، توپ‌ها و مأموریت‌ها
- ذخیره پیشرفت روی همان دستگاه

## ساخت APK با GitHub
1. این ZIP را استخراج و محتویاتش را در یک مخزن GitHub قرار بده.
2. در GitHub برو به تب **Actions**.
3. workflow با نام **Build Android APK** را اجرا کن.
4. بعد از پایان موفق، در همان اجرای Actions بخش **Artifacts** فایل `SarZarb-debug-apk` را دانلود کن.
5. فایل APK داخل ZIP دانلودشده است.

## آپلود از Termux
```bash
pkg update -y
pkg install git unzip -y
unzip sarzarb_game.zip
cd sarzarb_game
git init
git add .
git commit -m "Initial SarZarb game"
git branch -M main
git remote add origin https://github.com/USERNAME/REPOSITORY.git
git push -u origin main
```
به‌جای USERNAME و REPOSITORY نام حساب و مخزن خودت را بگذار.

## نکته
این نسخه نمونه اولیه است، نه بازسازی کامل موتور سه‌بعدی بازی اصلی. برخوردها، فیزیک و گرافیک فعلاً ساده‌سازی شده‌اند. برای انتشار عمومی باید تست، بهینه‌سازی و تکمیل سیستم فصل/فینال انجام شود.
