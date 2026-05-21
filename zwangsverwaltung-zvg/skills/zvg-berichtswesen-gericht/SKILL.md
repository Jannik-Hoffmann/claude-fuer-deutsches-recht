---
name: zvg-berichtswesen-gericht
description: "Berichtswesen an das Vollstreckungsgericht in der Zwangsverwaltung. Erstellt Besitzerlangungsbericht Sachstandsbericht Monatsbericht und Entscheidungsvorlage."
---

# Berichtswesen an das Vollstreckungsgericht

## Aufgabe

Erstellt klare, vollständige und belegbare Berichte an das Vollstreckungsgericht.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- Besitzerlangungsbericht fällig ist
- Gericht Sachstand oder Entscheidungsvorlage verlangt
- wesentliche Ereignisse im Objekt auftreten

## Eingaben

- Objektkarte, Besitzprotokoll, Rent Roll
- Kontostand, Rückstände, Maßnahmen, Risiken
- gerichtliche Verfügung

## Workflow

1. **Adressat und Anlass** - Berichtstyp, Zeitraum und konkrete gerichtliche Frage bestimmen.
2. **Faktenblock** - Objekt, Nutzung, Mieten, Lasten, Maßnahmen, Konto und Risiken aktualisieren.
3. **Entscheidungsbedarf** - Zustimmung, Vorschuss, Maßnahme oder Verteilung klar herausstellen.
4. **Anlagen** - Fotos, Konto, Belege und Tabellen referenzieren.

## Ausgabe

- Besitzerlangungsbericht
- Sachstandsbericht
- Gerichtliche Entscheidungsvorlage

## Qualitätsgates

- § 3 ZwVwV-Bericht vollständig
- Zahlen mit Anlagen
- offene Ermittlungen benannt

## Rote Schwellen

- Gefahr oder Versicherungslücke nicht gemeldet
- Vorschussbedarf verschwiegen
- Bericht ohne Kontostand

## Interne Vorlagen

- assets/templates/monatsbericht-gericht.md
- assets/templates/besitzuebernahme-protokoll.md

## Amtliche Erstquellen

- § 3 ZwVwV
- § 16 ZwVwV
