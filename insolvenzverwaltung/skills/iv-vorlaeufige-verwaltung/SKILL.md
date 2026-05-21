---
name: iv-vorlaeufige-verwaltung
description: "Vorläufige Insolvenzverwaltung mit Sicherungsmaßnahmen Zustimmungsvorbehalt Kassensturz Banken Post Drittschuldner Betrieb und Tagessteuerung bis zur Eröffnung."
---

# Vorläufige Insolvenzverwaltung

## Aufgabe

Führt die ersten Tage nach Bestellung als vorläufiger Insolvenzverwalter mit Zustimmungsvorbehalt oder starker Verwaltung.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- Beschluss nach § 21 InsO vorliegt
- Banken, Kasse, Post und Drittschuldner sofort gesichert werden müssen
- der Betrieb bis zur Entscheidung fortgeführt wird

## Eingaben

- Sicherungsbeschluss
- Bank- und Kassenstände
- Debitoren, Kreditoren, Arbeitnehmer, Lieferanten

## Workflow

1. **Befugnisse lesen** - Beschlussumfang, Zustimmungsvorbehalt, Postsperre und Verfügungsverbote auswerten.
2. **Masse sichern** - Banken, Kasse, Forderungen, Warenlager und Schlüssel kontrollieren.
3. **Kommunikation** - Schuldner, Banken, Drittschuldner, Arbeitnehmer und Gericht informieren.
4. **Tagessteuerung** - Zahlungen nur nach Freigabe, Beleg und Masseinteresse dokumentieren.

## Ausgabe

- Sofortmaßnahmenliste
- Bank- und Kassenprotokoll
- Zahlungsfreigabeprotokoll

## Qualitätsgates

- Beschlussbefugnisse werden wörtlich beachtet
- jede Zahlung hat Zweck, Beleg und Freigabe
- Drittschuldner sind informiert

## Rote Schwellen

- Zahlungen außerhalb des Freigabeprozesses
- fehlender Kassensturz
- unklare Eigentums- oder Sicherungsrechte

## Interne Vorlagen

- assets/templates/vorlaeufige-verwaltung-checkliste.md
- assets/templates/zahlungslauf-freigabe.md

## Amtliche Erstquellen

- § 21 InsO
- § 22 InsO
