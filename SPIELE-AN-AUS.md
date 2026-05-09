# Spiele – Module ein- und ausschalten

## Wo?

Datei: `spiele/index.html`
Öffnen in VS Code, dann ganz nach unten zum `<script>`-Block scrollen.
Die Schalter stehen ganz oben im Script, deutlich markiert.

---

## Gesamte Plattform sperren / freischalten

```javascript
const GAMES_ENABLED = true;   // ← true = offen, false = gesperrt
```

Wenn `false`: Teilnehmer sehen nach der Passworteingabe die Meldung
„Die Spiele sind momentan nicht verfügbar."

---

## Einzelne Module ein- / ausschalten

```javascript
const MODULE_STATUS = {
    'modul-1-quiz':      true,   // Szenario-Quiz (Multiplayer)
    'modul-1-baukasten': true,   // Prompt-Baukasten (Solo)
    'modul-1-sortierer': true,   // Methoden-Sortierer (Solo)
    'modul-2': false,            // Rechtliche Grundlagen
    'modul-3': false,            // Risikomanagement & Datenschutz
    'modul-4': false,            // PM & Qualitätssicherung
    'modul-5': false,            // Daten & Change Management
    'modul-6': false,            // ISO 42001
    'modul-7': false,            // EU AI Act
};
```

- `true` → Karte ist anklickbar (grüner Rahmen, „▶ Spielen")
- `false` → Karte bleibt gesperrt (🔒 Demnächst), auch wenn die Datei schon existiert

---

## Nach jeder Änderung: deployen

```bash
cd /home/imader/Dokumente/KI-Beauftragter && git add spiele/index.html && git commit -m "Spiele: Modul X freigeschaltet" && git subtree push --prefix spiele https://HappyJeanny:TOKEN@github.com/HappyJeanny/ki-spiele.git main
```

`TOKEN` = Personal Access Token von github.com → Settings → Developer settings → Tokens (classic)

GitHub Pages aktualisiert sich danach automatisch innerhalb von 1–2 Minuten.

---

## Neues Modul hinzufügen

1. Spiel-Dateien unter `spiele/modul-X/` anlegen
2. Neue Karte in `spiele/index.html` im `.games-grid` einfügen (mit `data-module="modul-X"`)
3. Eintrag `'modul-X': false` in `MODULE_STATUS` ergänzen
4. Wenn fertig: auf `true` setzen und deployen
