---
name: iv-verteilung-schlussrechnung
description: "Schlussbericht Schlussrechnung und Verteilung im Insolvenzverfahren. Erstellt Quote Verteilungsverzeichnis Schlussrechnung Bericht Anlagen und Nachtragsverteilung."
---

# Schlussbericht, Schlussrechnung und Verteilung

## Aufgabe

Führt die Abschlussphase des Verfahrens: Schlussbericht, Schlussrechnung, Verteilungsverzeichnis, Quote und Nachtragsverteilung.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- Verwertung abgeschlossen oder weitgehend abgeschlossen ist
- Schlussverteilung vorbereitet wird
- Gericht Schlussbericht oder Schlussrechnung erwartet

## Eingaben

- Massekonto, Buchhaltung, Verwertungserlöse
- Tabelle, Rangklassen, Kosten, Vergütung
- offene Prozesse und Nachtragsrisiken

## Workflow

1. **Abschlussreife** - offene Masse, Prozesse, Steuern und Verwertung prüfen.
2. **Rechnung** - Einnahmen, Ausgaben, Kosten, Vergütung und Belege konsolidieren.
3. **Verteilung** - Rang, Quote, Abschläge und Verteilungsverzeichnis erstellen.
4. **Bericht** - Schlussbericht, Anlagenliste und Nachtragsverteilungsnotiz ausgeben.

## Ausgabe

- Schlussbericht
- Schlussrechnung
- Verteilungsverzeichnis

## Qualitätsgates

- Massekonto stimmt mit Buchhaltung
- Tabelle final geprüft
- Nachtragspositionen markiert

## Rote Schwellen

- offener Prozess mit Quotenwirkung
- nicht gebuchte Kosten
- Rangfehler

## Interne Vorlagen

- assets/templates/schlussbericht-schlussrechnung.md
- assets/templates/verteilungsverzeichnis.md

## Amtliche Erstquellen

- §§ 187 ff. InsO
- §§ 196 ff. InsO
