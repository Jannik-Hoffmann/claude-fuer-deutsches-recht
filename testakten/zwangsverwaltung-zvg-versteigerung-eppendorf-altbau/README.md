# Testakte ZVG-Versteigerung Eppendorf Altbau

Fiktive Testakte für `zwangsverwaltung-zvg`. Der Fall spielt in Hamburg-Eppendorf und simuliert ein vermietetes Wohnungseigentum in einem alten Mehrfamilienhaus. Die Akte eignet sich für:

- ZVG-Portal-Recherche
- Auswertung von Grundbuchauszug und Verkehrswertgutachten
- Bewertung eines Bieterangebots
- Vorbereitung der Teilnahme am Versteigerungstermin
- Schnittstelle zwischen Zwangsverwaltung, Mietverwaltung und Zwangsversteigerung

## Fiktions- und Anonymisierungshinweis

Diese Akte ist vollständig fiktiv. Sie wurde nur strukturell durch typische ZVG-Unterlagen inspiriert. Namen, Grundbuchblatt, Gemarkung, Flurstück, Straße, Aktenzeichen, Gerichtsdaten und Mieterdaten sind frei erfunden. Originalfotos und echte Lagebilder werden nicht übernommen; an diesen Stellen stehen Platzhalter.

## Enthaltene Unterlagen

| Datei | Zweck |
| --- | --- |
| `00_hinweis_anonymisierung.md` | Fiktions- und Abgrenzungsvermerk |
| `01_zvg_portal_rechercheprotokoll.md` | dokumentierte ZVG-Portal-Suche Hamburg/Eppendorf |
| `02_terminsbekanntmachung.md` | fiktive Terminsbekanntmachung |
| `03_grundbuchauszug_anonymisiert.md` | fiktiver Wohnungsgrundbuchauszug |
| `04_verkehrswertgutachten_kurzfassung.md` | fiktive Gutachten-Kurzfassung ohne Fotos |
| `05_mietvertrag_kurznotiz.md` | Mietvertrags- und Nutzungsnotiz |
| `06_bieterangebot_bewertung.md` | Beispielbewertung eines Bieterangebots |
| `07_versteigerungsteilnahme_checkliste.md` | Termin- und Sicherheitsleistungscheck |
| `08_risikomatrix.csv` | strukturierte Risiken |
| `09_bietlimit_rechenblatt.csv` | einfache Bietlimit-Rechnung |
| `10_quality_gate.md` | Prüfpunkte vor Ausgabe |

## Schnellstart

1. `/zwangsverwaltung-zvg:zvg-portal-recherche` auf `01_zvg_portal_rechercheprotokoll.md` anwenden.
2. `/zwangsverwaltung-zvg:zvg-bieterangebot-bewertung` auf die Gesamtakte anwenden.
3. `/zwangsverwaltung-zvg:zvg-versteigerungsteilnahme` zur Terminvorbereitung starten.
