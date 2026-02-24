# Changelog

Alle belangrijke wijzigingen aan dit project worden gedocumenteerd in dit bestand.

Het formaat is gebaseerd op [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
en dit project volgt [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2025-02-24

### 🎉 Initial Release

Eerste productie-versie van de Basis-Fit Workout Tracker!

### ✨ Added

#### Core Features
- **Workout Tracking** - Volledig werkende workout tracking systeem
- **Programma's** - 5 vooraf ingestelde trainingsschema's (Push/Pull/Legs, Upper/Lower, Full Body)
- **Open Training** - Dynamisch oefeningen toevoegen tijdens je workout
- **PR Tracking** - Automatische detectie en opslag van persoonlijke records
- **Sessie Geschiedenis** - Bekijk je laatste 10 trainingen met details

#### Authentication & Sync
- **Firebase Authentication** - Google Sign-In + Email/Password registratie
- **Cloud Sync** - Real-time data synchronisatie via Firestore
- **Multi-device Support** - Log in op elk apparaat en synchroniseer automatisch
- **Offline Support** - Lokale caching voor offline gebruik

#### User Experience
- **Rust Timer** - Instelbare rust timer (30s - 5min) met notificaties
- **Wake Lock** - Screen blijft aan tijdens trainingen
- **Confetti Animatie** - Bij afronden van workouts en nieuwe PR's
- **Dark Mode Support** - Navy-gebaseerd kleurenschema
- **Responsive Design** - Perfect op mobile, tablet en desktop

#### Sharing & Social
- **Workout Cards** - Genereer visuele workout cards
- **Instagram Stories** - Direct delen naar Instagram
- **Custom Achtergronden** - Gebruik je eigen foto's of maak een foto
- **Native Share API** - Deel via elke geïnstalleerde app

#### Customization
- **Eigen Schema's** - Maak en bewaar je eigen trainingsschema's
- **Custom Machines** - Voeg je eigen oefeningen toe aan de lijst
- **Avatar Keuze** - Kies uit 20 emoji avatars
- **Profiel Personalisatie** - Stel je naam en voorkeuren in

#### Legal & Documentation
- **Privacybeleid** - Volledige AVG/GDPR compliant privacy policy
- **Gebruiksvoorwaarden** - Duidelijke terms of service
- **Over Pagina** - App info, features en technologie details
- **README** - Uitgebreide documentatie voor developers

### 🎨 Design
- Modern, clean interface met Syne & DM Sans fonts
- Smooth animaties en transitions
- Intuïtieve UX met bottom navigation
- Card-based design met subtle shadows
- Navy/Blue accent kleurenschema

### 🔒 Security
- Firebase Security Rules geïmplementeerd
- HTTPS-only via Vercel
- Security headers (CSP, XSS Protection, etc.)
- Per-user data isolation
- Wachtwoord minimaal 6 karakters

### 📱 PWA
- Installeerbaar op home screen
- App manifest geconfigureerd
- Offline-ready met service worker
- Apple Touch Icons
- Theme color support

### 🚀 Performance
- Single-file architecture (~120KB)
- Lazy loading waar mogelijk
- Optimized animations (CSS transforms)
- Efficient Firebase queries
- Local storage caching

### 🛠️ Technical
- **Frontend:** Vanilla JavaScript (ES6+), HTML5, CSS3
- **Backend:** Firebase (Auth, Firestore, Analytics)
- **Hosting:** Vercel with custom configuration
- **Version Control:** Git + GitHub
- **Build:** No build process (single HTML file)

### 📊 Analytics
- Firebase Analytics geïntegreerd
- Anonieme gebruiksstatistieken
- Event tracking voor belangrijke acties

### 🌍 Localization
- Volledig in het Nederlands
- Nederlandse datumnotatie
- Aangepaste foutmeldingen

---

## [Unreleased]

### 🔮 Planned Features
- Workout statistieken en grafieken
- Week/maand overzichten
- Streak tracking (x dagen op rij getraind)
- Badge/achievement system
- Export naar CSV/PDF
- Social features (vrienden, challenges)
- Dark mode toggle
- Multiple language support
- Progressive overload suggesties

### 🐛 Known Issues
Geen bekende kritieke issues op dit moment.

---

## Versie Nummering

We gebruiken [SemVer](http://semver.org/) voor versie nummering:
- **MAJOR** - Incompatibele API wijzigingen
- **MINOR** - Nieuwe features (backwards compatible)
- **PATCH** - Bug fixes (backwards compatible)

## Feedback & Contributies

Suggesties of bugs gevonden? Open een issue op GitHub!

---

**Laatst bijgewerkt:** 24 februari 2025
