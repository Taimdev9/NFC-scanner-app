<div align="center">

# 📡 NFC Web Reader
### By TRL TEAM FOR DEVELOPMENT

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Web NFC](https://img.shields.io/badge/Web_NFC-API-blue?style=for-the-badge)](https://w3c.github.io/web-nfc/)

**A lightweight, bilingual, and browser-based NFC tag reader.**

</div>

---

## 🇬🇧 English Documentation

### 📖 About The Project
**NFC Web Reader** is a single-file web application developed by **TRL TEAM FOR DEVELOPMENT**. It utilizes the **Web NFC API** to scan and decode NFC tags directly through the browser without the need for a native mobile application. 

The application is designed to parse standard **NDEF** (NFC Data Exchange Format) records such as URLs, Text, and MIME types. Additionally, it features a smart detection mechanism that alerts users when an unsupported card (like a bank card or ID) is scanned, ensuring transparency and data privacy.

### ✨ Key Features
- **Bilingual Support:** Seamlessly switch between English (Default) and Arabic with full RTL/LTR layout support.
- **Sleek UI/UX:** Minimalist black, white, and gray design with a professional loading screen.
- **Smart Detection:** Decodes URLs, Text, MIME types, Smart Posters, and Absolute URLs.
- **Bank Card Alert:** Detects when an unsupported card is tapped and informs the user that sensitive data cannot be read.
- **Single File:** The entire application (HTML, CSS, JS) is bundled into one `index.html` file for easy deployment.

### ⚙️ Prerequisites & Limitations
> **Important:** Web NFC is currently a working draft and has strict limitations:
- **Device:** Must be an **Android** device with NFC hardware.
- **Browser:** Requires **Google Chrome** (or Chromium-based browsers). It is **NOT** supported on iOS (Safari) or Desktop browsers.
- **Security:** The website **MUST** be served over **HTTPS** (e.g., GitHub Pages, Vercel, Netlify).
- **Privacy:** The API cannot read encrypted bank card data or unformatted smart cards.

### 🚀 How to Use
1. Open the hosted website on your Android device using Google Chrome.
2. Click the **"Start Scan"** button.
3. Tap any NFC tag (like NTAG213) against the back of your phone.
4. View the decoded data instantly on the screen.

---

## 🇸🇦 التوثيق العربي

### 📖 عن المشروع
**قارئ NFC عبر الويب** هو تطبيق ويب بملف واحد تم تطويره بواسطة **فريق TRL للتطوير (TRL TEAM FOR DEVELOPMENT)**. يعتمد التطبيق على **Web NFC API** لمسح وقراءة علامات NFC مباشرة من خلال المتصفح، دون الحاجة لتثبيت تطبيق خارجي.

صُمم التطبيق لتحليل سجلات **NDEF** القياسية مثل الروابط (URLs)، والنصوص (Text)، وأنواع MIME. كما يتميز بآلية ذكية للتنبيه عند محاولة قراءة بطاقة غير مدعومة (مثل البطاقات البنكية أو بطاقات الهوية)، مما يضمن الشفافية وحماية الخصوصية.

### ✨ المميزات الرئيسية
- **دعم اللغتين:** التبديل بسلاسة بين اللغتين الإنجليزية (الافتراضية) والعربية مع دعم كامل لاتجاه النص (RTL/LTR).
- **تصميم عصري وبسيط:** واجهة مستخدم تعتمد على الألوان الأساسية (الأبيض، الأسود، الرمادي) مع شاشة تحميل احترافية.
- **اكتشاف ذكي:** قراءة وتحليل الروابط، النصوص، أنواع MIME، والملصقات الذكية.
- **تنبيه البطاقات البنكية:** يكتشف التطبيق البطاقات غير المدعومة ويبلغ المستخدم بعدم إمكانية قراءة بياناتها الحساسة.
- **ملف واحد:** الكود بالكامل (HTML, CSS, JS) موجود في ملف `index.html` واحد لسهولة النشر والرفع.

### ⚙️ المتطلبات والقيود
> **تنبيه هام:** تقنية Web NFC لا تزال في مرحلة المسودة، ولها قيود صارمة:
- **الجهاز:** يجب أن يكون جهاز **أندرويد (Android)** يحتوي على شريحة NFC.
- **المتصفح:** يتطلب متصفح **Google Chrome** (أو المتصفحات المبنية على Chromium). **لا يدعم** أجهزة iOS (Safari) أو متصفحات الكمبيوتر.
- **الأمان:** يجب استضافة الموقع على خادم يدعم **HTTPS** (مثل GitHub Pages، Vercel، Netlify).
- **الخصوصية:** لا يمكن للتطبيق قراءة البيانات المشفرة للبطاقات البنكية أو البطاقات الذكية غير المهيأة.

### 🚀 كيفية الاستخدام
1. افتح رابط الموقع المستضاف على جهاز الأندرويد الخاص بك باستخدام متصفح Google Chrome.
2. اضغط على زر **"بدء المسح" (Start Scan)**.
3. قم بلمس أي علامة NFC (مثل NTAG213) في الجزء الخلفي من هاتفك.
4. شاهد البيانات التي تم فك تشفيرها فورًا على الشاشة.

---

## 👨‍💻 Team & Credits
- **Developed by:** TRL TEAM FOR DEVELOPMENT
- **Team Leader:** Taimdev9
- **Project Type:** Web NFC Integration (Frontend)

<div align="center">
  <br>
  <i>Built with ❤️ by TRL TEAM</i>
</div>
