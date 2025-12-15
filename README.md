# پروژه یادگیری ماشین املاک 🏠📊

این رپازیتوری برای انجام پروژه‌ی گروهی درس **یادگیری ماشین** طراحی شده است. هدف اصلی این ساختار، جلوگیری از تداخل کدها (به‌خصوص در Jupyter Notebookها) و ساده‌سازی همکاری ۴ نفره با استفاده از **Git و GitHub** است.

---

## اعضای تیم

* Ehsan
* Mahya
* Parisa
* Navid

---

## ساختار کلی پروژه

```
real-estate-ml-project
│   .gitignore
│   README.md
│
├── 1-Questions
│   ├── drafts
│   │   ├── navid-questions.ipynb
│   │   ├── ehsan-questions.ipynb
│   │   ├── mahya-questions.ipynb
│   │   └── parisa-questions.ipynb
│   │
│   └── questions-final.ipynb
│
├── 2-Hypothesis
│   ├── drafts
│   └── hypothesis-final.ipynb
│
├── 3-Problem1
│   ├── drafts
│   └── problem1-final.ipynb
│
└── 4-Problem2
│   ├── drafts
│   └── problem2-final.ipynb
```

###  توضیح ساختار

* پوشه‌های `drafts/` مخصوص نوت‌بوک‌های شخصی هر فرد هستند
* فایل‌های `*-final.ipynb` نسخه‌ی نهایی و قابل تحویل پروژه‌اند
* هیچ‌کس به‌صورت مستقیم روی فایل‌های final کار نمی‌کند

---

##  استراتژی برنچ‌ها (Branch Strategy)

### شاخه‌ی اصلی

* `main`: فقط شامل کدهای نهایی و تمیز

### برنچ‌های کاری

هر فرد برای هر بخش یک برنچ جدا دارد:

مثال:

* `navid-questions`
* `ehsan-problem1`
* `mahya-hypothesis`

❌ کامیت مستقیم روی `main` ممنوع است

---

##  شروع کار (برای هر عضو تیم)

### 1️⃣ دریافت پروژه

```bash
git clone https://github.com/NavidByti/real-estate-ml-project.git
cd real-estate-ml-project
```

### 2️⃣ ساخت برنچ شخصی

```bash
git checkout main
git pull
git checkout -b navid-questions
```

---

##  روند کار روزانه

### 🔹 فقط روی فایل شخصی خودت کار کن

مثال:

```
1-Questions/drafts/navid-questions.ipynb
```

### 🔹 ذخیره تغییرات (Commit)

```bash
git add 1-Questions/drafts/navid-questions.ipynb
git commit -m "تحلیل سوالات ۱، ۵ و ۶"
```

### 🔹 ارسال به GitHub (Push)

```bash
git push origin navid-questions
```

---

##  Pull Request (PR) چیست؟

Pull Request یعنی:

> «من کارم را در برنچ خودم تمام کرده‌ام، لطفاً آن را به main اضافه کنید»

### مراحل:

1. رفتن به GitHub
2. انتخاب برنچ خودت
3. کلیک روی **Open Pull Request**
4. توضیح کوتاه درباره کاری که انجام دادی
5. تأیید و Merge

---

##  ساخت فایل نهایی (Final Notebook)

برای هر بخش، یک نفر (یا دو نفر) مسئول جمع‌بندی است:

### مراحل:

1. گرفتن آخرین نسخه‌ی main

```bash
git checkout main
git pull
```

2. ساخت برنچ جدید

```bash
git checkout -b questions-final
```

3. باز کردن نوت‌بوک‌های drafts و انتقال:

* کدهای درست
* نمودارها
* توضیحات تمیز و آکادمیک

4. کامیت فایل نهایی

```bash
git add 1-Questions/questions-final.ipynb
git commit -m "نسخه نهایی سوالات"
git push origin questions-final
```

5. Pull Request و Merge

---

## ⚠️ قوانین مهم

* ❌ ویرایش همزمان یک نوت‌بوک توسط دو نفر ممنوع
* ❌ کامیت مستقیم روی `main` ممنوع
* ✅ هر نفر فقط فایل خودش را تغییر دهد
* ✅ قبل از شروع کار همیشه `git pull`

---

## 🛠 دستورات پرکاربرد Git

| دستور                   | توضیح               |
| ----------------------- | ------------------- |
| `git status`            | دیدن وضعیت فایل‌ها  |
| `git branch`            | دیدن برنچ‌ها        |
| `git checkout <branch>` | رفتن به برنچ        |
| `git pull`              | گرفتن آخرین تغییرات |
| `git push`              | ارسال تغییرات       |

---


این ساختار:

* از تداخل Jupyter Notebook جلوگیری می‌کند
* همکاری تیمی را ساده می‌کند
* استاندارد و قابل ارائه برای پروژه‌های ML است

اگر همه به این روند پایبند باشیم، پروژه بدون دردسر جلو می‌رود 🚀

موفق باشید 💙
