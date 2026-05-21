---
name: iv-eroeffnungsgutachten
description: "Eröffnungsgutachten nach InsO aus Sicht des Sachverstaendigen oder vorläufigen Insolvenzverwalters. Prüft Eröffnungsgrund Massekostendeckung Sicherung und Empfehlung."
---

# Eröffnungsgutachten

## Aufgabe

Erstellt die Arbeitsgliederung für ein Eröffnungsgutachten mit Sachverhalt, Eröffnungsgründen, Massekostendeckung, Sicherungsbedarf und gerichtlicher Empfehlung.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- das Gericht ein Gutachten zur Verfahrenseröffnung beauftragt
- Zahlungsunfähigkeit, drohende Zahlungsunfähigkeit oder Überschuldung zu prüfen ist
- eine Fortführung bis zur Eröffnung möglich erscheint

## Eingaben

- Antrag und Anlagen
- BWA, SuSa, OPOS, Bankdaten, Lohn- und Steuerstände
- Vermögensverzeichnis und Sicherheiten

## Workflow

1. **Sachverhalt sichern** - Antrag, Gesellschaft, Geschäftsbetrieb und Unterlagenstand darstellen.
2. **Eröffnungsgründe prüfen** - § 17, § 18 und § 19 InsO anhand konkreter Zahlen trennen.
3. **Masse prüfen** - freie Masse, Kosten, Verwertung, Vorschuss und Massearmut abgleichen.
4. **Empfehlung bauen** - Eröffnung, Abweisung, Sicherungsmaßnahmen oder weitere Aufklärung begründen.

## Ausgabe

- Gutachtengliederung
- Zahlen- und Belegliste
- Empfehlungsentwurf an das Insolvenzgericht

## Qualitätsgates

- Eröffnungsgrund und Kostendeckung getrennt
- jede Zahl mit Quelle
- fehlende Unterlagen als Aufklärungsbedarf markiert

## Rote Schwellen

- Kassenbestand nicht verifiziert
- Sicherheiten ungeklärt
- Betriebsfortführung ohne Liquiditätsbrücke

## Interne Vorlagen

- assets/templates/eroeffnungsgutachten-gliederung.md
- assets/templates/liquiditaetsstatus-kurzcheck.md

## Amtliche Erstquellen

- §§ 16 bis 19 InsO
- § 26 InsO
