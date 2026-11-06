# 📆 Shamsi Advanced Calendar for Power BI | تقویم شمسی پیشرفته پاور بی‌آی

[![Power BI Custom Visual](https://img.shields.io/badge/Power_BI-Custom_Visual-F2C811?logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Jalali Calendar](https://img.shields.io/badge/Calendar-Solar_Hijri_(Jalali)-teal.svg)](#)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

[English](#english) | [فارسی](#فارسی)

---

## فارسی

### معرفی پروژه
**تقویم شمسی پیشرفته (Shamsi Advanced Calendar)** کامل‌ترین و قدرتمندترین ابزار بصری تقویم و مدیریت رویداد مبتنی بر گاه‌شماری خورشیدی جلالی برای Power BI است. این ویژوال با تلفیق ۴ نمای تحلیلی بی‌نظیر، نوار شاخص‌های زنده (KPIs)، زمان‌بندی ساعت‌به‌ساعت و دسته‌بندی موضوعی رویدادها، تجربه کار با تقویم را در داشبوردهای مدیریتی دگرگون می‌کند.

---

### 🌟 نماهای ۴ گانه تقویم

| نما (View) | شرح و قابلیت‌ها |
| :--- | :--- |
| **۱. نمای ماهانه (Month View)** | چیدمان سنتی و کاربردی تقویم ماه با برچسب‌های رویداد، تاریخ معادل میلادی، هایلایت تعطیلات و نشانگر امروز |
| **۲. هیت‌مپ سالانه (Annual Heatmap)** | ماتریس حرارتی ۳۶۵ روزه (مشابه GitHub Heatmap) برای شناسایی فصول و روزهای اوج رخدادها در یک نگاه |
| **۳. نمای هفتگی (Week View)** | بررسی فشرده فعالیت‌ها و رویدادهای ۷ روز هفته با کارت‌های مجزا |
| **۴. نمای روزانه با محور زمانی (Daily Timeline)** | محور ۲۴ ساعته با ثبت ساعت شروع و پایان (مثلاً ۰۸:۳۰ تا ۱۲:۰۰) و **مدیریت هوشمند تداخل زمان‌ها (Overlap)** |

---

### ✨ سایر قابلیت‌های برجسته
- 📊 **نوار شاخص‌های کلیدی (KPI Summary Bar):** محاسبه لحظه‌ای مجموع مقادیر ماه، میانگین روزانه و تعداد کل فعالیت‌ها.
- 🎨 **سیستم وضعیت و برچسب‌های رنگی:** اختصاص رنگ‌های مجزا به دسته‌بندی‌ها (فنی، مالی، بازاریابی، شیفت) و برچسب‌های وضعیت (عادی، مهم، بحرانی).
- ⏱️ **مدیریت تداخل زمانی رویدادها:** سازمان‌دهی خودکار ستون‌های موازی در صورت وقوع دو یا چند رویداد هم‌زمان در نمای روزانه.
- ⚙️ **شخصی‌سازی گسترده در پنل فرمت:** امکان خاموش/روشن کردن هر یک از نماها، قفل کردن تقویم روی ماه جاری، تنظیم فونت‌های فارسی، استایل بولد/ایتالیک و سفارشی‌سازی رنگ روزهای تعطیل.
- 🔍 **تول‌تیپ تعاملی و هوشمند:** نمایش خلاصه روزانه در نمای ماه و شناسنامه جامع رویداد هنگام مکث موس روی کارت‌ها.

---

### 🗂️ راهنمای نگاشت فیلدهای داده (Field Mapping)

| نقش در Power BI | نوع فیلد | توضیحات |
| :--- | :---: | :--- |
| **تاریخ رویداد (Event Date)** | الزامی | تاریخ به فرمت شمسی (مانند `1405/07/08`) یا میلادی |
| **عنوان رویداد / فعالیت (Event Title)** | الزامی | نام یا شرح مختصر رویداد |
| **دسته‌بندی (Category)** | اختیاری | عنوان دسته‌بندی جهت رنگ‌بندی تفکیک‌شده |
| **مقدار عددی (Value)** | اختیاری | مبالغ، ساعات کارکرد یا اوزان جهت محاسبه جمع ماه و هیت‌مپ |
| **زمان شروع (Start Time)** | اختیاری | ساعت شروع به فرمت `08:00` یا `14:30` |
| **زمان پایان (End Time)** | اختیاری | ساعت پایان به فرمت `12:00` یا `16:30` |
| **وضعیت / اولویت (Status)** | اختیاری | برچسب‌های اولویت رویداد |

---

### 🛠️ کامپایل و توسعه محلی
```bash
# نصب پکیج‌ها
npm install

# اجرای سرویس توسعه محلی
npm start

# ساخت بسته‌های نهایی (.pbiviz)
node build-deliver.js
```

---

## English

### Overview
**Shamsi Advanced Calendar** is the ultimate Persian (Jalali / Solar Hijri) calendar and schedule visualization engine for Microsoft Power BI. It combines multi-view calendar layouts, heatmaps, live KPI metrics, and a daily 24-hour timeline with automatic event conflict (overlap) management.

### 🌟 4 Integrated Calendar Views
1. **Smart Month View:** Traditional monthly calendar grid featuring event chips, dual Gregorian date equivalents, weekend & holiday highlights, and today indicator.
2. **Annual Heatmap View:** 365-day density matrix (GitHub-style) designed for spotting peak business activity and pattern detection.
3. **Week View:** Concise 7-day schedule breakdown.
4. **Daily Timeline View:** Hourly 24-hour vertical timeline with start & end times and smart horizontal lane allocation for overlapping events.

### ✨ Highlights
- **Real-time KPI Summary Bar:** Automatically computes monthly totals, daily averages, and event counts.
- **Event Categorization & Priority:** Visual color coding by departments (HR, Sales, Tech, Ops) and status pills.
- **Rich Formatting Pane:** Turn individual views on/off, lock navigation to the current month, choose embedded Persian fonts (Vazirmatn, Sahel, Shabnam), and customize palette themes.
- **Cross-Platform Delivery:** Runs smoothly on Power BI Desktop, Power BI Cloud Service, and Power BI Report Server (PBIRS).

### 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
