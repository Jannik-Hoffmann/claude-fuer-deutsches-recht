---
name: iv-qualitaets-und-plausibilitaetsgate
description: "Qualitaets und Plausibilitaetsgate für Insolvenzverwaltung. Prüft Rollen Fristen Rechenwerke Quellen Tabellen Berichte Anfechtung § 15b und Masse."
---

# Qualitäts- und Plausibilitätsgate

## Aufgabe

Prüft IV-Arbeitsergebnisse vor Versand oder Entscheidung auf Widersprüche, Rechenfehler, fehlende Belege und Rollenfehler.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- ein Gutachten, Bericht, Klageentwurf oder eine Anzeige versandt werden soll
- Tabellen, Verteilung oder Masseberechnung fertig wirken
- mehrere Workstreams zusammengeführt werden

## Eingaben

- Arbeitsprodukt
- Zahlenanlagen, Quellen, Aktennotizen
- Adressat und Zweck

## Workflow

1. **Rollencheck** - Verwalter, Sachwalter, Schuldnerin, Gericht und Gläubiger nicht vermischen.
2. **Zahlencheck** - Summen, Stichtage, Quoten, Zahlungslisten und Tabellenverweise prüfen.
3. **Normencheck** - einschlägige Normen und amtliche Quellen plausibilisieren.
4. **Lückencheck** - fehlende Belege, Annahmen und rote Schwellen offenlegen.

## Ausgabe

- QA-Vermerk
- Fehlerliste mit Prioritäten
- Freigabe- oder Stopp-Empfehlung

## Qualitätsgates

- keine blinden Quellen
- keine Zahl ohne Anlage
- jede rote Schwelle bewertet

## Rote Schwellen

- unbelegte Insolvenzreife
- vertauschte Rangklasse
- fehlender § 208-Check bei negativer Masseprognose

## Interne Vorlagen

- assets/templates/quality-gate.md
- assets/templates/liquiditaetsstatus-kurzcheck.md

## Amtliche Erstquellen

- InsO Gesamtfassung
- amtliche Normseiten im Quellenverzeichnis
