<p align="center">
  <img src="assets/img/logo.svg" alt="شعار مكتب الرسالة" width="120" height="120">
</p>

<h1 align="center">🎓 مكتب الرسالة — Thesis Desk (v3)</h1>

<p align="center">
  <b>مساعد ذكي لإدارة رسالة الدكتوراه</b> — من تحديد المشروع حتى بناء الاستبيان، مع فحص صحة المراجع والبحث الأكاديمي.
</p>

<p align="center">
  <a href="https://ahmedawe2026-svg.github.io/DBA-Research-Dissertation-Assistant/"><b>🌐 تجربة مباشرة</b></a>
  &nbsp;·&nbsp;
  <a href="docs/guide.html">📖 دليل الاستخدام</a>
  &nbsp;·&nbsp;
  <a href="README.en.md">English</a>
</p>

<p align="center">
  <img alt="License" src="https://img.shields.io/badge/License-MIT-2f5fe0.svg">
  <img alt="HTML5" src="https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white.svg">
  <img alt="CSS3" src="https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white.svg">
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black.svg">
  <img alt="No dependencies" src="https://img.shields.io/badge/dependencies-none-0f8a52.svg">
  <img alt="RTL" src="https://img.shields.io/badge/العربية-RTL-7038d8.svg">
</p>

---

تطبيق ويب عربي (RTL) لإدارة رسالة الدكتوراه من البداية حتى الاستبيان: **ملف المشروع، الهيكل، الدراسات السابقة، سجل المراجع، فحص صحة المراجع، البحث الأكاديمي، مصفوفة الاتساق، والمولّد الآلي للمادة العلمية**.

يعمل بلا إنترنت في معظم الأجزاء (البيانات تُحفظ محلياً في متصفّحك)، ويستخدم الإنترنت اختيارياً للبحث الأكاديمي والتحقق من المراجع.

---

## 🖼️ لقطات الشاشة

<p align="center">
  <img src="screenshots/01-dashboard.png" alt="لوحة الملخص والتحقق" width="49%">
  <img src="screenshots/02-generator.png" alt="المولّد الآلي" width="49%">
</p>
<p align="center">
  <img src="screenshots/03-search.png" alt="البحث الأكاديمي" width="49%">
  <img src="screenshots/04-guide.png" alt="دليل الاستخدام" width="49%">
</p>
<p align="center">
  <img src="screenshots/05-dark-mode.png" alt="الوضع الليلي" width="70%">
</p>

---

## ✨ المزايا الرئيسية

### التبويبات
| # | التبويب | الوظيفة |
|---|---------|---------|
| 0 | 📊 الملخص والتحقق | لوحة تقدم + نتائج قواعد التحقق (أكثر من 25 قاعدة) وإحصاءات |
| 1 | 🧾 ملف المشروع | العنوان، القطاع، المتغير المستقل/التابع/الوسيط، الحد الأدنى لسنوات الدراسات (2020) |
| 2 | 🗂️ متتبع الهيكل | 7 أجزاء و48 قسماً مع حالة كل قسم وملاحظات المشرف |
| 3 | 📚 الدراسات السابقة | بطاقات الدراسات (13 حقلاً) مصنّفة بالمحاور |
| 4 | 🔗 سجل المراجع | توثيق APA 7 + تصنيف (أ/ب/ج) + محكّم/لغة |
| 5 | 🔎 فحص المراجع | فحص مباشر عبر Crossref و OpenAlex |
| 6 | 🔍 البحث الأكاديمي | 36 بوابة بحث في 4 مجموعات + مولّد الاستعلامات |
| 7 | 🧩 مصفوفة الاتساق | ربط الفجوة/السؤال/الهدف/الفرضية/الأداة/النتيجة/التوصية |
| 8 | 🗑️ سلة المحذوفات | استعادة العناصر المحذوفة |
| 9 | 💾 النسخ الاحتياطي | تصدير/استيراد المشاريع + لقطات حتى 5 |
| 10 | 🤖 المولّد الآلي | بحث آلي + فحص + تجميع + توليد نص أكاديمي |

### 🤖 المولّد الآلي (v3 الجديد)
- **بحث آلي** في فهرس **OpenAlex** العالمي بناءً على متغيرات المشروع + كلمات إضافية.
- يستبعد تلقائياً العمل **المسحوب (Retraction)** وبلا DOI.
- **إضافة تلقائية**: دراسة سابقة + مرجع بتوثيق APA مولّد آلياً.
- **فحص آلي** لكل مرجع مُضاف عبر Crossref/OpenAlex.
- **تجميع جاهز للتصدير (Word / Markdown)**:
  - تقرير المراجعة الأدبية.
  - هيكل الرسالة الكامل (مع الدراسات والمصفوفة والمراجع).
- **مولّد نص أكاديمي** (اختياري) عبر مفتاح API متوافق مع OpenAI: مقدمة الفصل الثاني، تعليق نقدي وفجوة، أسئلة استبيان أولية.

---

## 🗂️ بنية المستودع

```
DBA-Research-Dissertation-Assistant/
├── index.html                  # الصفحة الرئيسية
├── assets/
│   ├── css/style.css           # كل الأنماط (نهاري/ليلي تلقائي)
│   ├── js/app.js               # كل منطق التطبيق
│   └── img/logo.svg            # الشعار والأيقونة
├── standalone/
│   └── thesis-desk-v3.html     # نسخة مكتفية ذاتياً (ملف واحد يعمل بأي مكان)
├── docs/
│   └── guide.html              # دليل الاستخدام الشامل (22 قسماً، قابل للطباعة PDF)
├── screenshots/                # لقطات الشاشة
├── README.md                   # التوثيق العربي
├── README.en.md                # التوثيق الإنجليزي
├── LICENSE
└── .gitignore
```

> **ملاحظة:** توجد نسختان:
> - `index.html` + `assets/` → للتطوير والنشر عبر GitHub Pages.
> - `standalone/thesis-desk-v3.html` → ملف واحد جاهز للاستخدام المباشر بمجرد فتحه في المتصفّح.

> 📖 **دليل الاستخدام الكامل:** [`docs/guide.html`](docs/guide.html) — يشرح كل تبويب خطوة بخطوة.

---

## 🚀 التشغيل

### الطريقة الأولى — فتح مباشر
افتح `standalone/thesis-desk-v3.html` في متصفّحك مباشرة (Chrome / Edge / Firefox).

### الطريقة الثانية — نسخة المطوّر
افتح `index.html` مباشرة، أو شغّل خادماً محلياً:

```bash
# Python
python -m http.server 8080

# Node
npx serve .
```
ثم افتح `http://localhost:8080`.

### النشر عبر GitHub Pages
الموقع مُفعّل على:
**https://ahmedawe2026-svg.github.io/DBA-Research-Dissertation-Assistant/**

---

## 📖 دليل الاستخدام
دليل مفصّل يشرح كل تبويب خطوة بخطوة (22 قسماً):

- الملف: [`docs/guide.html`](docs/guide.html)
- مباشر: https://ahmedawe2026-svg.github.io/DBA-Research-Dissertation-Assistant/docs/guide.html

الدليل يدعم الوضعين النهاري/الليلي، وقابل للطباعة أو الحفظ كـ **PDF**.

---

## 🔐 الخصوصية والبيانات
- كل البيانات تُحفظ في **متصفّحك فقط** (`localStorage` بمفتاح `thesis-desk-v2`) ولا تُرسَل إلى أي خادم.
- عمليات البحث والفحص تتصل بواجهات عامة مجانية:
  - [OpenAlex](https://api.openalex.org) — بحث الفهارس.
  - [Crossref](https://api.crossref.org) — فحص DOI والتوثيق.
- مفتاح الـAPI (اختياري، للمولّد النصي) يُحفظ محلياً في متصفّحك فقط (`td-api`).

---

## ⚠️ تنبيه أخلاقي وعلمي
هذا التطبيق **أداة مساعدة** للجمع والفحص والتنسيق، وليس بديلاً عن الباحث أو المشرف. يجب مراجعة كل مُخرَج وتحريره والتحقق منه، والالتزام بسياسة جامعتك بشأن أدوات المساعدة. النصوص المولّدة آلياً مسوّدات أولية فقط.

---

## 🛠️ التقنية
- HTML5 + CSS3 + JavaScript (Vanilla، بلا مكتبات خارجية).
- تصميم عربي RTL مع دعم الوضع النهاري/الليلي تلقائياً حسب النظام.
- تعمل كملف محلي أو مستضافة على أي خادم ثابت.

---

## 📄 الرخصة
هذا المشروع تحت رخصة **MIT** — انظر ملف [LICENSE](LICENSE).