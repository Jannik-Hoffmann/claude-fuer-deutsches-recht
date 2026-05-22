---
name: avv-grenzpruefung-datenschutz
description: "Schnittstelle zum Datenschutzrecht. Pruefe ob eine Auftragsverarbeitungsvereinbarung nach Art. 28 DS-GVO vorliegt und ob die berufsrechtliche Pruefung der vorliegenden Skills durch die AVV nicht ersetzt wird. AVV ist eigenstaendige andere Pruefung. Berufsrecht laeuft parallel und ist strenger. Wichtige Abgrenzungspunkte und Stolperfallen."
---

# AVV-Grenzprüfung Datenschutz

## Disclaimer

Diese Vorprüfung ist keine Rechtsberatung, sondern strukturierte Argumentationshilfe für das Anbietergespräch. Die abschließende berufsrechtliche und strafrechtliche Beurteilung bleibt der inhabilen Kanzlei beziehungsweise einer beauftragten Spezialkanzlei vorbehalten.

## Zweck dieser Skill

Diese Skill ist bewusst eine **Grenzprüfung**, keine vertiefte Datenschutzprüfung. Das Plugin behandelt das Berufsrecht und das Strafrecht. Die datenschutzrechtliche Prüfung ist eine eigene, parallele Aufgabe — sie wird häufig mit der berufsrechtlichen Prüfung verwechselt oder vermischt.

Das Plugin `datenschutzrecht` im selben Repository deckt diese Prüfung ab.

## Was die AVV regelt — und was nicht

Die Auftragsverarbeitungsvereinbarung nach Art. 28 DS-GVO regelt die Verarbeitung personenbezogener Daten. Sie regelt:

- Gegenstand, Dauer, Art und Zweck der Verarbeitung
- Kategorien betroffener Personen und Datenarten
- Pflichten und Rechte des Verantwortlichen
- Weisungsbindung des Auftragsverarbeiters
- TOM (Art. 32 DS-GVO)
- Unterauftragnehmer (Art. 28 Abs. 4 DS-GVO)
- Mitwirkungspflichten
- Löschung am Vertragsende

Die AVV regelt **nicht** das Berufsgeheimnis. Sie schützt nicht die Verschwiegenheit als solche, sondern den personenbezogenen Datenschutz. Beide Schutzregimes laufen parallel.

## Was das Berufsrecht zusätzlich verlangt

Die berufsrechtliche Dienstleisterregelung (§§ 43e BRAO, 62a StBerG, 50a WPO, 39c PAO, 26a BNotO) verlangt darüber hinaus:

- Verschwiegenheitspflicht in Textform — auch wenn keine personenbezogenen Daten verarbeitet werden (zum Beispiel anonymisierte Vertragsanalyse)
- Strafrechtliche Belehrung (§§ 203, 204 StGB)
- Festlegung Subunternehmer mit berufsrechtlicher (nicht datenschutzrechtlicher) Weiterverpflichtung
- Beachtung des § 203 Abs. 4 Satz 2 Nr. 1 StGB (Sekundärpflicht)

## DAV-Klarstellung

Die DAV-Stellungnahme 32/2025 (Seite 17 und 18) stellt klar:

- Beide Regelungsregimes (DS-GVO und Berufsrecht) gelten nebeneinander
- Die anwaltliche Verschwiegenheitspflicht ist breiter als die DS-GVO (sie erfasst auch nicht personenbezogene Geheimnisse wie Strategiepapiere)
- Anonymisierung oder Pseudonymisierung der Mandatsdaten ist nach der DS-GVO ein Mittel der Datenminimierung, **nicht** ein berufsrechtlich zwingendes Erfordernis — soweit der Dienstleister § 43e-konform verpflichtet ist (DAV S. 11)

## Prüfschema

| Punkt | Status | Bemerkung |
|---|---|---|
| AVV nach Art. 28 DS-GVO liegt vor | | |
| Aktueller Stand (Datum, Version) | | |
| Datenkategorien sind beschrieben | | |
| TOM nach Art. 32 DS-GVO (Anlage) | | |
| Subunternehmer nach Art. 28 Abs. 4 DS-GVO (Anlage) | | |
| Drittlandsübermittlung geregelt (SCC, Adequacy) | | |
| Verweis auf Berufsrecht im Vertrag | | |

## Typische Stolperfallen

- Anbieter argumentiert, die AVV decke alles ab — sie deckt das Berufsrecht nicht ab
- AVV verweist auf US-Datenschutzstandards — DSGVO-konform fraglich
- Pseudonymisierung wird angepriesen als "berufsrechtlich notwendig" — sie ist es nach DAV nicht (DAV S. 11)
- Trennung von Verschwiegenheit und Datenschutz fehlt
- Berufsrechtliche Verpflichtung in der AVV "versteckt" — sollte eigenständig erfolgen

## Output

Kurzer Zwischenstatus. Falls die AVV unzureichend ist, Hinweis auf das Plugin `datenschutzrecht` und den separaten Prüfprozess.
