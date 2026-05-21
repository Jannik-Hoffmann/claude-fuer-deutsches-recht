---
name: zvg-bieterangebot-bewertung
description: "Bewertet Zwangsversteigerungsobjekte und Bieterangebote aus Investorensicht: Verkehrswert, geringstes Gebot, Sicherheitsleistung, bestehenbleibende Rechte, Mietlage, Sanierungsrisiko und Bietlimit."
---

# Bieterangebot Bewerten

## Aufgabe

Bewertet ein Objekt aus der Zwangsversteigerung oder ein vor-/außerterminliches Angebot. Der Skill ersetzt keine Finanzierung, Besichtigung oder anwaltliche Endprüfung; er macht die Risiken entscheidungsfähig.

## Startet bei

- "Ist dieses Versteigerungsangebot attraktiv?"
- "Welches Bietlimit ist plausibel?"
- "Was bedeutet Mindestgebot?"
- "Wie bewerte ich Gutachten, Grundbuch und Mietvertrag?"

## Workflow

1. **Unterlagen inventarisieren**: Bekanntmachung, Gutachten, Grundbuch, Teilungserklärung, Mietvertrag, Hausgeld, Protokolle, Baulasten, Energie, Versicherungen.
2. **Rechtsbegriffe sauberziehen**: Umgangssprachlich "Mindestgebot" meist vom rechtlichen "geringsten Gebot" unterscheiden.
3. **Wertbasis prüfen**: Verkehrswert, Stichtag, Innen-/Außenbesichtigung, Bewertungsverfahren, Abschläge, Vergleichsdaten, Marktrisiko.
4. **Lasten prüfen**: Abteilung II, Abteilung III soweit bekannt, bestehenbleibende Rechte, Rückstände, öffentliche Lasten, WEG-Hausgeld, Sonderumlagen.
5. **Nutzung prüfen**: Mietvertrag, tatsächliche Nutzung, Klingel-/Briefkasten-Abweichungen, Renovierungsabreden, Kündigungs-/Räumungsrisiko.
6. **Bietlimit rechnen**: Maximalbudget minus Sicherheitsabschlag, Erwerbsnebenkosten, Sanierung, Leerstand, Prozesskosten, Finanzierungspuffer und bestehenbleibende Rechte.
7. **Ampel ausgeben**: GRÜN nur bei belegtem Wert, klaren Lasten und ausreichendem Puffer; sonst GELB/ROT mit Nachforderungen.

## Ausgabe

- Bieterangebots-Matrix
- Bietlimit mit Annahmen
- offene Fragen an Gericht, Verwalter, WEG-Verwaltung, Bank oder Sachverständigen
- Entscheidung: beobachten, nachrecherchieren, bieten, nicht bieten

## Qualitätsgates

- Keine Gewährleistungsannahmen: ZVG-Erwerb ist kein normaler Kaufvertrag.
- Geringstes Gebot und 5/10-/7/10-Grenzen werden getrennt erläutert.
- Sicherheitsleistung wird auf Basis des Verkehrswerts geprüft.
- Bietlimit enthält Finanzierung und Liquidität, nicht nur Kaufpreis.

## Rote Schwellen

- Nur Außenbesichtigung und zugleich hoher Sanierungshebel
- unklare tatsächliche Nutzung oder gewerbliche Hinweise in Wohnraum
- bestehenbleibende Rechte nicht verstanden
- Angebot drängt zu schneller Zahlung außerhalb klarer Gerichts-/Notarstruktur

## Interne Vorlage

- `assets/templates/bieterangebot-bewertung.md`
