---
name: zvg-mieteinzug-rueckstaende
description: "Mieteinzug Rückstände und Zahlungsabgleich in der Zwangsverwaltung. Führt Soll Ist Mahnung Ratenzahlung Klage Zahlungseingang und Kontoabgleich."
---

# Mieteinzug und Rückstände

## Aufgabe

Sichert laufende Nutzungen und treibt Rückstände mit sauberem Soll-Ist-Abgleich ein.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- Mieteinnahmen fehlen
- Rückstände vor oder nach Beschlagnahme bestehen
- Zahlungen nicht zugeordnet werden können

## Eingaben

- Rent Roll, Kontoauszüge, Mieterkonten
- Rückstandsliste, Mahnungen, Einwendungen
- Mietverträge und Betriebskostenstände

## Workflow

1. **Soll-Ist-Abgleich** - Sollmieten je Einheit mit Zahlungseingängen und Altrückständen matchen.
2. **Rückstände trennen** - beschlagnahmte Nutzungen, Altansprüche und streitige Posten unterscheiden.
3. **Mahnen** - freundliche Zahlungserinnerung, Mahnung, Ratenplan oder Klagevorschlag erstellen.
4. **Gericht berichten** - wesentliche Rückstände und Einziehungsmaßnahmen dokumentieren.

## Ausgabe

- Rückstandsliste
- Mahn- und Klagepaket
- Zahlungsabgleich

## Qualitätsgates

- jede Zahlung einer Einheit zugeordnet
- Alt- und Neurückstände getrennt
- Einwendungen protokolliert

## Rote Schwellen

- Dauerleerstand
- Mietminderung ohne Prüfung
- Kontoauszug fehlt

## Interne Vorlagen

- assets/templates/mieteinzug-rueckstaende.md
- assets/templates/konto-kassenbuch.md

## Amtliche Erstquellen

- § 8 ZwVwV
- § 13 ZwVwV
