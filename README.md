# Aachener Trompetenforum — Website

Statische Website, ready für Cloudflare Pages.

## Dateien

```
atf-website/
├── index.html          ← Startseite
├── news.html           ← Newsseite
├── ensembles.html      ← Ensembles & Buchung
├── kontakt.html        ← Kontaktformular
├── impressum.html      ← Impressum (Daten ergänzen!)
├── datenschutz.html    ← Datenschutz
├── 404.html            ← Fehlerseite
├── _redirects          ← Cloudflare Weiterleitungen
├── styles/
│   └── main.css
├── scripts/
│   └── main.js
└── public/images/
    ├── logo.png
    ├── hero-bg.jpg
    ├── trumpet-bw.jpg
    ├── philharmonie.jpg
    └── piccolos.jpg
```

## Deployment auf Cloudflare Pages

1. **GitHub Repository anlegen** (github.com → New Repository)
2. **Alle Dateien hochladen** (per Git oder direkt im Browser)
3. **Cloudflare Pages** → pages.cloudflare.com → "Create a project"
4. **GitHub verbinden** → Repository auswählen
5. **Build settings:** Framework preset: `None`, Build command: leer lassen, Output: `/`
6. **Deploy!** → Läuft sofort

## Kontaktformular aktivieren

1. Gehe zu **formspree.io** und registriere dich (kostenlos)
2. Neues Formular erstellen → du bekommst eine Form-ID (z.B. `xpzgkldw`)
3. In `kontakt.html` ersetzen:
   ```html
   action="https://formspree.io/f/YOUR_FORM_ID"
   ```
   durch deine echte ID.

## Eigene Domain (RWTH)

Unter Cloudflare Pages → Custom Domains → deine Domain eintragen.
Dann den angezeigten CNAME-Eintrag bei der RWTH beantragen.

## News aktualisieren

Einfach in `news.html` den HTML-Block kopieren und mit neuen Inhalten füllen.

## Impressum

Bitte die `[Platzhalter]` in `impressum.html` mit echten Daten ersetzen!
