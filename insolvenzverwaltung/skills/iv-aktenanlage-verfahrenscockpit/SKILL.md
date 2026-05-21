---
name: iv-aktenanlage-verfahrenscockpit
description: "Aktenanlage und Verfahrenscockpit für Insolvenzverwaltung. Erzeugt Aktenzeichen Beteiligtenregister Ordnerplan Massekonto Forderungstabelle Fristen und Workstreams freistehend."
---

# Aktenanlage und Verfahrenscockpit

## Aufgabe

Eröffnet eine saubere Verfahrensakte mit eigenem Aktenzeichen, Rollen, Ordnerplan, Tabellenlogik und Workstream-Register.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- ein neuer Beschluss, Gutachtenauftrag oder Sachwalterauftrag vorliegt
- eine unstrukturierte Datenlieferung sortiert werden muss
- bestehende Akten nicht auswertbar sind

## Eingaben

- Beschluss, Antrag, Schuldnerfragebogen
- Beteiligte, Banken, Arbeitnehmer, Sicherungsgläubiger
- erste Dokumente und Dateiliste

## Workflow

1. **Aktenkern** - Gericht, Aktenzeichen, Schuldner, Verwalterrolle, Stichtage und Fristen erfassen.
2. **Ordnung** - Ordnerplan für Gericht, Masse, Tabelle, Personal, Verträge, Anfechtung und Berichte erzeugen.
3. **Register** - Beteiligtenregister, Gläubigerliste, Drittschuldnerliste und Zustellwege anlegen.
4. **Kontrollpunkte** - Wiedervorlagen und Verantwortlichkeiten setzen.

## Ausgabe

- Mandatskarte
- Ordnerplan
- Beteiligtenregister
- Fristen- und Workstreamliste

## Qualitätsgates

- keine Partei ohne Rolle
- jede Frist mit Quelle
- keine Vermischung von Masse und Kanzleidaten

## Rote Schwellen

- fehlender Bestellungsbeschluss
- unklare Zuständigkeit
- fehlender Zahlungsweg für Massekonto

## Interne Vorlagen

- assets/templates/iv-mandatskarte.md
- assets/templates/glaeubigerausschuss-bericht.md

## Amtliche Erstquellen

- InsO Gesamtfassung
- §§ 27, 28 InsO
