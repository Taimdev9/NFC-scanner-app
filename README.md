<div align="center">

# 📡 TRL NFC Pro
### Advanced Web-Based NFC Reader, Writer & Cloud Logger

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com/)
[![Web NFC](https://img.shields.io/badge/Web_NFC-API-blue?style=for-the-badge)](https://w3c.github.io/web-nfc/)

**Developed by TRL TEAM FOR DEVELOPMENT - Led by Taimdev9**

</div>

---

## 🇬🇧 English Documentation

### 📖 About The Project
**TRL NFC Pro** is a comprehensive, single-file web application that utilizes the **Web NFC API** to read and write NFC tags directly from the browser. It features a sleek bilingual interface (English/Arabic), real-time Cloud logging via **Firebase Firestore**, Geolocation tracking, and a secure Admin Dashboard for monitoring. 

### ✨ Key Features
- **Read & Write Modes:** Seamlessly switch between reading NDEF tags (URLs, Text) and writing new data to empty tags.
- **Cloud Logging (Firebase):** Automatically logs every scan (Serial Number, Type, Timestamp, and Geolocation) to Firestore.
- **Secure Admin Dashboard:** Access a hidden dashboard via `?admin=true` to view all scanned data, protected by a password.
- **Smart Detection:** Differentiates between standard NDEF tags and encrypted smart cards (e.g., Bank Cards) without exposing sensitive data.
- **Haptic & Audio Feedback:** Vibrates and plays a beep upon successful scans/writes.
- **PWA Ready:** Installable on mobile devices for a native app-like experience.
- **Bilingual UI:** Full English and Arabic support with RTL/LTR layouts.

### ⚙️ Prerequisites
- **Device:** Android smartphone with NFC hardware.
- **Browser:** Google Chrome (or Chromium-based).
- **Hosting:** Must be served over **HTTPS** (e.g., GitHub Pages, Vercel).
- **Backend:** A Firebase project with Firestore enabled.

### 🚀 How to Deploy
1. **Clone the repository** or download `index.html`.
2. **Configure Firebase:**
   - Go to your Firebase Console, create a Web App, and copy the `firebaseConfig` object.
   - Open `index.html` and replace the `firebaseConfig` placeholder with your actual credentials.
3. **Setup Firestore Rules:**
   - Go to Firestore > Rules and paste the necessary security rules to allow write/read access (as per your project requirements).
4. **Change Admin Password:**
   - In the JavaScript code, find `const adminPass = "YOUR_SECURE_PASSWORD";` and change it to your own strong password.
5. **Host the File:** Upload `index.html` to GitHub Pages or any HTTPS-enabled hosting.
6. **Access:** Open the link on your Android device. To view the dashboard, append `?admin=true` to the URL.

---

## 🇸🇦 التوثيق العربي

### 📖 عن المشروع
**TRL NFC Pro** هو تطبيق ويب متكامل بملف واحد، يستخدم **Web NFC API** لقراءة وكتابة علامات NFC مباشرة من المتصفح. يتميز بواجهة ثنائية اللغة (عربي/إنجليزي)، تسجيل سحابي فوري عبر **Firebase Firestore**، تتبع الموقع الجغرافي، ولوحة تحكم سرية لمراقبة البيانات.

### ✨ المميزات الرئيسية
- **أوضاع القراءة والكتابة:** التبديل بسهولة بين قراءة العلامات (روابط، نصوص) وكتابة بيانات جديدة على العلامات الفارغة.
- **التسجيل السحابي (Firebase):** حفظ تلقائي لبيانات كل مسح (الرقم التسلسلي، النوع، الوقت، والموقع الجغرافي) في Firestore.
- **لوحة تحكم سرية:** الوصول إلى لوحة تحكم مخفية عبر إضافة `?admin=true` للرابط، محمية بكلمة مرور لعرض البيانات.
- **اكتشاف ذكي:** التمييز بين علامات NDEF القياسية والبطاقات الذكية المشفرة (مثل البطاقات البنكية) دون كشف البيانات الحساسة.
- **تفاعل حسي:** اهتزاز الهاتف وإصدار صوت عند نجاح القراءة أو الكتابة.
- **دعم PWA:** إمكانية تثبيت الموقع كتطبيق على شاشة الهاتف الرئيسية.
- **دعم اللغتين:** دعم كامل للغتين العربية والإنجليزية مع اتجاه النص المناسب (RTL/LTR).

### ⚙️ المتطلبات الأساسية
- **الجهاز:** هاتف أندرويد يحتوي على شريحة NFC.
- **المتصفح:** Google Chrome (أو ما يعتمد عليه).
- **الاستضافة:** يجب استضافة الموقع على خادم يدعم **HTTPS** (مثل GitHub Pages).
- **قاعدة البيانات:** مشروع Firebase مع تفعيل خدمة Firestore.

### 🚀 كيفية النشر
1. **نسخ الكود:** قم بتحميل ملف `index.html` أو استنساخ المستودع.
2. **إعداد Firebase:**
   - اذهب إلى لوحة تحكم Firebase، وأنشئ تطبيق ويب، وانسخ كائن `firebaseConfig`.
   - افتح ملف `index.html` واستبدل إعدادات Firebase التجريبية بإعداداتك الحقيقية.
3. **إعداد قواعد Firestore:**
   - اذهب إلى Firestore > Rules وضع القواعد الأمنية المناسبة للسماح بالقراءة والكتابة.
4. **تغيير كلمة مرور المسؤول:**
   - في كود الـ JavaScript، ابحث عن `const adminPass = "YOUR_SECURE_PASSWORD";` واستبدلها بكلمة مرور قوية خاصة بك.
5. **الرفع:** ارفع ملف `index.html` إلى GitHub Pages أو أي استضافة تدعم HTTPS.
6. **الدخول:** افتح الرابط على هاتف الأندرويد. للوصول إلى لوحة التحكم، أضف `?admin=true` إلى نهاية الرابط.

---

## 👨‍💻 Team & Credits
- **Developed by:** TRL TEAM FOR DEVELOPMENT
- **Team Leader:** Taimdev9
- **Technologies:** HTML5, CSS3, Vanilla JavaScript, Web NFC API, Firebase Firestore, PWA.

<div align="center">
  <br>
  <i>Built with ❤️ by TRL TEAM</i>
</div>