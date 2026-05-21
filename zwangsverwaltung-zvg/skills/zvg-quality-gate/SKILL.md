---
name: zvg-quality-gate
description: "Quality Gate für Zwangsverwaltung. Prüft Beschluss Objekt Konto Rent Roll Berichte Rechnungslegung Verteilung Belege Rollen und Risiken vor Versand."
---

# Quality Gate für Zwangsverwaltung

## Aufgabe

Prüft ZVG-Arbeitsprodukte vor Versand oder Zahlung auf Rechenfehler, fehlende Belege und Rollenprobleme.

Der Skill arbeitet freistehend. Er setzt keine anderen Plugins voraus. Wenn Material fehlt, fragt er gezielt nach oder erzeugt einen klar markierten Simulations- bzw. Platzhalterstand.

## Startet bei

- Bericht, Rechnung, Verteilungsplan oder Schreiben fertig wirkt
- Zahlung oder Auszahlung vorbereitet wird
- ein kritischer Konflikt dokumentiert werden soll

## Eingaben

- Arbeitsprodukt
- Beschluss, Rent Roll, Konto, Belege
- Adressat, Zweck und Frist

## Workflow

1. **Rollencheck** - Zwangsverwalter, Schuldner, Gläubiger, Mieter und Gericht sauber trennen.
2. **Zahlencheck** - Soll-Ist, Saldo, Rückstände, Ausgaben und Verteilung prüfen.
3. **Belegcheck** - Fotos, Kontoauszüge, Rechnungen und Beschlüsse referenzieren.
4. **Freigabe** - Freigabe, Stopp oder Rückfrage mit Priorität ausgeben.

## Ausgabe

- QA-Vermerk
- Fehlerliste
- Freigabe- oder Stopp-Empfehlung

## Qualitätsgates

- keine Zahlung ohne Kontobeleg
- keine Verteilung ohne Rücklagenprüfung
- Berichte adressatengerecht

## Rote Schwellen

- falsches Konto
- fehlende Versicherung
- unbelegte Verteilung

## Interne Vorlagen

- assets/templates/quality-gate.md
- assets/templates/rechnungslegung.md

## Amtliche Erstquellen

- §§ 13 bis 16 ZwVwV
- § 155 ZVG
