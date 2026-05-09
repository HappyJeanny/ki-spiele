# Spiele – Änderungen deployen

## Voraussetzungen

- Änderungen sind in VS Code gespeichert
- Du bist im Haupt-Repo `KI-Beauftragter` eingeloggt
- Personal Access Token bereit (siehe unten)

---

## Befehl (alles in einer Zeile)

```bash
cd /home/imader/Dokumente/KI-Beauftragter && git add spiele/ && git commit -m "Spiele: kurze Beschreibung der Änderung" && git subtree push --prefix spiele https://HappyJeanny:TOKEN@github.com/HappyJeanny/ki-spiele.git main
```

`TOKEN` ersetzen durch deinen Personal Access Token.

Nach ca. 1–2 Minuten ist die Änderung live unter `https://spiele.ki-strategie.co`.

---

## Personal Access Token erstellen (einmalig oder bei Ablauf)

1. github.com → oben rechts: Profilbild → **Settings**
2. Links unten: **Developer settings**
3. **Personal access tokens** → **Tokens (classic)**
4. **Generate new token (classic)**
   - Note: `ki-spiele deploy`
   - Expiration: 90 days
   - Scope: **repo** ankreuzen
5. **Generate token** → Token kopieren (`ghp_...`)

---

## Was kann ich alles ändern?

| Was | Datei |
|---|---|
| Fragen im Quiz | `spiele/modul-1/index.html` → `const QUESTIONS = [...]` |
| RAKF-Übungen im Baukasten | `spiele/modul-1/baukasten.html` → `const EXERCISES = [...]` |
| Szenarien im Sortierer | `spiele/modul-1/sortierer.html` → `const SZENARIEN = [...]` |
| Module sperren / freischalten | `spiele/index.html` → `MODULE_STATUS` (siehe SPIELE-AN-AUS.md) |
| Zugangscode ändern | `spiele/index.html` → `const HUB_PASSWORD = "..."` |
| Neues Modul hinzufügen | siehe SPIELE-AN-AUS.md |

---

## Troubleshooting

**„Datei oder Verzeichnis nicht gefunden"**
→ Prüfen ob du im richtigen Ordner bist: Befehl beginnt mit `cd /home/imader/Dokumente/KI-Beauftragter`

**Authentifizierungsfehler**
→ Token abgelaufen oder falsch eingegeben → neuen Token erstellen (siehe oben)

**Änderung nicht sichtbar nach 5 Minuten**
→ Browser-Cache leeren (Strg + Shift + R)
