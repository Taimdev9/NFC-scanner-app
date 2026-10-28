<div align="center">

# 📡 NFC Web Reader & Logger

### By TRL TEAM FOR DEVELOPMENT

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com/)
[![Web NFC](https://img.shields.io/badge/Web_NFC-API-blue?style=for-the-badge)](https://w3c.github.io/web-nfc/)

**A lightweight, bilingual, browser-based NFC tag reader with real-time Cloud logging via Firebase.**

</div>

---

## 🇬🇧 English Documentation

### 📖 About The Project
**NFC Web Reader & Logger** is a powerful single-file web application developed by **TRL TEAM FOR DEVELOPMENT**. It utilizes the **Web NFC API** to scan and decode NFC tags directly through the browser, eliminating the need for a native mobile application.

The application is designed to parse standard **NDEF** records and features a smart detection mechanism that alerts users when an unsupported card (like a bank card) is scanned. Furthermore, every scan is securely logged in real-time to a **Firebase Firestore** database for monitoring and analytics.

### ✨ Key Features
- **Real-time Cloud Logging:** Sends scan data (Serial Number, Type, Decoded Content, Timestamp) directly to Firebase Firestore.
- **Bilingual Support:** Seamlessly switch between English (Default) and Arabic with full RTL/LTR layout support.
- **Smart Detection:** Decodes URLs, Text, MIME types, and distinguishes between standard NDEF tags and encrypted smart cards (e.g., Bank Cards).
- **Sleek UI/UX:** Minimalist black, white, and gray design with a professional loading screen.
- **Single File Architecture:** HTML, CSS, and JS are bundled into one `index.html` file for easy deployment.

### ⚙️ Prerequisites & Limitations
> **Important:** Web NFC is currently a working draft and has strict limitations:
- **Device:** Must be an **Android** device with NFC hardware.
- **Browser:** Requires **Google Chrome** (or Chromium-based browsers). It is **NOT** supported on iOS (Safari) or Desktop browsers.
- **Security:** The website **MUST** be served over **HTTPS** (e.g., GitHub Pages, Vercel, Netlify).

### 🚀 How to Deploy
1. Clone the repository or copy the `index.html` file.
2. Ensure your Firebase project is set up and Firestore is enabled in **Test Mode** (or configure proper Security Rules).
3. Update the `firebaseConfig` object in the `<script type="module">` tag with your own Firebase project credentials.
4. Host the file on a secure HTTPS server (like GitHub Pages).
5. Open the link on an Android device using Chrome.

---

## 🇸🇦 التوثيق العربي

### 📖 عن المشروع
**قارئ ومسجل NFC عبر الويب** هو تطبيق ويب متكامل بملف واحد تم تطويره بواسطة **فريق TRL للتطوير (TRL TEAM FOR DEVELOPMENT)**. يعتمد التطبيق على **Web NFC API** لمسح وقراءة علامات NFC مباشرة من خلال المتصفح، بالإضافة إلى الربط مع قاعدة بيانات **Firebase Firestore** لتسجيل كل عملية مسح في السحابة بشكل فوري.

صُمم التطبيق لتحليل سجلات **NDEF** القياسية، ويتميز بآلية ذكية للتنبيه عند محاولة قراءة بطاقة غير مدعومة (مثل البطاقات البنكية). يتم إرسال بيانات كل مسح (الرقم التسلسلي، نوع البطاقة، البيانات المستخرجة، ووقت المسح) إلى قاعدة البيانات لمراقبتها وتحليلها.

### ✨ المميزات الرئيسية
- **تسجيل سحابي فوري:** إرسال بيانات المسح مباشرة إلى قاعدة بيانات Firebase Firestore.
- **دعم اللغتين:** التبديل بسلاسة بين اللغتين الإنجليزية (الافتراضية) والعربية مع دعم كامل لاتجاه النص (RTL/LTR).
- **اكتشاف ذكي:** قراءة وتحليل الروابط، النصوص، وأنواع MIME، مع التمييز بين علامات NDEF والبطاقات الذكية المشفرة (مثل البطاقات البنكية).
- **تصميم عصري:** واجهة مستخدم بسيطة (أبيض، أسود، رمادي) مع شاشة تحميل احترافية تحمل اسم الفريق.
- **ملف واحد:** الكود بالكامل (HTML, CSS, JS) موجود في ملف `index.html` واحد لسهولة النشر.

### ⚙️ المتطلبات والقيود
> **تنبيه هام:** تقنية Web NFC لا تزال في مرحلة المسودة، ولها قيود صارمة:
- **الجهاز:** يجب أن يكون جهاز **أندرويد (Android)** يحتوي على شريحة NFC.
- **المتصفح:** يتطلب متصفح **Google Chrome**. **لا يدعم** أجهزة iOS أو متصفحات الكمبيوتر.
- **الأمان:** يجب استضافة الموقع على خادم يدعم **HTTPS**.

### 🚀 كيفية النشر والاستخدام
1. قم بنسخ كود `index.html` إلى مستودعك.
2. تأكد من إنشاء مشروع في Firebase وتفعيل Firestore (في وضع الاختبار).
3. ضع إعدادات مشروعك في الكائن `firebaseConfig` الموجود داخل الكود.
4. ارفع الملف على استضافة تدعم HTTPS (مثل GitHub Pages).
5. افتح الرابط من هاتف أندرويد باستخدام متصفح Chrome.

---

## 👨‍💻 Team & Credits
- **Developed by:** TRL TEAM FOR DEVELOPMENT
- **Team Leader:** Taimdev9
- **Technologies:** HTML5, CSS3, JavaScript (ES6), Web NFC API, Firebase Firestore.

<div align="center">
  <br>
  <i>Built with ❤️ by TRL TEAM</i>
</div>