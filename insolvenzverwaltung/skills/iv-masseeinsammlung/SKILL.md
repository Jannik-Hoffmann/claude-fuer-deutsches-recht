---
name: iv-masseeinsammlung
description: "Masseeinsammlung für Insolvenzverwalter. Ermittelt Bankguthaben Debitoren Herausgabeansprüche Drittschuldner Versicherungen Rückstände und Belege."
---

# Masseeinsammlung

## Aufgabe

Erfasst und realisiert Massepositionen: Geld, Forderungen, Herausgabeansprüche, Versicherungen, Debitoren, Rückstände und streitige Ansprüche.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- Massebestand unvollständig ist
- Banken, Kunden, Versicherer oder Drittschuldner angeschrieben werden müssen
- kurzfristig Liquidität für Kosten und Fortführung gebraucht wird

## Eingaben

- Banklisten, OPOS, Debitoren, Verträge
- Anlagenverzeichnis, Versicherungen, Prozesslisten
- Korrespondenz mit Drittschuldnern

## Workflow

1. **Massekarte** - Alle potenziellen Massepositionen mit Beleg, Schuldner, Fälligkeit und Durchsetzbarkeit anlegen.
2. **Priorisieren** - schnell realisierbare Forderungen vor streitigen Ansprüchen; Sicherheiten trennen.
3. **Anschreiben** - Drittschuldner-, Bank-, Kunden- und Herausgabeschreiben vorbereiten.
4. **Nachhalten** - Zahlungseingänge matchen, Mahnstufen und Klageoptionen steuern.

## Ausgabe

- Masseeinsammlungsregister
- Drittschuldneranschreiben
- Einziehungs- und Mahnplan

## Qualitätsgates

- Absonderungsrechte geprüft
- Fälligkeit und Anspruchsgrund dokumentiert
- Eingänge mit Forderungen gematcht

## Rote Schwellen

- Zahlung an Schuldner statt Massekonto
- ungeklärte Sicherungsabtretung
- Verjährung oder Ausschlussfrist

## Interne Vorlagen

- assets/templates/masseverzeichnis.md
- assets/templates/massenachverfolgung.csv

## Amtliche Erstquellen

- §§ 80 ff. InsO
- §§ 166 ff. InsO
