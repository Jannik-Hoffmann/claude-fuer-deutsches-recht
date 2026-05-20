---
name: kanzlei-lebenszyklus-ustva-simulation
description: "Bietet Fallbacks wenn UStVA oder ELSTER nicht funktionieren. Führt durch ELSTER-Simulation manuelle Eingabe XML-Upload-Prüfung Fachsoftware-Export Steuerberater-Paket Fehlerdiagnose und Übertragungsprotokoll ohne echte Abgabe."
---

# UStVA- und ELSTER-Simulation

## Zweck

Dieser Skill greift, wenn die Umsatzsteuer-Voranmeldung vorbereitet ist, aber ELSTER, Buchhaltung, XML-Upload oder Fachsoftware nicht angeschlossen ist oder scheitert. Er bietet einen realistischen Übungslauf und sichere Fallbacks, ohne eine echte steuerliche Übermittlung zu behaupten.

## Grundsatz

ELSTER ist kein Ablageort für beliebige Dokumente. Eine UStVA wird in Mein ELSTER im Formular erfasst oder über geeignete Software beziehungsweise passende XML-Daten übertragen. Ein PDF, eine Markdown-Datei oder ein gewöhnliches Tabellenblatt ist kein UStVA-Upload. Wenn XML genutzt wird, muss die Datei zum ELSTER/ERiC-Datensatz passen und technisch geprüft sein.

## Startfrage

> UStVA ist vorbereitet, aber ELSTER oder die Fachsoftware ist nicht angeschlossen. Soll ich den Ablauf simulieren, eine manuelle ELSTER-Eingabeliste erzeugen, ein Steuerberater-Paket bauen oder eine XML-Upload-Prüfung vorbereiten?

## Modi

### Modus A: ELSTER-Online-Simulation

- Formularauswahl simulieren.
- Zeitraum, Steuernummer, Besteuerungsart und Dauerfristverlängerung abfragen.
- Kennzahlen mit Beträgen aus dem Vorbereitungsblatt befüllen.
- Plausibilitätsfehler simulieren.
- Abgabe-Haltepunkt setzen.
- Simuliertes Übertragungsprotokoll nur als Übung markieren.

### Modus B: Manuelle ELSTER-Eingabeliste

- Feld-für-Feld-Eingabebogen erzeugen.
- Beträge, Quellen und Unsicherheiten daneben ausweisen.
- Keine Abgabe behaupten.
- Nach echter Übermittlung Übertragungsprotokoll anfordern.

### Modus C: XML-Upload-Prüfung

- Klären, ob eine Fachsoftware oder ein validierter Export vorhanden ist.
- Keine freie XML-Datei erfinden.
- Wenn ein XML vorliegt: Schema, Datenart, Zeitraum, Steuernummer, Summen und Plausibilität prüfen oder `Validierung offen` markieren.
- Upload nur als Nutzerhandlung oder Fachsoftwareprozess beschreiben.

### Modus D: Steuerberater- oder Buchhaltungspaket

- Summenblatt, Eingangsrechnungen, Ausgangsrechnungen, offene Reverse-Charge-Fragen und Belegliste bündeln.
- Rückfrage an Steuerberater formulieren.
- Keine elektronische Abgabe behaupten.

### Modus E: Fehlerdiagnose

Typische Probleme strukturiert abfragen:

- ELSTER-Zertifikat fehlt oder abgelaufen.
- Falsche Steuernummer oder falscher Mandant.
- Formular nicht gefunden.
- Zeitraum falsch.
- Dauerfristverlängerung unklar.
- XML wird abgelehnt.
- Plausibilitätsfehler.
- Übertragungsprotokoll fehlt.

## Stoppschilder

Immer anhalten bei:

- echter Abgabe,
- Korrekturmeldung,
- Dauerfristverlängerung,
- Sondervorauszahlung,
- Reverse Charge,
- Auslandssachverhalten,
- unklarer Vorsteuer,
- fehlender Steuernummer,
- fehlendem Übertragungsprotokoll.

## Ausgabe

- `assets/templates/ustva-elster-simulation.md`.
- `assets/templates/ustva-elster-eingabebogen.md`.
- `assets/templates/ustva-xml-upload-pruefung.md`.
- `assets/templates/ustva-steuerberater-paket.md`.
