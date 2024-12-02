# EventForge

**Forge your perfect events with ease!**

EventForge ist eine moderne Event-Management-Anwendung, die mit React, TailwindCSS und einer RESTful API erstellt wurde. Dieses Projekt dient dazu, Fähigkeiten in React, Routing, API-Integration und LocalStorage zu vertiefen.

## Features

- **Eventübersicht und -details**: Übersichtliche Darstellung von Events mit detaillierten Informationen.
- **Benutzerregistrierung und Anmeldung**: Sichere und benutzerfreundliche Authentifizierung.
- **Event-Erstellung**: Geschützte Funktionalität, um Events zu erstellen, verfügbar nur für angemeldete Benutzer mit gültigem API-Token.

## Technologien

- **React**: Frontend-Framework für die Benutzeroberfläche.
- **TailwindCSS**: Stilbibliothek für schnelles und flexibles Design.
- **React Router DOM**: Routing und Navigation.
- **RESTful API**: Interaktion mit realen Daten über CRUD-Operationen.

## Ziel

Benutzerfreundliche und intuitive Event-Verwaltung für Entwickler und Anwender gleichermaßen.

## Installation

### 1. Projekt einrichten
1. **Erstelle ein neues React-Projekt**:
   ```bash
   npx create-react-app eventforge --template cra-template-pwa
   cd eventforge
   ```
2. **Entferne unnötige Dateien**: Lösche ggf. Dateien wie `App.css` und passe die Struktur an.

### 2. TailwindCSS installieren und einrichten
1. **Installiere TailwindCSS und PostCSS**:
   ```bash
   npm install -D tailwindcss postcss autoprefixer
   npx tailwindcss init
   ```
2. **Konfiguriere `tailwind.config.js`**:
   ```javascript
   module.exports = {
     content: ["./src/**/*.{js,jsx,ts,tsx}"],
     theme: {
       extend: {},
     },
     plugins: [],
   };
   ```
3. **Erstelle die `tailwind.css` in `src/`**:
   ```css
   @tailwind base;
   @tailwind components;
   @tailwind utilities;
   ```
4. **Importiere Tailwind in deine App**:
   Öffne `src/index.css` und füge Folgendes hinzu:
   ```css
   @import './tailwind.css';
   ```

### 3. DaisyUI hinzufügen
1. **Installiere DaisyUI**:
   ```bash
   npm install daisyui
   ```
2. **Aktiviere DaisyUI in der Tailwind-Konfiguration**:
   ```javascript
   module.exports = {
     content: ["./src/**/*.{js,jsx,ts,tsx}"],
     theme: {
       extend: {},
     },
     plugins: [require('daisyui')],
   };
   ```
3. **Optional: DaisyUI-Themen anpassen**:
   ```javascript
   daisyui: {
     themes: ["light", "dark", "cupcake"],
   },
   ```

### 4. Font Awesome Icons einbinden
1. **Installiere Font Awesome**:
   ```bash
   npm install @fortawesome/fontawesome-svg-core @fortawesome/free-solid-svg-icons @fortawesome/react-fontawesome
   ```
2. **Nutze Icons in deiner App**:
   ```javascript
   import { FontAwesomeIcon } from '@fortawesome/react-fontawesome';
   import { faCalendarAlt } from '@fortawesome/free-solid-svg-icons';

   function IconExample() {
     return <FontAwesomeIcon icon={faCalendarAlt} className="text-blue-500" />;
   }
   ```

## Starten und Testen
1. **Start des Projekts**:
   ```bash
   npm start
   ```
2. Überprüfe, ob TailwindCSS, DaisyUI-Komponenten und Font Awesome Icons korrekt geladen werden.


## Lizenz

Dieses Projekt ist unter der MIT-Lizenz veröffentlicht. Weitere Informationen findest du in der Datei [LICENSE](./LICENSE).

---

*Freue dich darauf, mit EventForge deine eigenen Events zu schmieden!*
