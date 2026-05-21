---
name: zvg-kommandocenter
description: "ZVG Zwangsverwaltungs-Kommandocenter. Triage Bestellung Beschlagnahme Besitz Mieter Konto Bericht Rechnungslegung Verteilung und Risiken freistehend."
---

# Zwangsverwaltungs-Kommandocenter

## Aufgabe

Führt Zwangsverwalterinnen und Zwangsverwalter vom Bestellungsbeschluss bis zur laufenden Verwaltung und Verteilung.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- ein Zwangsverwaltungsbeschluss eingeht
- Objekt, Mieter, Schuldner oder Gläubiger geordnet werden müssen
- unklar ist, welche Sofortmaßnahmen anstehen

## Eingaben

- Anordnungs- und Bestellungsbeschluss
- Grundstücksdaten, Gläubiger, Schuldner, Mieter
- Mietlisten, Lasten, Versicherungen, Kontoangaben

## Workflow

1. **Beschluss lesen** - Objekt, Schuldner, Gläubiger, Rang und Umfang der Beschlagnahme erfassen.
2. **Sofortplan** - Besitz, Mieterinformation, Konto, Versicherung und Lasten priorisieren.
3. **Objektcockpit** - Rent Roll, Rückstände, Ausgaben, Risiken und Gerichtswiedervorlagen anlegen.
4. **Nächste Aktion** - konkrete Schreiben, Vor-Ort-Termin oder Gerichtsanzeige ausgeben.

## Ausgabe

- Objektkarte
- Sofortmaßnahmenliste
- Kommunikationspaket

## Qualitätsgates

- Bestellung und Objekt exakt erfasst
- keine Zahlung auf Privatkonto
- Mieter und Pächter werden korrekt informiert

## Rote Schwellen

- fehlende Versicherung
- akute Gefahr am Objekt
- Mietzahlungen an Schuldner nach Beschlagnahme

## Interne Vorlagen

- assets/templates/zvg-objektkarte.md
- assets/templates/quality-gate.md

## Amtliche Erstquellen

- §§ 150, 152 ZVG
- §§ 1, 3 ZwVwV
