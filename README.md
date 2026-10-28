
```markdown
<div align="center">

# 📡 NFC Web Scanner & Logger
### By TRL TEAM FOR DEVELOPMENT

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Firebase](https://img.shields.io/badge/Firebase-039BE5?style=for-the-badge&logo=Firebase&logoColor=white)](https://firebase.google.com/)
[![Web NFC](https://img.shields.io/badge/Web_NFC-API-blue?style=for-the-badge)](https://w3c.github.io/web-nfc/)

**A lightweight, bilingual, browser-based NFC scanner with real-time cloud logging.**

</div>

---

## 🇬🇧 English Documentation

### 📖 About The Project
**NFC Web Scanner & Logger** is an advanced single-file web application developed by **TRL TEAM FOR DEVELOPMENT**. It utilizes the **Web NFC API** to scan and decode NFC tags directly through the browser without requiring a native mobile app.

What sets this project apart is its integration with **Firebase Firestore**. Every scan is securely logged to a cloud database, allowing administrators to track scan history, card types, and timestamps in real-time.

### ✨ Key Features
- **Cloud Logging (Firebase):** Automatically saves scan data (Serial Number, Type, Content, Timestamp) to a Firestore database.
- **Bilingual Support:** Seamlessly switch between English (Default) and Arabic with full RTL/LTR layout support.
- **Sleek UI/UX:** Minimalist black, white, and gray design with a professional loading screen.
- **Smart Detection:** Decodes URLs, Text, MIME types, Smart Posters, and Absolute URLs.
- **Bank Card Alert:** Detects unsupported cards (like bank cards) and informs the user that sensitive data cannot be read via the browser.
- **Single File Architecture:** The entire frontend (HTML, CSS, JS) is bundled into one `index.html` file for easy deployment.

### ⚙️ Prerequisites & Limitations
> **Important:** Web NFC is currently a working draft and has strict limitations:
- **Device:** Must be an **Android** device with NFC hardware.
- **Browser:** Requires **Google Chrome** (or Chromium-based browsers). It is **NOT** supported on iOS (Safari) or Desktop.
- **Security:** The website **MUST** be served over **HTTPS**.
- **Privacy:** The API cannot read encrypted bank card data.

### 🚀 Setup & Installation
1. Clone this repository or download the `index.html` file.
2. Create a project on [Firebase Console](https://console.firebase.google.com/).
3. Set up a **Cloud Firestore** database (Start in *Test Mode* initially).
4. Register a Web App in Firebase and copy your `firebaseConfig` object.
5. Open `index.html` and replace the `firebaseConfig` in the `<script type="module">` section with your own credentials.
6. Host the file on GitHub Pages, Vercel, or Firebase Hosting.

### 🛡️ Securing Your Database (Firestore Rules)
After testing, update your Firestore Rules to allow writing but prevent public reading:
```javascript
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /nfc_scans/{document=**} {
      allow create: if true;  // Allows the app to write data
      allow read: if false;   // Hides data from the public web
    }
  }
}
```

---

🇸🇦 التوثيق العربي

📖 عن المشروع

قارئ ومسجل NFC عبر الويب هو تطبيق ويب متقدم بملف واحد، تم تطويره بواسطة فريق TRL للتطوير (TRL TEAM FOR DEVELOPMENT). يعتمد التطبيق على Web NFC API لمسح وقراءة علامات NFC مباشرة من خلال المتصفح، دون الحاجة لتثبيت تطبيق خارجي.

ما يميز هذا المشروع هو ربطه بقاعدة بيانات Firebase Firestore. يتم تسجيل كل عملية مسح في السحابة، مما يسمح للمطورين أو الإداريين بتتبع سجل المسح، أنواع البطاقات، وأوقات المسح في الوقت الفعلي.

✨ المميزات الرئيسية

· التسجيل السحابي (Firebase): حفظ تلقائي لبيانات المسح (الرقم التسلسلي، النوع، المحتوى، الوقت) في قاعدة بيانات Firestore.
· دعم اللغتين: التبديل بسلاسة بين اللغتين الإنجليزية (الافتراضية) والعربية مع دعم كامل لاتجاه النص (RTL/LTR).
· تصميم عصري وبسيط: واجهة مستخدم تعتمد على الألوان الأساسية (الأبيض، الأسود، الرمادي) مع شاشة تحميل احترافية.
· اكتشاف ذكي: قراءة وتحليل الروابط، النصوص، أنواع MIME، والملصقات الذكية.
· تنبيه البطاقات البنكية: يكتشف التطبيق البطاقات غير المدعومة ويبلغ المستخدم بعدم إمكانية قراءة بياناتها الحساسة.
· ملف واحد: الكود بالكامل (HTML, CSS, JS) موجود في ملف index.html واحد لسهولة النشر.

⚙️ المتطلبات والقيود

تنبيه هام: تقنية Web NFC لا تزال في مرحلة المسودة، ولها قيود صارمة:

· الجهاز: يجب أن يكون جهاز أندرويد (Android) يحتوي على شريحة NFC.
· المتصفح: يتطلب متصفح Google Chrome (أو المتصفحات المبنية على Chromium). لا يدعم أجهزة iOS أو متصفحات الكمبيوتر.
· الأمان: يجب استضافة الموقع على خادم يدعم HTTPS.
· الخصوصية: لا يمكن للتطبيق قراءة البيانات المشفرة للبطاقات البنكية.

🚀 التثبيت والتشغيل

1. قم بنسخ (Clone) هذا المستودع أو تحميل ملف index.html.
2. أنشئ مشروعاً جديداً في Firebase Console.
3. قم بتفعيل Cloud Firestore (اختر وضع الاختبار Test Mode في البداية).
4. سجل تطبيق ويب (Web App) في Firebase وانسخ كود firebaseConfig.
5. افتح ملف index.html واستبدل كود firebaseConfig بكودك الخاص داخل وسم <script type="module">.
6. ارفع الملف على GitHub Pages أو Vercel أو Firebase Hosting.

🛡️ تأمين قاعدة البيانات (Firestore Rules)

بعد الانتهاء من التجربة، قم بتحديث قواعد الحماية (Rules) في Firebase للسماح بالكتابة ومنع القراءة العامة:

```javascript
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /nfc_scans/{document=**} {
      allow create: if true;  // يسمح للتطبيق بحفظ البيانات
      allow read: if false;   // يخفي البيانات عن المتصفحات العامة
    }
  }
}
```

---

👨‍💻 Team & Credits

· Developed by: TRL TEAM FOR DEVELOPMENT
· Team Leader: Taimdev9
· Project Type: Web NFC Integration & Firebase Backend

<div align="center">
  <br>
  <i>Built with ❤️ by TRL TEAM</i>
</div>
```