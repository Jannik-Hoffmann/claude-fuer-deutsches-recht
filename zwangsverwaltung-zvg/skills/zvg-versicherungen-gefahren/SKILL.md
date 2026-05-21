---
name: zvg-versicherungen-gefahren
description: "Versicherungen und Gefahren in der Zwangsverwaltung. Prüft Gebäudeversicherung Haftpflicht Beitragsrückstände Schadenmeldung Deckung und Sicherung."
---

# Versicherungen und Gefahren

## Aufgabe

Prüft und sichert den Versicherungsschutz des verwalteten Objekts.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- Versicherungsstatus unklar ist
- Schadensfall, Beitragsrückstand oder Kündigung droht
- Besitzerlangung einen Gefahrenpunkt zeigt

## Eingaben

- Policen, Beitragsrechnungen, Schadenmeldungen
- Objektzustand, Fotos, Dienstleisterberichte
- Konto- und Vorschusslage

## Workflow

1. **Status klären** - Police, Versicherungsnehmer, Objekt, Deckung, Prämien und Rückstände erfassen.
2. **Lücke schließen** - Zahlung, Deckungsbestätigung, Nachversicherung oder Gerichtsinformation vorbereiten.
3. **Schaden** - Schadenanzeige, Belege, Sicherungsmaßnahmen und Anspruchsverfolgung steuern.
4. **Monitoring** - Wiedervorlagen für Prämien und Deckungsänderungen setzen.

## Ausgabe

- Versicherungsregister
- Deckungs- und Schadenvermerk
- Sofortschreiben

## Qualitätsgates

- Deckungsbestätigung belegt
- Rückstände geprüft
- Schaden dokumentiert

## Rote Schwellen

- keine Gebäudeversicherung
- gekündigte Police
- Leitungswasser- oder Brandschaden

## Interne Vorlagen

- assets/templates/versicherung-und-lasten.md
- assets/templates/instandhaltung-gefahrensicherung.md

## Amtliche Erstquellen

- § 3 Abs. 1 Nr. 4 ZwVwV
- § 13 ZwVwV
