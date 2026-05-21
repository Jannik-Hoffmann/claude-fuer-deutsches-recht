---
name: zvg-verteilungsplan-155
description: "Verteilungsplan nach § 155 ZVG. Ordnet Nutzungen Ausgaben Kosten Gläubigerzahlungen Vorschuesse Rang und Auszahlung in der Zwangsverwaltung."
---

# Verteilungsplan § 155 ZVG

## Aufgabe

Bereitet die Verteilung der Nutzungen und Erlöse unter Berücksichtigung von Ausgaben, Kosten und Rang vor.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- auskehrbare Überschüsse vorhanden sind
- Gläubiger Zahlung verlangen
- Schlussrechnung oder laufende Auszahlungen anstehen

## Eingaben

- Kontostand, Einnahmen, Ausgaben, Kosten
- Gläubigerforderungen, Rang, Gerichtskosten
- Rücklagen und absehbare Objektkosten

## Workflow

1. **Verteilungsmasse** - verfügbare Nutzungen nach Abzug laufender Ausgaben und Rücklagen bestimmen.
2. **Rang prüfen** - Gläubiger, Gerichtskosten, Verwaltervergütung und öffentliche Lasten einordnen.
3. **Plan erstellen** - Auszahlungsbeträge, Rückbehalte und Begründung darstellen.
4. **Freigabe** - Gericht oder Beteiligte informieren und Zahlung dokumentieren.

## Ausgabe

- Verteilungsplan
- Auszahlungsliste
- Berichtsbaustein

## Qualitätsgates

- keine Verteilung ohne Rücklagencheck
- Rang und Kosten geprüft
- Zahlungen belegt

## Rote Schwellen

- Auskehr trotz offener Notkosten
- falscher Gläubiger
- ungeklärte öffentliche Last

## Interne Vorlagen

- assets/templates/verteilungsplan-155.md
- assets/templates/rechnungslegung.md

## Amtliche Erstquellen

- § 155 ZVG
- §§ 11, 12 ZwVwV
