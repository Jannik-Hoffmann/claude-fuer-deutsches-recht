---
name: zvg-portal-recherche
description: "Recherchiert Zwangsversteigerungstermine im amtlichen ZVG-Portal, dokumentiert Suchparameter, Treffer, Gutachten-/Exposee-Downloads und Grenzen der Recherche."
---

# ZVG-Portal-Recherche

## Aufgabe

Führt eine belegbare Recherche im amtlichen ZVG-Portal durch und macht daraus ein Rechercheprotokoll für Akte, Bieterprüfung oder Verwalterkommunikation.

## Startet bei

- Auftrag: "Suche im ZVG-Portal"
- Prüfung eines Aktenzeichens, Gerichts, Ortes, Ortsteils, Objekttyps oder Termins
- Abgleich, ob Gutachten, Exposee oder Fotos im Portal verfügbar sind

## Workflow

1. **Suchziel klären**: Gericht, Bundesland, Ort, Ortsteil, Straße, Aktenzeichen, Objektart, Terminfenster.
2. **Portal öffnen**: `https://www.zvg-portal.de/index.php?button=Termine%20suchen`.
3. **Parameter dokumentieren**: Bundesland, Gericht, Verfahrensart, Objektart, Straße, PLZ, Ort, Ortsteil, Termin von/bis, Sortierung.
4. **Treffer sichern**: Trefferzahl, Aktenzeichen, Gericht, Objektbeschreibung, Verkehrswert, Termin, Detail-URL, Abrufdatum.
5. **Downloads prüfen**: Gutachten, Exposee, Fotos nur vermerken; keine fremden Fotos in Test- oder Arbeitsakten übernehmen.
6. **Negativtreffer festhalten**: Auch "0 Treffer" ist ein verwertbares Rechercheergebnis.
7. **Grenzen notieren**: Portal ist Veröffentlichungsplattform. Maßgeblich bleiben Bekanntmachung, Gerichtsakte, Grundbuch und Termin.

## Ausgabe

- Rechercheprotokoll mit URL, Datum, Suchparametern, Trefferliste und offenem Nachfassbedarf
- Kurzvermerk für Akte oder Mandantenkommunikation

## Qualitätsgates

- Abrufdatum und Uhrzeit enthalten
- Suchparameter so konkret, dass die Recherche wiederholbar ist
- Treffer nicht mit materieller Rechtsprüfung verwechselt
- Bei Portalfehler oder leerem Treffer: keine Fantasie-Treffer erzeugen

## Rote Schwellen

- Behaupteter Termin ohne Treffer-/Gerichtsbeleg
- Download fremder Fotos in eine Demo- oder Testakte
- Verwechslung privater ZVG-Portale mit dem amtlichen Portal

## Interne Vorlage

- `assets/templates/zvg-portal-rechercheprotokoll.md`

## Amtliche Erstquellen

- Amtliches Portal: `https://www.zvg-portal.de/`
- Suchformular: `https://www.zvg-portal.de/index.php?button=Termine%20suchen`
