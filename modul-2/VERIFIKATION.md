# Modul 2 – Rechtliche Grundlagen: Spielinhalt zur Verifikation

Bitte alle §-Referenzen über NotebookLM prüfen. Unsichere Stellen sind mit ⚠️ markiert.

---

## Spiel 1: Szenario-Quiz (Multiplayer, 8 Fragen)

---

### F1
**Szenario:** Bewerber der Muster GmbH erhalten nur eine Standard-Absage per E-Mail. Kein Hinweis, dass SmartHire die Vorauswahl getroffen hat.

**Frage:** Welche Pflicht wurde verletzt?

- A) Datenminimierung (DSGVO Art. 5 Abs. 1 lit. c)
- B) Informationspflicht bei automatisierten Entscheidungen (DSGVO Art. 13 Abs. 2 lit. f i.V.m. Art. 22)
- C) Risikodokumentation (EU AI Act Art. 9)
- D) Keine – Absagen müssen nicht begründet werden

**Antwort:** B
**Erklärung:** Werden automatisierte Entscheidungen getroffen, müssen Betroffene darüber informiert werden – auch wenn keine Anfrage gestellt wurde.

---

### F2
**Szenario:** SmartHire wurde von einem Drittanbieter entwickelt. Muster GmbH setzt es ein, ohne eigene Risikoprüfung durchzuführen.

**Frage:** Gegen welche Pflicht verstößt Muster GmbH als Betreiber?

- A) DSGVO Art. 28 (kein Auftragsverarbeitungsvertrag)
- B) EU AI Act Art. 26 (Pflichten des Betreibers)
- C) AGG § 12 (Präventionspflicht des Arbeitgebers)
- D) Keine – der Anbieter trägt die Verantwortung

**Antwort:** B
**Erklärung:** Als Betreiber einer Hochrisiko-KI trägt Muster GmbH eigene Pflichten – unabhängig davon, wer das System entwickelt hat.

⚠️ Bitte prüfen: Ist Art. 26 EU AI Act der richtige Artikel für Betreiberpflichten?

---

### F3
**Szenario:** SmartHire analysiert Lebensläufe anhand aller verfügbaren Angaben – inklusive Hobbys, Wohnort und Vereinsmitgliedschaften.

**Frage:** Welcher DSGVO-Grundsatz wird verletzt?

- A) Zweckbindung (Art. 5 Abs. 1 lit. b)
- B) Datenminimierung (Art. 5 Abs. 1 lit. c)
- C) Richtigkeit (Art. 5 Abs. 1 lit. d)
- D) Speicherbegrenzung (Art. 5 Abs. 1 lit. e)

**Antwort:** B
**Erklärung:** Es dürfen nur die Daten verarbeitet werden, die für den konkreten Zweck notwendig sind. Hobbys und Wohnort sind für eine Eignungsbewertung nicht erforderlich.

---

### F4
**Szenario:** Ein abgelehnter Bewerber fragt schriftlich nach dem Grund seiner Ablehnung. Muster GmbH antwortet nicht.

**Frage:** Welches Recht des Bewerbers wurde verletzt?

- A) Recht auf Datenübertragbarkeit (DSGVO Art. 20)
- B) Auskunftsrecht (DSGVO Art. 15) und Recht auf Erläuterung der Entscheidung (DSGVO Art. 22 Abs. 3)
- C) Recht auf Berichtigung (DSGVO Art. 16)
- D) Widerspruchsrecht gegen Profiling (DSGVO Art. 21)

**Antwort:** B
**Erklärung:** Betroffene haben das Recht, eine Erläuterung zu automatisierten Entscheidungen zu erhalten und diese anfechten zu können.

⚠️ Bitte prüfen: Gilt Art. 22 Abs. 3 auch dann, wenn der Bewerber nicht explizit nach der KI fragt?

---

### F5
**Szenario:** Die Trainingsdaten für SmartHire wurden aus öffentlich zugänglichen LinkedIn-Profilen ohne Einwilligung der Betroffenen gesammelt.

**Frage:** Welche Rechtsverstöße liegen vor?

- A) Nur DSGVO Art. 6 (keine Rechtsgrundlage für Verarbeitung)
- B) Nur UrhG § 44b (Grenzen des Text- und Data-Mining)
- C) Beide – DSGVO und UrhG
- D) Keine – öffentlich sichtbare Daten sind frei verwendbar

**Antwort:** C
**Erklärung:** Öffentlich zugängliche Daten sind nicht automatisch frei verarbeitbar. Personenbezogene Daten benötigen eine Rechtsgrundlage (DSGVO), und kommerzielles Scraping ohne Erlaubnis kann gegen das Urheberrecht verstoßen.

§ 44b UrhG gilt auch für kommerzielle Nutzung – sofern der Rechtsinhaber die Nutzung nicht durch maschinenlesbaren Vorbehalt gesperrt hat. Für Forschung gilt speziell § 60d UrhG.

---

### F6
**Szenario:** SmartHire bewertet Bewerber mit Elternzeit-Einträgen im Lebenslauf systematisch schlechter – was faktisch Frauen benachteiligt.

**Frage:** Gegen welches Gesetz verstößt das?

- A) DSGVO Art. 5 (Grundsätze der Datenverarbeitung)
- B) EU AI Act Art. 10 (Anforderungen an Trainingsdaten)
- C) AGG § 3 Abs. 2 (mittelbare Diskriminierung wegen des Geschlechts)
- D) Kein Verstoß – Elternzeit ist ein neutrales Merkmal

**Antwort:** C
**Erklärung:** Mittelbare Diskriminierung liegt vor, wenn ein scheinbar neutrales Kriterium eine Gruppe unverhältnismäßig benachteiligt. Elternzeit wird überwiegend von Frauen genommen.

---

### F7
**Szenario:** Muster GmbH hat keine Datenschutz-Folgenabschätzung (DSFA) für SmartHire durchgeführt, bevor das System in Betrieb genommen wurde.

**Frage:** Wann ist eine DSFA verpflichtend?

- A) Ab 500 verarbeiteten Datensätzen pro Jahr
- B) Bei jeder KI-Nutzung im Unternehmen
- C) Bei Verarbeitungen, die voraussichtlich ein hohes Risiko für Rechte und Freiheiten natürlicher Personen aufweisen (DSGVO Art. 35)
- D) Nur bei der Verarbeitung besonderer Kategorien (DSGVO Art. 9)

**Antwort:** C
**Erklärung:** Automatisierte Entscheidungen in der Personalauswahl gelten als hohes Risiko – eine DSFA ist daher Pflicht, bevor das System eingesetzt wird.

---

### F8
**Szenario:** SmartHire ist als Hochrisiko-KI eingestuft. Welche der folgenden Aussagen über die Konformitätsbewertung ist korrekt?

**Frage:**

- A) Hochrisiko-KI muss immer von einer externen Stelle (Notified Body) zertifiziert werden
- B) Für die meisten Hochrisiko-KI-Systeme nach Anhang III ist eine Selbstbewertung durch den Anbieter möglich
- C) Eine Konformitätsbewertung ist freiwillig und hat keine rechtlichen Folgen
- D) Die Bewertung muss jährlich wiederholt werden

**Antwort:** B
**Erklärung:** Für viele Hochrisiko-KI-Systeme (u.a. in der Personalauswahl) ist eine interne Konformitätsbewertung möglich. Eine externe Stelle ist nur bei bestimmten Systemkategorien vorgeschrieben.

Für Anhang III Nr. 4 (Recruiting/SmartHire) reicht interne Konformitätsbewertung (Anhang VI). Notified Body Pflicht nur bei biometrischen Systemen (Anhang III Nr. 1) ohne harmonisierte Normen – EU AI Act Art. 43 Abs. 1.

---

## Spiel 2: Gesetz-Sortierer (Solo, 6 Szenarien)

Spalten: **DSGVO** | **EU AI Act** | **Urheberrecht** | **AGG**

---

| Nr. | Szenario | Zuordnung | Referenz |
|---|---|---|---|
| 1 | SmartHire informiert Bewerber nicht darüber, dass eine KI über ihre Bewerbung entscheidet. | DSGVO | Art. 13 Abs. 2 lit. f |
| 2 | Das SmartHire-Modell wurde auf Trainingsdaten aus 2010 trainiert – ohne Prüfung auf Aktualität und Repräsentativität. | EU AI Act | Art. 10 (Anforderungen an Trainingsdaten) |
| 3 | SmartHire generiert automatisch Absageschreiben im Stil eines bekannten deutschen Autors. | Urheberrecht | ⚠️ Bitte prüfen: UrhG § 2 / § 23? |
| 4 | SmartHire rankt Bewerberinnen nach Elternzeit-Einträgen systematisch schlechter als Bewerber. | AGG | § 3 Abs. 2 (mittelbare Diskriminierung) |
| 5 | Muster GmbH speichert abgelehnte Bewerbungsunterlagen ohne festgelegte Löschfrist dauerhaft. | DSGVO | Art. 5 Abs. 1 lit. e (Speicherbegrenzung) |
| 6 | SmartHire trägt keine CE-Kennzeichnung, obwohl es als Hochrisiko-KI gilt und in der EU eingesetzt wird. | EU AI Act | Art. 48 (CE-Kennzeichnung) |

---

## Spiel 3: Compliance-Detektiv (Solo, 10 Karten)

Aufgabe: Jede Praxis als **Compliant ✓** oder **Verstoß ✗** einordnen.

---

| Nr. | SmartHire-Praxis | Bewertung | Referenz |
|---|---|---|---|
| 1 | In der Stellenanzeige wird darauf hingewiesen, dass KI bei der Vorauswahl eingesetzt wird. | ✓ | DSGVO Art. 13 Abs. 2 lit. f |
| 2 | Bewerbungsunterlagen werden 10 Jahre ohne Rechtsgrundlage gespeichert. | ✗ | DSGVO Art. 5 Abs. 1 lit. e |
| 3 | Das Modell wurde ausschließlich auf Lebensläufen westeuropäischer Bewerber trainiert – internationale Bewerber werden systematisch schlechter bewertet. | ✗ | AGG § 1 / EU AI Act Art. 10 |
| 4 | Muster GmbH hat mit dem SmartHire-Anbieter einen Auftragsverarbeitungsvertrag abgeschlossen. | ✓ | DSGVO Art. 28 |
| 5 | Jede SmartHire-Empfehlung wird vor der finalen Entscheidung von einer HR-Person geprüft. | ✓ | EU AI Act Art. 14 (menschliche Aufsicht) ⚠️ |
| 6 | Die Risikoklassifizierung von SmartHire wurde nie dokumentiert. | ✗ | EU AI Act Art. 6 Abs. 4 (Dokumentation der Einstufung) |
| 7 | Bewerbungsfotos werden zur Analyse verwendet, ohne dass das in der Datenschutzerklärung erwähnt wird. | ✗ | DSGVO Art. 6 + Art. 13 |
| 8 | Bewerber können jederzeit Auskunft über ihre gespeicherten Daten beantragen und erhalten eine Antwort innerhalb von 30 Tagen. | ✓ | DSGVO Art. 15 i.V.m. Art. 12 Abs. 3 |
| 9 | Muster GmbH hat keine DSFA durchgeführt, obwohl SmartHire systematisch Personen bewertet. | ✗ | DSGVO Art. 35 |
| 10 | SmartHire-generierte Texte werden als eigene Inhalte veröffentlicht, ohne Kennzeichnung als KI-Output. | ✗ | EU AI Act Art. 50 Abs. 4 – Ausnahme: wenn redaktionelle Verantwortung durch Mensch liegt |
