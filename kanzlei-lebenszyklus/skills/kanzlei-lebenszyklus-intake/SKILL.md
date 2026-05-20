---
name: kanzlei-lebenszyklus-intake
description: "Strukturiert jeden Kanzlei-Eingang aus Brief Fax beA E-Mail SMS iMessage WhatsApp Telegram Teams Screenshot Upload oder Telefonnotiz. Erkennt Absender Akte Aktenzeichen Fristen Action-Items Datenschutzrisiken und nächsten Schritt. Fragt bei Unsicherheit gezielt nach."
---

# Intake und Eingangstriage

## Zweck

Dieser Skill nimmt beliebige Eingänge entgegen und macht daraus eine geordnete Kanzlei-Entscheidung: zuordnen, neu anlegen, beantworten, fristen, delegieren oder zurückfragen.

## Unterstützte Eingangskanäle

- Brief, Scan, Foto, Fax.
- beA-Nachricht, EGVP-Ausdruck, Empfangsbekenntnis.
- E-Mail und Anhänge.
- SMS, iMessage, WhatsApp, Telegram, Teams.
- Screenshot, Audio-Notiz, Telefonnotiz.
- Ordnerdrop oder Datenraum-Upload.

## Ablauf

1. **Kanal bestimmen**: Quelle, Empfangsdatum, technische Metadaten, Zuverlässigkeit.
2. **Absender und Beteiligte extrahieren**: Mandant, Gegner, Gericht, Behörde, Versicherung, Dritte.
3. **Aktenbezug prüfen**: eigenes Aktenzeichen, fremdes Aktenzeichen, Name, Sache, Gericht.
4. **Fristen und Action-Items erkennen**: Rechtsbehelfsfrist, gerichtliche Verfügung, Antwortfrist, Wiedervorlage, Rückruf.
5. **Mandatsannahme/GwG-Indikatoren erkennen**: neue Anfrage, Unternehmensmandant, Immobilien, Gesellschaft, Transaktion, Ausweiskopie, Handelsregisterauszug, wirtschaftlich Berechtigte, PEP, Fremdgeld, Drittzahlung, abweichender Zahler.
6. **Datenschutz und Geheimnis prüfen**: Drittinhalte, Gesundheitsdaten, Bankdaten, Ausweiskopien, Kinder, Strafdaten, besondere Kategorien.
7. **Priorität setzen**: sofort, heute, diese Woche, warten, nur ablegen.
8. **Ausgabe erzeugen**: Intake-Karte plus vorgeschlagene Ablage.

## Kanalregeln

### Messenger und Screenshots

- Authentizität nicht unterstellen.
- Kontext erfassen: wer schreibt, wann, in welchem Thread.
- Keine privaten Drittinhalte unnötig übernehmen.
- Bei Screenshots immer prüfen, ob abgeschnittene Inhalte entscheidend sein könnten.

### beA

- Empfangstag und eventuelle Zustellung sauber dokumentieren.
- Empfangsbekenntnis nie ohne Freigabe abgeben.
- Keine beA-PIN, Zertifikate oder Token speichern.
- Bei beA-Connect immer `kanzlei-lebenszyklus-bea-journal` verwenden: Nachrichtenjournal einsehen, Screenshot sichern, jede eingegangene Nachricht als ZIP exportieren oder herunterladen, ZIP entpacken und der Akte zuordnen.
- Wenn ein elektronisches Empfangsbekenntnis verlangt wird, EB-Workflow anbieten und vor Abgabe ausdrücklich warnen.

### Fax und Brief

- Eingangsstempel und Lesbarkeit prüfen.
- Bei Fristbezug Originaleingang und Scanzeit trennen.

## Ausgabeformat

```markdown
## Intake-Karte

- Kanal:
- Eingang am:
- Absender:
- Betroffene Akte:
- Externe Aktenzeichen:
- Kurzinhalt:
- Fristen:
- Action-Items:
- Risiken:
- Mandatsannahme/GwG:
- Vorschlag:
- Rückfragen:
```

## Übergabe

- Neue Sache: `kanzlei-lebenszyklus-akte` und bei Annahme-/Identifizierungs-/GwG-Indikatoren `kanzlei-lebenszyklus-mandatsannahme-gwg`.
- Unklare Aktenzeichen: `kanzlei-lebenszyklus-aktenzeichen`.
- Frist oder Handlung: `kanzlei-lebenszyklus-fristen-monitor`.
- Antwortentwurf oder Versand: `kanzlei-lebenszyklus-output-versand`.
- beA-Journal, beA-ZIP oder elektronisches Empfangsbekenntnis: `kanzlei-lebenszyklus-bea-journal`.
