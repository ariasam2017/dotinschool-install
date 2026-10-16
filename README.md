# dotinschool-install

<div dir="rtl" align="right">

نصب سریع سامانه‌های **دوتین‌اسکول** روی سرور لینوکس — **با یک دستور، بدون توکن گیت‌هاب و بدون نیاز به Go**.

این مخزن فقط اسکریپت‌های نصب و نسخهٔ آماده (باینری کامپایل‌شده + فایل‌های Docker) را دارد؛ کد منبع خصوصی است.

دستور را با کاربر **root** در ترمینال سرور بزنید. روی سرور تازه مستقیم نصب می‌کند؛ اگر قبلاً نصب شده باشد، همان دستور **منوی مدیریتی** را باز می‌کند.

## 💻 سامانهٔ چالش برنامه‌نویسی

**نصب مستقل (سرویس سیستم):**

</div>

```bash
bash <(curl -Ls https://raw.githubusercontent.com/ariasam2017/dotinschool-install/main/challenge.sh)
```

<div dir="rtl" align="right">

**نصب با Docker:**

</div>

```bash
bash <(curl -Ls https://raw.githubusercontent.com/ariasam2017/dotinschool-install/main/challenge-docker.sh)
```

<div dir="rtl" align="right">

بعد از نصب: منوی مدیریتی با دستور `dotinschool-challenge` · پورت پیش‌فرض **8081**

## 🎮 بازی «لیگ قهرمانان برنامه‌نویسی»

**نصب مستقل (سرویس سیستم):**

</div>

```bash
bash <(curl -Ls https://raw.githubusercontent.com/ariasam2017/dotinschool-install/main/game.sh)
```

<div dir="rtl" align="right">

**نصب با Docker:**

</div>

```bash
bash <(curl -Ls https://raw.githubusercontent.com/ariasam2017/dotinschool-install/main/game-docker.sh)
```

<div dir="rtl" align="right">

بعد از نصب: منوی مدیریتی با دستور `dotinschool-game` · پورت پیش‌فرض **8080**

## نکته‌ها

- هر دو سامانه کاملاً مستقل‌اند (دیتابیس، سرویس، پورت و منوی جدا) و می‌توانند روی یک سرور کنار هم نصب شوند. فقط یکی از آن‌ها می‌تواند با دامنه روی پورت 443 HTTPS بگیرد.
- آخر نصب، آدرس پنل، نام کاربری و رمز ادمین چاپ می‌شود. بعداً با `dotinschool-challenge admin` یا `dotinschool-game admin` دوباره قابل دیدن است.
- **به‌روزرسانی:** روی سرور `dotinschool-challenge update` یا `dotinschool-game update` (یا گزینهٔ ۲ منو). داده‌ها دست‌نخورده می‌مانند.
- اگر سرور به گیت‌هاب دسترسی نداشت، اسکریپت خودش از mirrorهای عمومی دانلود می‌کند. اگر باز هم نشد، گزینهٔ «Cloudflare WARP» منو را بزنید.

</div>
