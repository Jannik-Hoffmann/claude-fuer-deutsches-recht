---
name: cloud-act-und-drittstaat-pruefen
description: "Pruefe Auslandsbezug des KI-Anbieters nach Absatz vier der einschlaegigen Dienstleisterregelung (BRAO StBerG WPO PAO BNotO). EU/EWR werden als gleichwertig unterstellt. Drittstaaten benoetigen vergleichbares Schutzniveau. US-CLOUD Act und Foreign Intelligence Surveillance Act schaffen Restzugriff. Professional Secrecy Addendum empfohlen. DAV-Stellungnahme Seite fuenfzehn sechzehn."
---

# Cloud Act und Drittstaat prüfen

## Disclaimer

Diese Vorprüfung ist keine Rechtsberatung, sondern strukturierte Argumentationshilfe für das Anbietergespräch. Die abschließende berufsrechtliche und strafrechtliche Beurteilung bleibt der inhabilen Kanzlei beziehungsweise einer beauftragten Spezialkanzlei vorbehalten.

## Norm

Absatz 4 der jeweiligen Dienstleisterregelung. Wortlaut (am Beispiel § 43e Abs. 4 BRAO; identisch in § 62a Abs. 4 StBerG, § 50a Abs. 4 WPO, § 39c Abs. 4 PAO; bei § 26a BNotO entsprechend):

"Bei der Inanspruchnahme von Dienstleistungen, die im Ausland erbracht werden, darf der Rechtsanwalt dem Dienstleister den Zugang zu fremden Geheimnissen unbeschadet der übrigen Voraussetzungen dieser Vorschrift nur dann eröffnen, wenn der dort bestehende Schutz der Geheimnisse dem Schutz im Inland vergleichbar ist, es sei denn, dass der Schutz der Geheimnisse dies nicht gebietet."

## DAV-Lesart

DAV-Stellungnahme 32/2025 (Seite 15): EU-Mitgliedstaaten erfüllen aufgrund der Harmonisierung anwaltlicher Berufspflichten in der Regel das Erfordernis des vergleichbaren Schutzes. Außerhalb der EU/des EWR ist die Vergleichbarkeit einzelfallabhängig zu prüfen.

Wichtig: Die Vergleichbarkeit bezieht sich auf den Schutz der Geheimnisse, nicht auf das allgemeine Rechtsschutzniveau. Selbst wenn ein Land eine funktionierende Justiz hat, kann der Schutz von Berufsgeheimnissen mangelhaft sein.

## Problemzone USA

Die USA stellen die größte praktische Herausforderung dar, weil die meisten LLM-Anbieter dort ansässig sind oder dort verarbeiten lassen.

### CLOUD Act (2018)

Der US-Clarifying Lawful Overseas Use of Data Act verpflichtet US-Anbieter und ihre weltweiten Töchter, US-Behörden auf Anordnung Zugang zu Daten zu gewähren, auch wenn diese außerhalb der USA gespeichert sind. Eine deutsche Hostinglokation schützt also nicht.

### FISA Section 702

Der Foreign Intelligence Surveillance Act erlaubt US-Geheimdiensten Zugriff auf elektronische Kommunikation von Nicht-US-Personen ohne richterlichen Beschluss. Praktisch betroffen sind insbesondere große Cloudanbieter und LLM-Provider.

### Konsequenz

Bei US-Anbietern besteht ein struktureller Restzugriff durch US-Behörden, der mit dem deutschen Berufsgeheimnis nicht vollständig kompatibel ist. Die DAV-Stellungnahme verlangt nicht den vollständigen Verzicht auf US-Anbieter, aber sie verlangt eine sorgfältige Abwägung und vertragliche Absicherung.

## Professional Secrecy Addendum

Bei US-Anbietern empfehlenswert: ein eigenes Berufsgeheimnis-Addendum zum Hauptvertrag, das

- die berufsrechtlichen Anforderungen explizit übernimmt
- den Anbieter zur Anfechtung jedes US-Auskunftsverlangens verpflichtet
- den Anbieter zur unverzüglichen Information der Kanzlei verpflichtet, soweit gesetzlich zulässig
- den Anbieter zur Datenminimierung in Richtung USA verpflichtet (keine US-Backups, keine US-Logs)
- Gerichtsstand und anwendbares Recht in Deutschland

Microsoft und Google haben für ihre Cloud-Dienste teilweise solche Addenda anerkannt; OpenAI nur eingeschränkt.

## Prüfschema

| Punkt | Status | Ampel | Bemerkung |
|---|---|---|---|
| Sitz Anbieter (Hauptvertragspartei) | | | |
| Konzernzugehörigkeit (US-Konzern?) | | | |
| Verarbeitungsstandort | | | |
| Backup-Standort | | | |
| Modellanbieter (etwa OpenAI) Standort | | | |
| Hoster Standort | | | |
| CLOUD-Act-Anwendbarkeit | | | |
| FISA-Anwendbarkeit | | | |
| Professional Secrecy Addendum | | | |
| Gerichtsstand Deutschland | | | |
| Anwendbares deutsches Recht | | | |
| Standardvertragsklauseln (SCC) | | | |
| Adequacy decision (EU-US-DPF) | | | |

## EU-US-Data Privacy Framework

Das 2023 in Kraft getretene Data Privacy Framework regelt den datenschutzrechtlichen Datentransfer in die USA. **Es regelt nicht das Berufsgeheimnis.** Es schützt nicht vor CLOUD-Act-Zugriffen. Der DPF ist datenschutzrechtlich relevant, berufsrechtlich nur als Indiz für ein gewisses Schutzniveau, nicht als Genehmigung.

## Empfehlungen

- Bei EU/EWR-Anbietern: Auslandsbezug grundsätzlich unproblematisch
- Bei US-Anbietern: Professional Secrecy Addendum, EU-Hosting-Zusicherung, kein US-Backup
- Bei Anbietern aus sonstigen Drittstaaten (China, Indien): in der Regel rote Ampel — Vergleichbarkeit muss positiv nachgewiesen werden

## Output

Tabellarische Bewertung. Bei US-Bezug: Vorlage für Professional Secrecy Addendum aus dem Skill `klauselvorschlaege`.
