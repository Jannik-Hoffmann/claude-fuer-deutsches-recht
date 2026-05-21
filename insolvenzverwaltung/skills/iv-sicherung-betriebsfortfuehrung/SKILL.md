---
name: iv-sicherung-betriebsfortfuehrung
description: "Betriebsfortfuehrung in der Insolvenzverwaltung. Führt Cash Bridge Lieferanten Arbeitnehmer Insolvenzgeld Kundenauftraege Produktion und Fortfuehrungsrisiken."
---

# Sicherung und Betriebsfortführung

## Aufgabe

Prüft und steuert, ob und wie der Geschäftsbetrieb im Eröffnungsverfahren oder eröffneten Verfahren fortgeführt werden kann.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- Betrieb, Filiale, Praxis oder Werk noch aktiv ist
- Löhne, Lieferanten und Kundenaufträge offen sind
- Massemehrung durch Fortführung möglich erscheint

## Eingaben

- Auftragsbestand, Deckungsbeiträge, Liquiditätsplan
- Lohnliste, Insolvenzgeldzeitraum, Lieferantenkritikalität
- Versicherungen, Genehmigungen, Schlüsselressourcen

## Workflow

1. **Fortführungsziel** - Massemehrung, Sanierung, Verkauf oder geordnete Ausproduktion definieren.
2. **Cash-Bridge** - Einzahlungen, Auszahlungen, Insolvenzgeld, kritische Lieferanten und Steuern planen.
3. **Operative Risiken** - Versicherung, Arbeitsschutz, Umwelt, IT, Schlüsselpersonen und Genehmigungen prüfen.
4. **Entscheidungsvorlage** - Fortführung, Stilllegung oder Hybrid mit Ampel und Bedingungen ausgeben.

## Ausgabe

- Fortführungswochenplan
- Lieferanten- und Kundenampel
- Entscheidungsvorlage für Gericht oder Ausschuss

## Qualitätsgates

- kein Fortführungsbeschluss ohne Cash-Bridge
- kritische Genehmigungen geprüft
- Masseinteresse dokumentiert

## Rote Schwellen

- negative Fortführungsdeckung
- ungeklärte Versicherung
- Lohn- oder Sozialabgabenrisiko

## Interne Vorlagen

- assets/templates/betriebsfortfuehrung-wochenplan.md
- assets/templates/liquiditaetsstatus-kurzcheck.md

## Amtliche Erstquellen

- §§ 21, 22, 55 InsO
- SGB III Insolvenzgeld als zu prüfende Schnittstelle
