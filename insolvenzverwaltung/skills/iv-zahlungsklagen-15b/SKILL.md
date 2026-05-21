---
name: iv-zahlungsklagen-15b
description: "Zahlungsklagen nach § 15b InsO. Rekonstruiert Insolvenzreife Zahlungen Organstellung Ausnahmen Schaden Verjährung D und O und Klageantrag."
---

# Zahlungsklagen nach § 15b InsO

## Aufgabe

Bereitet Ansprüche gegen Geschäftsleiter wegen Zahlungen nach Insolvenzreife aus Sicht der Insolvenzmasse vor.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- Zahlungsunfähigkeit oder Überschuldung vor Antrag plausibel ist
- Zahlungen nach Eintritt der Insolvenzreife rekonstruiert werden
- D&O-Deckung oder Vergleich geprüft wird

## Eingaben

- Liquiditätsstatus, BWA, OPOS, Bankjournale
- Organstellung, Geschäftsverteilung, Beschlüsse
- Zahlungslisten, Steuer- und SV-Zahlungen, Fortführungsmaßnahmen

## Workflow

1. **Insolvenzreife datieren** - § 17 und § 19 InsO getrennt, stichtagsbezogen und belegbasiert prüfen.
2. **Zahlungen filtern** - Zahlungen nach Stichtag mit Empfänger, Zweck, Konto und Beleg erfassen.
3. **Ausnahmen prüfen** - ordnungsgemäßer Geschäftsgang, Antragstellung, Steuerprivileg und Masseinteresse prüfen.
4. **Klage bauen** - Anspruch, Schaden, Verjährung, D&O und Beweisangebot strukturieren.

## Ausgabe

- § 15b-Zahlungsmatrix
- Anspruchs- und Verteidigungsmatrix
- Klageentwurf oder Vergleichsvermerk

## Qualitätsgates

- Insolvenzreife nicht geschätzt, sondern begründet
- Zahlungslisten bankseitig belegbar
- Ausnahmen transparent geprüft

## Rote Schwellen

- unvollständige Bankdaten
- unklare Organstellung
- Verjährungsdruck

## Interne Vorlagen

- assets/templates/zahlungsklage-15b.md
- assets/templates/liquiditaetsstatus-kurzcheck.md

## Amtliche Erstquellen

- § 15b InsO
- §§ 17, 19 InsO
