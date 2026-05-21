---
name: zvg-miet-und-pachtverwaltung
description: "Miet und Pachtverwaltung in der Zwangsverwaltung. Prüft Mietvertraege Pachtvertraege Zahlstellen Vorausverfuegungen Kautionen Nebenkosten und Nutzung."
---

# Miet- und Pachtverwaltung

## Aufgabe

Ordnet Miet- und Pachtverhältnisse im beschlagnahmten Objekt mit Kommunikation, Zahlstellen, Kautionen und Vertragsrisiken.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- Mieter oder Pächter vorhanden sind
- Mietzahlungen umzuleiten sind
- Verträge, Kautionen oder Vorausverfügungen unklar sind

## Eingaben

- Miet- und Pachtverträge
- Mieterliste, Zahlungsverlauf, Kautionen
- Schreiben des Schuldners oder der Mieter

## Workflow

1. **Verträge erfassen** - Einheit, Nutzer, Miete, Nebenkosten, Laufzeit, Kaution und Sonderrechte aufnehmen.
2. **Mitteilung** - Mieter/Pächter über Zwangsverwaltung und neue Zahlstelle informieren.
3. **Vorausverfügungen** - Abtretung, Vorauszahlung, Kaution und Rückstände prüfen.
4. **Laufend verwalten** - Anpassungen, Nebenkosten, Mängel, Kündigungen und Kommunikation steuern.

## Ausgabe

- Rent Roll
- Mieterschreiben
- Vertragsrisikomatrix

## Qualitätsgates

- Soll- und Istmiete getrennt
- Kautionen nicht als freie Masse behandelt
- Vorausverfügungen geprüft

## Rote Schwellen

- Zahlung an Schuldner
- fehlender Mietvertrag
- streitiger Besitz

## Interne Vorlagen

- assets/templates/mieterliste-rent-roll.md
- assets/templates/schuldner-glaeubiger-kommunikation.md

## Amtliche Erstquellen

- §§ 4, 5, 6 ZwVwV
- § 152 ZVG
