# 🎨 Moderne Portfolio Website

Eine professionelle, moderne und responsive Portfolio-Website mit dunklem Design, Glassmorphism und sanften Animationen.

## ✨ Features

- ✅ **Vollständig Responsive** - Perfekt auf Desktop, Tablet und Smartphone
- ✅ **Modernes Design** - Dunkles Theme mit Glassmorphism und Neon-Elementen
- ✅ **Smooth Animationen** - Sanfte Fade-In und Scroll-Effekte
- ✅ **Interaktiv** - Mobile Navigation, Formular-Handling, Scroll-to-Top
- ✅ **Optimiert** - Schnelle Performance, Clean Code
- ✅ **Accessibility** - Keyboard Navigation, Semantisches HTML
- ✅ **Mobile-First** - Entwickelt für mobile Geräte zuerst

## 🚀 Schnellstart

### 1. Repository klonen oder lokal starten

```bash
# Option 1: Mit Live Server (VSCode Extension)
# 1. Installiere "Live Server" Extension in VSCode
# 2. Klicke auf "Go Live" (unten rechts)
# 3. Website öffnet sich automatisch

# Option 2: Mit Python (Python 3.x)
python -m http.server 8000
# Öffne dann: http://localhost:8000

# Option 3: Mit Node.js (http-server)
npm install -g http-server
http-server
```

### 2. Im Browser öffnen

```
http://localhost:8000
oder
http://localhost:3000
(je nachdem welche Option du verwendest)
```

## 📁 Ordnerstruktur

```
portfolio/
├── index.html          # Hauptseite mit all den Inhalten
├── css/
│   └── styles.css      # Alle Stile und Animationen
├── js/
│   └── script.js       # JavaScript für Interaktivität
└── README.md           # Diese Datei
```

## 📝 Inhalte anpassen

### Deinen Namen eintragen

Öffne `index.html` und suche nach:
```html
<h1 class="hero-title fade-in">Hallo, ich bin <span class="gradient-text">Dein Name</span></h1>
```

Ersetze "Dein Name" mit deinem Namen.

### Hero Section ändern

In der Hero Section (Zeilen ~60-80) kannst du anpassen:
- Hauptüberschrift
- Untertitel ("Web Developer & Designer")
- Beschreibungstext
- Button-Texte

### About Section aktualisieren

Suche nach "Über mich" Section (Zeilen ~85-130) und ändere:
- Professionelle Beschreibung
- Statistiken (50+ Projekte, etc.)

### Skills hinzufügen/ändern

Finde die Skills Section und ändere:
- Skill-Namen
- Icons (nutze Font Awesome Klassen)
- Prozentualzahl in den Progress Bars

```html
<div class="skill-progress">
    <div class="progress-bar" style="width: 95%;"></div>
</div>
```

### Projekte bearbeiten

Suche die Projekte Section und update für jedes Projekt:
- Bild URL (nutze kostenlose Platzhalterbilder)
- Projekttitel
- Beschreibung
- Tags (Technology Stack)
- Demo und GitHub Links

### Kontaktformular

Das Kontaktformular arbeitet momentan lokal. Um es funktionsfähig zu machen, brauchst du:
- Backend API oder
- Service wie Formspree, Netlify Forms, oder SendGrid

### Social Links im Footer

Update die Social Media Links:
```html
<a href="https://github.com/dein-username" class="social-link">
    <i class="fab fa-github"></i>
</a>
```

## 🎨 Design Anpassungen

### Farben ändern

Öffne `css/styles.css` und ändere die CSS-Variablen (Zeilen ~8-20):

```css
:root {
    --bg-primary: #0f0f1e;      /* Haupthintergrund */
    --accent-primary: #00d4ff;  /* Primäre Accent Farbe (Cyan) */
    --accent-secondary: #ff006e; /* Sekundäre Accent Farbe (Pink) */
    --accent-tertiary: #8338ec;  /* Tertiäre Accent Farbe (Purple) */
    /* ... weitere Variablen */
}
```

### Schriftarten ändern

In `index.html` findest du den Font Import (Zeile ~6):
```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Poppins:wght@600;700;800&display=swap" rel="stylesheet">
```

Du kannst andere Google Fonts nutzen von: https://fonts.google.com/

### Animationen anpassen

In `css/styles.css` kannst du die Animation-Verzögerungen ändern:
- `animation-delay: 0.1s;` - Zeit bis Animation startet
- `animation: fadeInUp 0.8s;` - Dauer der Animation

## 🖼️ Kostenlose Platzhalterbilder

Die Website nutzt bereits Platzhalterbilder von Unsplash. Du kannst deine eigenen Bilder verwenden:

1. **Unsplash** - https://unsplash.com (kostenlos)
2. **Pexels** - https://www.pexels.com (kostenlos)
3. **Pixabay** - https://pixabay.com (kostenlos)

URL Format: `https://images.unsplash.com/photo-[ID]?w=400&h=300&fit=crop`

## 📱 Browser Support

- ✅ Chrome (neueste)
- ✅ Firefox (neueste)
- ✅ Safari (neueste)
- ✅ Edge (neueste)
- ✅ Mobile Browser (iOS Safari, Chrome Mobile)

## ⚡ Performance Tipps

1. **Bilder optimieren** - Nutze Bildkompression Tools
2. **Lazy Loading** - Für viele Bilder
3. **Caching** - Browser Caching aktivieren
4. **CDN** - Font Awesome und Google Fonts nutzen bereits CDN

## 🔧 Weitere Verbesserungen

### Contact Form funktionstüchtig machen

Option 1: Mit Netlify Forms
```html
<form name="contact" method="POST" netlify>
    <input type="text" name="name" placeholder="Dein Name" required>
    <input type="email" name="email" placeholder="Deine E-Mail" required>
    <textarea name="message" placeholder="Deine Nachricht" required></textarea>
    <button type="submit">Senden</button>
</form>
```

Option 2: Mit Formspree (https://formspree.io/)
```html
<form action="https://formspree.io/f/YOUR-ID" method="POST">
    <!-- Form Felder -->
</form>
```

### SEO Optimierung

Füge Meta Tags hinzu:
```html
<meta name="description" content="Portfolio Website von [Dein Name]">
<meta name="keywords" content="portfolio, web developer, designer">
<meta property="og:title" content="Mein Portfolio">
<meta property="og:description" content="Willkommen auf meiner Portfolio-Website">
<meta property="og:image" content="url-zu-preview-bild">
```

### Google Analytics

Füge Google Analytics hinzu (optional):
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_ID');
</script>
```

## 📚 Nützliche Ressourcen

- **Font Awesome Icons** - https://fontawesome.com
- **Google Fonts** - https://fonts.google.com
- **CSS Tricks** - https://css-tricks.com
- **MDN Web Docs** - https://developer.mozilla.org
- **Can I Use** - https://caniuse.com (Browser Kompatibilität)

## 🐛 Häufige Probleme

### Website sieht merkwürdig aus
- Cache löschen: `Ctrl+Shift+Delete` (oder `Cmd+Shift+Delete` auf Mac)
- Hard Refresh: `Ctrl+F5` (oder `Cmd+Shift+R` auf Mac)

### Bilder laden nicht
- Prüfe die Image URLs
- Stelle sicher, dass die Bilder öffentlich zugänglich sind
- Nutze HTTPS URLs

### Form funktioniert nicht
- Das lokale Formular zeigt nur eine Success-Nachricht
- Um echte E-Mails zu erhalten, nutze Netlify Forms oder Formspree

### Navigation funktioniert nicht auf Handy
- Prüfe ob JavaScript aktiviert ist
- Versuche die Seite zu aktualisieren
- Teste in verschiedenen Browsern

## 📧 Kontakt & Support

Hast du Fragen? Erstelle ein Issue auf GitHub oder kontaktiere mich!

## 📄 Lizenz

Diese Website ist kostenlos und kann frei verwendet werden. Du kannst sie verwenden, modifizieren und anpassen wie du möchtest.

---

**Viel Spaß mit deiner neuen Portfolio-Website! 🚀**

Made with ❤️ und modernem Code.
