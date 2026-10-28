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
