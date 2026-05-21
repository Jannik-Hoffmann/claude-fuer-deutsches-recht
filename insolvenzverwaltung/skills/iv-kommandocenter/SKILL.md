---
name: iv-kommandocenter
description: "Insolvenzverwaltungs-Kommandocenter für Insolvenzverwalter Sachwalter und vorläufige Verwaltung. Triage Regelverfahren Eigenverwaltung Schutzschirm Anfechtung Forderungsprüfung Masse und Berichte."
---

# Insolvenzverwaltungs-Kommandocenter

## Aufgabe

Führt als erste Schaltstelle durch ein Insolvenzverwaltungsmandat aus Sicht des Insolvenzverwalters, vorläufigen Insolvenzverwalters oder Sachwalters.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- neue Bestellung, Gutachtenauftrag oder laufende Verfahrensakte eingeht
- unklar ist, ob Regelverfahren, Eigenverwaltung oder Schutzschirm betroffen ist
- eine schnelle Tagespriorisierung gebraucht wird

## Eingaben

- Beschluss oder Gutachtenauftrag
- Schuldnerdaten, Gericht, Aktenzeichen, Stichtage
- erste OPOS-, Bank-, Lohn- und Vermögenslisten

## Workflow

1. **Einordnen** - Verfahrensart, Rolle, Sicherungsmaßnahmen und rote Fristen erfassen.
2. **Akte bauen** - Verfahrenskarte, Beteiligtenregister, Masseampel und nächste Workstreams anlegen.
3. **Risiko priorisieren** - Betriebsfortführung, Massearmut, Lohn, Steuern, Anfechtung, § 15b InsO und Berichtspflichten gewichten.
4. **Arbeitsauftrag ausgeben** - Nächste drei Aktionen mit Beleganforderungen und Rückfragen formulieren.

## Ausgabe

- Verfahrenskarte mit Ampel
- Priorisierte To-do-Liste
- Rückfragen an Schuldner, Gericht, Banken und Dritte

## Qualitätsgates

- Aktenzeichen und Bestellungsumfang sind geprüft
- Rolle und Befugnisse sind nicht vermischt
- jede Empfehlung nennt Beleg oder fehlenden Beleg

## Rote Schwellen

- unklare Kassenlage
- drohende Masseunzulänglichkeit
- fortlaufende Zahlungen ohne Zustimmung oder Prüfung

## Interne Vorlagen

- assets/templates/iv-mandatskarte.md
- assets/templates/quality-gate.md

## Amtliche Erstquellen

- InsO §§ 21 ff., 56, 80 ff., 270 ff.
- § 208 InsO
