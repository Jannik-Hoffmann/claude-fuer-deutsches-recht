---
name: zvg-oeffentliche-lasten
description: "Öffentliche Lasten und grundstuecksbezogene Abgaben in der Zwangsverwaltung. Erfasst Grundsteuer Gebuehren Beitraege Rang Fälligkeit und Zahlung."
---

# Öffentliche Lasten und grundstücksbezogene Abgaben

## Aufgabe

Ordnet Grundsteuer, Gebühren, Beiträge und sonstige objektbezogene Lasten in der Zwangsverwaltung.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- Grundsteuer, Gebühren oder Beitragsbescheide eingehen
- Lasten im Besitzerlangungsbericht fehlen
- Verteilung oder Rechnungslegung vorbereitet wird

## Eingaben

- Bescheide, Lastenregister, Kontoauszüge
- Objektdaten, Grundsteuer, Gebühren, WEG-Unterlagen
- Fälligkeiten und Zahlungsnachweise

## Workflow

1. **Lasten erfassen** - Art, Zeitraum, Betrag, Fälligkeit und Behörde aufnehmen.
2. **Rang und Zweck** - öffentliche Last, Betriebskosten, Verwaltungsausgabe oder Schuldneraltlast trennen.
3. **Zahlungsplan** - Liquidität, Vorschussbedarf und Verteilungsauswirkung prüfen.
4. **Nachhalten** - Bescheide, Widerspruchsfristen und Belege ablegen.

## Ausgabe

- Lastenregister
- Zahlungsplan
- Berichtsbaustein

## Qualitätsgates

- Zeitraum sauber abgegrenzt
- Fälligkeit belegt
- Zahlung buchhalterisch zugeordnet

## Rote Schwellen

- Zwangsmaßnahmen der Kommune
- Doppelzahlung
- Beitragsbescheid mit kurzer Frist

## Interne Vorlagen

- assets/templates/versicherung-und-lasten.md
- assets/templates/konto-kassenbuch.md

## Amtliche Erstquellen

- § 3 Abs. 1 Nr. 5 ZwVwV
- § 15 ZwVwV
