# 📚 Personalized IELTS Tracker

<div align="center">

**A fully personalized, offline-capable IELTS preparation tracker — built as a single HTML file with Firebase real-time sync.**

[![Live Demo](https://img.shields.io/badge/Live_Demo-Visit_App-blue?style=for-the-badge)](https://jahid-ielts-tracker.netlify.app)
[![Firebase](https://img.shields.io/badge/Firebase-Firestore-orange?style=for-the-badge&logo=firebase)](https://firebase.google.com/)
[![Netlify](https://img.shields.io/badge/Deployed_on-Netlify-00c7b7?style=for-the-badge&logo=netlify)](https://netlify.com)

</div>

---

## ✨ Features

| Feature | Description |
|---|---|
| 📅 **4-Phase Study Plan** | A full 20-week plan from Sep 2026 → Jan 2027: Foundation, Skill Building, Mock Tests, Final Polish |
| ✅ **Daily Task Tracking** | Check off tasks each day with instant visual feedback and real-time progress updates |
| 🔥 **Streak Counter** | Tracks your daily study streak to keep you motivated |
| 🗓️ **Interactive Calendar** | Visual calendar showing completed days, mock test days, and exam date |
| 📊 **Progress Dashboard** | Phase-by-phase progress bars, overall completion %, and score trend charts |
| 🎯 **Score Tracker** | Log Listening/Reading/Writing/Speaking scores from each mock test |
| 📝 **Error Log** | Keep track of mistakes and their solutions for targeted revision |
| ⚡ **Real-time Sync** | Firebase Firestore real-time listener — updates instantly across all your devices |
| 📱 **Mobile Responsive** | Fully usable on iPhone, Android, tablet, and desktop |
| 🌙 **Dark Mode UI** | Elegant dark theme with Bengali (বাংলা) language UI |

---

## 🚀 Tech Stack

- **Frontend:** Vanilla HTML + CSS + JavaScript — **zero build step, single file**
- **Database:** Firebase Firestore (real-time `onSnapshot` listener)
- **Charts:** Chart.js v4
- **Fonts:** Google Fonts — Hind Siliguri + Inter
- **Hosting:** Netlify (free tier)

---

## 🗺️ Study Plan Overview

| Phase | Period | Focus |
|---|---|---|
| 🌱 Phase 1 — Foundation | Sep 1 – Oct 5, 2026 | Grammar, Core Vocabulary, Basics |
| 🏗️ Phase 2 — Skill Building | Oct 6 – Nov 16, 2026 | Section-wise intensive practice |
| 🧪 Phase 3 — Mock Tests | Nov 17 – Dec 28, 2026 | Full mocks + error analysis |
| 🏁 Phase 4 — Final Polish | Dec 29, 2026 – Jan 24, 2027 | Revision, weak areas, exam ready |
| 🎯 **IELTS Exam** | **Jan 25, 2027** | **Target: Band 7.0** |

---

## 🔧 Setup & Self-Hosting

### Option 1 — Open locally
```bash
git clone https://github.com/jahidstm/personalized_ielts-tracker.git
start ielts-tracker.html
```

### Option 2 — Deploy to Netlify (free)
1. Go to [Netlify Drop](https://app.netlify.com/drop) and drag the `ielts-tracker.html` file
2. Done ✅

### Option 3 — Connect your own Firebase
1. Create a project at [Firebase Console](https://console.firebase.google.com/)
2. Enable **Firestore Database** in Test Mode
3. Copy your Firebase config and replace the `firebaseConfig` object inside `ielts-tracker.html`
4. Set Firestore Rules to allow permanent access:
```javascript
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /{document=**} {
      allow read, write: if true;
    }
  }
}
```

---

## 🎯 Goal

| | |
|---|---|
| **Exam Date** | January 25, 2027 |
| **Target Band** | 7.0 |
| **Study Duration** | ~20 weeks (Sep 2026 – Jan 2027) |

---

## 📄 License

MIT License — feel free to fork and adapt for your own IELTS journey!

---

<div align="center">
Made with ❤️ for IELTS preparation &nbsp;·&nbsp; Good luck on your journey! 🎓
</div>
