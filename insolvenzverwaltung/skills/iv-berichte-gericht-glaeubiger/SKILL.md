---
name: iv-berichte-gericht-glaeubiger
description: "Berichte an Insolvenzgericht Gläubigerausschuss und Gläubigerversammlung. Erstellt Zwischenbericht Sachstandsbericht Beschlussvorlage und Ampelbericht."
---

# Berichte an Gericht und Gläubigerorgane

## Aufgabe

Erzeugt klare, prüfbare Berichte für Insolvenzgericht, Gläubigerausschuss und Gläubigerversammlung.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- Zwischenbericht, Sachstandsbericht oder Ausschussbericht fällig ist
- wichtige Verwertungs- oder Fortführungsentscheidungen anstehen
- Gläubigerkommunikation konsistent werden muss

## Eingaben

- Verfahrensstatus, Masse, Tabelle, Verwertung
- Prozess- und Anfechtungsstand, Fortführung, Kosten
- gerichtliche Verfügung oder Ausschussagenda

## Workflow

1. **Berichtsstand** - Stichtag, Zeitraum und Adressat festlegen.
2. **Faktenblock** - Masse, Tabelle, Verwertung, Prozesse, Personal, Steuern und Risiken aktualisieren.
3. **Entscheidungen** - Beschlussbedarf, Optionen und Empfehlung formulieren.
4. **Belege** - Anlagen, Tabellen und Nachweise referenzieren.

## Ausgabe

- Zwischenbericht
- Ausschussbericht
- Beschlussvorlage mit Anlagenliste

## Qualitätsgates

- keine Bewertung ohne Zahlenstand
- Adressatengerechte Tiefe
- offene Punkte klar markiert

## Rote Schwellen

- Masseunzulänglichkeit verschwiegen
- Quote ohne Basis
- Interessenkonflikt bei Verwertung

## Interne Vorlagen

- assets/templates/zwischenbericht.md
- assets/templates/glaeubigerausschuss-bericht.md

## Amtliche Erstquellen

- InsO Berichtspflichten nach Verfahrenslage
- § 156 InsO als Berichtstermin-Schnittstelle
