---
name: zvg-betriebskosten-hausgeld
description: "Betriebskosten Hausgeld und laufende Objektkosten. Prüft Nebenkosten Dienstleister WEG Hausgeld Versorger Wirtschaftlichkeit Abrechnung und Zahlungsplan."
---

# Betriebskosten, Hausgeld und laufende Objektkosten

## Aufgabe

Verhindert, dass laufende Objektkosten, Hausgeld und Versorgerleistungen die Verwaltung destabilisieren.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- WEG-Hausgeld, Betriebskosten oder Versorgerrechnungen eingehen
- Abrechnungen erstellt oder geprüft werden müssen
- Liquiditätsengpass bei laufender Verwaltung entsteht

## Eingaben

- Hausgeldabrechnung, Wirtschaftsplan, Versorgerverträge
- Betriebskostenbelege, Dienstleisterrechnungen
- Mieter-Vorauszahlungen und Leerstände

## Workflow

1. **Kosten erfassen** - laufende Kosten, öffentliche Lasten, Hausgeld, Dienstleister und Versorger trennen.
2. **Umlage prüfen** - umlagefähige und nicht umlagefähige Positionen markieren.
3. **Liquidität** - Fälligkeiten mit Mieten und Vorschussbedarf abgleichen.
4. **Abrechnung** - Betriebskosten- oder WEG-Schnittstellen für Bericht vorbereiten.

## Ausgabe

- Kostenmatrix
- Zahlungsplan
- Abrechnungsvorbereitung

## Qualitätsgates

- öffentliche Lasten separat
- Umlagefähigkeit geprüft
- Fälligkeit belegt

## Rote Schwellen

- Versorgungssperre
- Hausgeldrückstand mit Verwalterdruck
- unwirtschaftlicher Dienstleister

## Interne Vorlagen

- assets/templates/betriebskosten-hausgeld.md
- assets/templates/konto-kassenbuch.md

## Amtliche Erstquellen

- §§ 9, 13, 15 ZwVwV
- § 155 ZVG
