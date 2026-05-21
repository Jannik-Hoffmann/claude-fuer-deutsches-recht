---
name: zvg-rechnungslegung
description: "Rechnungslegung der Zwangsverwaltung. Erstellt Jahresrechnung Schlussrechnung Endabrechnung Einnahmenueberschussrechnung Soll Ist Belege und Salden."
---

# Rechnungslegung

## Aufgabe

Erstellt prüffähige Jahresrechnung, Schlussrechnung und Endabrechnung nach ZwVwV.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- Kalenderjahr endet
- Zwangsverwaltung aufgehoben wird
- Gericht oder Beteiligte Auskunft verlangen

## Eingaben

- Kontoauszüge, Belege, Buchungsjournal
- Rent Roll, Anfangssaldo, Schlussbestand
- Vergütung, Gerichtskosten, Zahlungen an Gläubiger

## Workflow

1. **Daten schließen** - Zeitraum, Anfangsbestand, Endbestand, Kontoauszüge und Belege festlegen.
2. **Gliedern** - Soll-/Isteinnahmen und Ausgaben nach ZwVwV-Konten darstellen.
3. **Prüfen** - Saldo, Belege, USt-Option und Einzelbuchungen abgleichen.
4. **Einreichen** - Jahresrechnung, Schlussrechnung oder Endabrechnung mit Anlagen erstellen.

## Ausgabe

- Jahresrechnung
- Schlussrechnung
- Endabrechnung mit Belegliste

## Qualitätsgates

- Saldo rechnerisch stimmig
- Soll-Ist vollständig
- Umsatzsteuer gesondert, falls Option

## Rote Schwellen

- Konto nicht auf Null bei Endabrechnung
- fehlende Belege
- ungeklärter Anfangsbestand

## Interne Vorlagen

- assets/templates/rechnungslegung.md
- assets/templates/konto-kassenbuch.md

## Amtliche Erstquellen

- § 14 ZwVwV
- § 15 ZwVwV
