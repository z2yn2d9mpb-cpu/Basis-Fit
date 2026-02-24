# 💪 Basis-Fit Workout Tracker

Een moderne, progressieve web applicatie voor het bijhouden van je fitness trainingen, programma's en persoonlijke records. Ontwikkeld met vanilla JavaScript en Firebase voor real-time synchronisatie tussen al je apparaten.

![Basis-Fit App](https://img.shields.io/badge/Status-Live-success)
![Version](https://img.shields.io/badge/Version-1.0.0-blue)
![License](https://img.shields.io/badge/License-Proprietary-red)

## 🌐 Live Demo

**Website:** [https://basis-fit.vercel.app/](https://basis-fit.vercel.app/)

## ✨ Features

### 🏋️ Workout Tracking
- **Vooraf ingestelde programma's** - Kies uit meerdere kant-en-klare trainingsschema's
- **Open Training** - Voeg dynamisch oefeningen toe tijdens je workout
- **Real-time voortgang** - Zie direct je volledige volume, sets en voltooide oefeningen
- **PR Tracking** - Automatische detectie van persoonlijke records met 🏆 badge
- **Rust timer** - Instelbare rust timer met notificaties

### 📊 Data & Analytics
- **Sessie geschiedenis** - Bekijk je laatste 10 trainingen
- **Volume tracking** - Totaal gewicht × reps per sessie
- **Voortgangsinzicht** - Zie je ontwikkeling over tijd
- **Cloud sync** - Al je data wordt automatisch gesynchroniseerd via Firebase

### 🎨 Delen & Social
- **Workout Cards** - Genereer visueel aantrekkelijke workout cards
- **Instagram Stories** - Direct delen naar Instagram
- **Custom achtergronden** - Gebruik je eigen foto's of camera
- **Native share** - Deel via alle geïnstalleerde apps

### ⚙️ Aanpasbaar
- **Eigen schema's** - Maak je eigen trainingsschema's
- **Custom machines** - Voeg je eigen oefeningen toe
- **Profiel personalisatie** - Kies je avatar en naam
- **Timer instellingen** - Stel je eigen rust duur in (30s - 5min)

### 📱 PWA Features
- **Installeerbaar** - Voeg toe aan je home screen
- **Offline-ready** - Werkt zonder internet
- **Wake Lock** - Screen blijft aan tijdens training
- **Responsive design** - Perfect op alle apparaten

## 🚀 Tech Stack

- **Frontend:** Vanilla JavaScript (ES6+), HTML5, CSS3
- **Backend:** Firebase
  - Authentication (Google + Email/Password)
  - Firestore (Real-time database)
  - Analytics
- **Hosting:** Vercel
- **Version Control:** Git / GitHub

## 🔒 Security

- ✅ Firebase Security Rules ingesteld
- ✅ Gebruikers kunnen alleen hun eigen data lezen/schrijven
- ✅ Authentication vereist voor alle acties
- ✅ HTTPS-only
- ✅ Security headers via Vercel configuratie

## 📦 Project Structuur

```
basis-fit/
├── index.html          # Volledige single-page app
├── README.md           # Project documentatie
├── .gitignore         # Git ignore configuratie
├── vercel.json        # Vercel deployment configuratie
└── docs/              # Documentatie (indien aanwezig)
```

## 🛠️ Lokale Development

### Vereisten
- Moderne browser (Chrome, Firefox, Safari, Edge)
- Geen build tools nodig - het is een single HTML file!

### Setup

1. **Clone de repository**
   ```bash
   git clone https://github.com/jouw-username/basis-fit.git
   cd basis-fit
   ```

2. **Open de app**
   - Open `index.html` direct in je browser, of
   - Start een lokale server:
     ```bash
     python -m http.server 8000
     # Of met Node.js
     npx serve
     ```

3. **Open in browser**
   - Navigeer naar `http://localhost:8000`

### Firebase Configuratie

De Firebase configuratie staat in `index.html` (regel 2551-2559). Dit is **openbaar** en **veilig** - Firebase API keys zijn bedoeld om publiek te zijn. De beveiliging komt van:
- Firestore Security Rules
- Authentication requirements
- Domain restrictions (via Firebase Console)

## 📝 Firebase Security Rules

```javascript
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /users/{userId} {
      allow read, write: if request.auth != null 
                         && request.auth.uid == userId;
    }
  }
}
```

## 🚀 Deployment

### Vercel (Huidige methode)

1. Push naar GitHub
2. Vercel detecteert automatisch wijzigingen
3. Automatische deployment naar productie

**Live URL:** https://basis-fit.vercel.app/

### Handmatige Deployment

```bash
# Installeer Vercel CLI
npm i -g vercel

# Deploy
vercel

# Productie deployment
vercel --prod
```

## 📊 Performance

- ⚡ **Lighthouse Score:** 95+
- 📦 **Bundle Size:** ~120KB (single HTML file)
- 🚀 **First Contentful Paint:** < 1s
- 📱 **PWA Ready:** Ja
- ♿ **Accessibility:** WCAG 2.1 AA compliant

## 🤝 Contributing

Dit is momenteel een persoonlijk project. Contributies zijn niet actief gezocht, maar suggesties zijn welkom via issues.

## 📄 Licentie

**Proprietary** - Alle rechten voorbehouden. Dit project is niet open source.

Voor commercieel gebruik of licentievragen, neem contact op.

## 🔗 Links

- **Live App:** [https://basis-fit.vercel.app/](https://basis-fit.vercel.app/)
- **Privacybeleid:** [https://basis-fit.vercel.app/#privacy](https://basis-fit.vercel.app/#privacy)
- **Gebruikersvoorwaarden:** [https://basis-fit.vercel.app/#terms](https://basis-fit.vercel.app/#terms)

## 📧 Contact

Voor vragen, feedback of support: Open een issue in deze repository.

## 🙏 Acknowledgments

- **Firebase** - Backend infrastructure
- **Vercel** - Hosting platform
- **Google Fonts** - Syne & DM Sans typography

---

**Versie:** 1.0.0  
**Laatst bijgewerkt:** Februari 2025  
**Status:** ✅ Live in productie
