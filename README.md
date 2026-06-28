# MAR STINKT 🦨 — Amtliches Gestank-Portal der Stadt Ravensburg

Ein aufwändig gestaltetes Portal, das auftritt wie ein offizielles Behörden-Angebot
der Stadt Ravensburg — und amtlich bestätigt: **Mar stinkt.**

## Features

- 🏛️ **Behörden-Optik** — echtes Ravensburg-Stadtwappen, Aktenzeichen und Amtssiegel
- 📈 **Animiertes Stink-O-Meter™** — Messnadel, die den „Gestankspegel" live auf 9,7 GES hochzählt
- 🧪 **Geruchs-Steckbrief & Vergleich** — Datenblatt + animierte Vergleichsbalken (Mar vs. Mülltonne, Fischmarkt …)
- 🗺️ **Sperrzonen-Karte** — schematischer Lageplan mit Evakuierungs-Radius rund um Mar
- 🕒 **Chronik des Gestanks** — Zeitstrahl der „dokumentierten Vorfälle"
- 📜 **Amtliches Gestank-Zertifikat** — seriöse Urkunde mit Zierrahmen, Siegel und Unterschriften
- 🖨️ **Druck-/PDF-Funktion** — das Zertifikat passt im Druck **genau auf eine A4-Seite**
- ✍️ **Petition mit Live-Zähler** — Unterschriften werden im Browser (localStorage) gezählt
- 📰 **Schlagzeilen-Ticker & Pressestimmen** — durchlaufende Fake-Meldungen
- 💬 **Scrollende Geruchszeugnisse** — absurde „verifizierte" Bewertungen mit Sternen
- ❓ **Amtliche FAQ** — Akkordeon mit seriös klingenden Antworten
- 📱 **Voll mobil-tauglich** — Mobile-First, läuft einwandfrei auf dem Smartphone

## Benutzung

Keine Installation, keine Build-Tools.

```
index.html im Browser öffnen (Doppelklick reicht)
```

Zertifikat ausdrucken / als PDF speichern: Button **„Zertifikat drucken / als PDF
speichern"** klicken → im Druckdialog „Als PDF speichern" wählen. Im Druck erscheint
nur das Zertifikat, seitenfüllend auf einer A4-Seite.

## Dateien

- `index.html` — komplette Seite (HTML + CSS + Vanilla-JS inline)
- `Wappen_Ravensburg.svg.png` — das Stadtwappen; wird von `index.html` direkt
  referenziert und muss daher **im selben Ordner** neben `index.html` liegen

## Technik

- HTML + CSS + Vanilla-JS, keine externen Skripte/Frameworks
- Animationen über `IntersectionObserver` (Reveal, Zähler, Stink-O-Meter, Balken)
- Petitions-Zähler persistiert in `localStorage`
- Amtssiegel als Inline-SVG; Stadtwappen als referenziertes PNG
- Schriften von Google Fonts mit System-Font-Fallback (funktioniert auch offline)
