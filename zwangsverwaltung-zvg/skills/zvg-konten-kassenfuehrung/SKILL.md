---
name: zvg-konten-kassenfuehrung
description: "Konten Kassenfuehrung und Buchfuehrung der Zwangsverwaltung. Führt Treuhandkonto Soll Ist Einnahmen Ausgaben Belege Vorschuss und Auskunft."
---

# Konten, Kasse und Buchführung

## Aufgabe

Führt die Finanzverwaltung mit getrenntem Treuhandkonto und prüffähiger Soll-Ist-Buchführung.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- Treuhandkonto einzurichten ist
- Zahlungen eingehen oder Ausgaben freigegeben werden
- Jahres- oder Schlussrechnung vorbereitet wird

## Eingaben

- Kontoauszüge, Belege, Rent Roll, Ausgaben
- Vorschussanforderungen, Gerichtskosten, Vergütung
- Vorjahressaldo und offene Posten

## Workflow

1. **Konto einrichten** - gesondertes Treuhandkonto und Zahlungsregeln dokumentieren.
2. **Buchen** - Soll- und Isteinnahmen, Ausgaben, Belege und Salden erfassen.
3. **Abgleichen** - Rent Roll, Konto, Belege und Vorschuss laufend abstimmen.
4. **Auskunft** - gerichtsfeste Auskunft und Unterlagenpaket vorbereiten.

## Ausgabe

- Konto- und Kassenbuch
- Soll-Ist-Abgleich
- Belegliste

## Qualitätsgates

- Masse getrennt von Eigenbeständen
- Einzelbuchungen ausgewiesen
- Belege zu jeder Buchung

## Rote Schwellen

- privates Konto
- nicht zuordenbare Bareinnahme
- fehlende Kontoauszüge

## Interne Vorlagen

- assets/templates/konto-kassenbuch.md
- assets/templates/rechnungslegung.md

## Amtliche Erstquellen

- § 13 ZwVwV
- § 14 ZwVwV
