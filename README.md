
```markdown
<div align="center">

# 📡 TRL NFC Pro

### By TRL TEAM FOR DEVELOPMENT

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com/)
[![Web NFC](https://img.shields.io/badge/Web_NFC-API-blue?style=for-the-badge)](https://w3c.github.io/web-nfc/)

**A comprehensive, bilingual, cloud-connected NFC Reader & Writer application.**

</div>

---

## 🇬🇧 English Documentation

### 📖 About The Project
**TRL NFC Pro** is an advanced, single-file web application developed by **TRL TEAM FOR DEVELOPMENT**. It leverages the **Web NFC API** to scan, decode, and write NFC tags directly through the mobile browser, completely eliminating the need for native mobile apps.

The application logs every interaction (read or write) securely to a **Firebase Firestore** database, capturing real-time data including timestamps and geolocation. It also features a built-in, secure Admin Dashboard to review the collected data.

### ✨ Key Features
- **NFC Reader:** Decodes standard NDEF records (URLs, Text, MIME types) and intelligently detects unsupported cards (like bank cards) to protect sensitive data.
- **NFC Writer:** Allows users to write custom URLs or Text directly to empty NFC tags (e.g., NTAG213).
- **Cloud Logging:** Automatically sends scan/write data to Firebase Firestore.
- **Geolocation Tagging:** Captures the user's approximate location (Latitude/Longitude) upon scanning (requires user permission).
- **Audio & Haptic Feedback:** Plays a beep and vibrates the device upon a successful action.
- **Admin Dashboard:** A built-in, password-protected control panel to view all logged data directly from the web interface.
- **PWA Ready:** Can be installed on the home screen as a standalone Progressive Web App.
- **Bilingual:** Full support for English and Arabic with RTL/LTR switching.

### ⚙️ Prerequisites & Limitations
> **Important:** Web NFC is currently a working draft and has strict limitations:
- **Device:** Must be an **Android** device with NFC hardware.
- **Browser:** Requires **Google Chrome** (or Chromium-based browsers). It is **NOT** supported on iOS (Safari) or Desktop browsers.
- **Security:** The website **MUST** be served over **HTTPS**.
- **Privacy:** The API is strictly blocked from reading encrypted financial data (Bank Cards).

### 🚀 How to Deploy
1. Clone the repository or download the `index.html` file.
2. Create a project on **Firebase Console** and enable **Firestore Database**.
3. Obtain your Firebase configuration keys and replace the placeholder `firebaseConfig` object in the code.
4. Set up the Firestore Security Rules (provided below).
5. Host the file on a secure HTTPS server (like GitHub Pages, Vercel, or Netlify).
6. Open the link on an Android device using Chrome.

---

## 🇸🇦 التوثيق العربي

### 📖 عن المشروع
**TRL NFC Pro** هو تطبيق ويب متكامل ومتقدم بملف واحد، تم تطويره بواسطة **فريق TRL للتطوير (TRL TEAM FOR DEVELOPMENT)**. يعتمد التطبيق على **Web NFC API** لمسح وقراءة وكتابة علامات NFC مباشرة من خلال متصفح الهاتف، مما يغني عن استخدام تطبيقات أخرى.

يقوم التطبيق بتسجيل كل عملية (قراءة أو كتابة) في قاعدة بيانات **Firebase Firestore** السحابية، مع حفظ الوقت وتاريخ العملية والموقع الجغرافي التقريبي. كما يتميز بوجود لوحة تحكم سرية (Admin Dashboard) لمطور التطبيق لمراجعة البيانات.

### ✨ المميزات الرئيسية
- **قارئ NFC:** يقرأ سجلات NDEF القياسية (روابط، نصوص، وأنواع MIME) ويكتشف البطاقات غير المدعومة (مثل البطاقات البنكية) لحماية الخصوصية.
- **كاتب NFC:** يسمح للمستخدم بكتابة روابط أو نصوص مخصصة على علامات NFC الفارغة.
- **تسجيل سحابي:** إرسال بيانات المسح والكتابة تلقائياً إلى قاعدة بيانات Firebase.
- **الموقع الجغرافي:** يلتقط إحداثيات (خط الطول والعرض) عند المسح (بعد إذن المستخدم).
- **تفاعل حسي:** إصدار صوت "بيب" واهتزاز الهاتف عند نجاح العملية.
- **لوحة تحكم (Admin):** واجهة محمية بكلمة مرور لمطور التطبيق لاستعراض جميع البيانات المسجلة.
- **تطبيق ويب (PWA):** قابل للتثبيت على الشاشة الرئيسية ويعمل كتطبيق مستقل.
- **دعم اللغتين:** تبديل سلس بين العربية والإنجليزية مع دعم اتجاه النص (RTL/LTR).

### ⚙️ المتطلبات والقيود
> **تنبيه هام:** تقنية Web NFC لا تزال في مرحلة المسودة، ولها قيود صارمة:
- **الجهاز:** يجب أن يكون جهاز **أندرويد (Android)** يحتوي على شريحة NFC.
- **المتصفح:** يتطلب متصفح **Google Chrome**. **لا يدعم** أجهزة iOS أو متصفحات الكمبيوتر.
- **الأمان:** يجب استضافة الموقع على خادم يدعم **HTTPS**.

### 🚀 كيفية النشر
1. قم بنسخ كود `index.html` إلى مستودعك.
2. أنشئ مشروعاً في Firebase وفعل خدمة Firestore.
3. ضع مفاتيحك الخاصة (Firebase Config) في الكود بدلاً من القيم الافتراضية.
4. قم بتطبيق قواعد الحماية (Rules) الموضحة أدناه.
5. ارفع الملف على استضافة تدعم HTTPS (مثل GitHub Pages).
6. افتح الرابط من هاتف أندرويد باستخدام متصفح Chrome.

---

## 🛡️ Firestore Security Rules

To ensure the app works perfectly, apply these rules in your Firebase Console:

```javascript
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /nfc_scans/{document} {
      allow create: if true; // Allow writing new logs
      allow read: if true;   // Allow reading for the Admin Dashboard
      allow update, delete: if false; // Prevent tampering
    }
  }
}
```

---

👨‍💻 Team & Credits

· Developed by: TRL TEAM FOR DEVELOPMENT
· Team Leader: Taimdev9
· Technologies: HTML5, CSS3, JavaScript (ES6), Web NFC API, Firebase Firestore, PWA.

<div align="center">
  <br>
  <i>Built with ❤️ by TRL TEAM</i>
</div>
```