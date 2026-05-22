---
name: subunternehmer-regelung-pruefen
description: "Pruefe die Subunternehmerklausel im KI-Anbietervertrag. Norm Absatz drei Satz zwei Nummer drei der einschlaegigen Dienstleisterregelung. Pflichtinhalte Zustimmungsvorbehalt der Kanzlei Subunternehmerliste Weiterverpflichtung in Textform Belehrung. Strafrechtliche Sekundaerpflicht nach § 203 Absatz vier Satz zwei Nummer eins StGB. Modellanbieter und Hoster als typische Subunternehmer."
---

# Subunternehmer-Regelung prüfen

## Disclaimer

Diese Vorprüfung ist keine Rechtsberatung, sondern strukturierte Argumentationshilfe für das Anbietergespräch. Die abschließende berufsrechtliche und strafrechtliche Beurteilung bleibt der inhabilen Kanzlei beziehungsweise einer beauftragten Spezialkanzlei vorbehalten.

## Norm

Absatz 3 Satz 2 Nr. 3 der jeweiligen Dienstleisterregelung. Der Vertrag mit dem Dienstleister muss festlegen, ob der Dienstleister befugt ist, weitere Personen zur Erfüllung des Vertrags heranzuziehen. Für diesen Fall ist dem Dienstleister aufzuerlegen, diese Personen in Textform zur Verschwiegenheit zu verpflichten.

Pro Beruf:

- § 43e Abs. 3 Satz 2 Nr. 3 BRAO
- § 62a Abs. 3 Satz 2 Nr. 3 StBerG
- § 50a Abs. 3 Satz 2 Nr. 3 WPO
- § 39c Abs. 3 Satz 2 Nr. 3 PAO
- § 26a Abs. 3 Satz 2 Nr. 3 BNotO

Strafrechtlich ergänzend: § 203 Abs. 3 Satz 2 StGB (Befugnis zur Weitergabe an mitwirkende Personen, die ihrerseits weitere Personen einbinden) und § 203 Abs. 4 Satz 2 Nr. 1 StGB (Sekundärpflicht zur Verpflichtung).

## Praxisproblem LLM-Anbieter

KI-Anbieter sind oft mehrstufige Strukturen:

1. **Frontend-Anbieter** (deutsche Vertragspartei, etwa ein Münchner Legal-Tech-Start-up)
2. **Modellanbieter** (etwa OpenAI, Anthropic, Mistral, Aleph Alpha)
3. **Hoster** (Microsoft Azure, AWS, Google Cloud)
4. **Eventuell Trainingsdienstleister**, **Annotation-Dienstleister**, **Support-Dienstleister**

Aus berufsrechtlicher Sicht sind alle vier Stufen Subunternehmer im Sinne von Abs. 3 Satz 2 Nr. 3. Der Frontend-Anbieter muss sie alle benennen und entsprechend weiterverpflichten.

## Anforderungen

### Festlegung im Vertrag

Der Vertrag muss explizit klären, ob der Dienstleister Subunternehmer einsetzen darf. Stillschweigen reicht nicht.

### Subunternehmerliste

Auch wenn die Norm das nicht ausdrücklich verlangt, ist eine **abschließende Liste der Subunternehmer mit Sitz, Funktion und gegebenenfalls Hosting-Ort** der Stand guter Praxis. Sie ist Vertragsanlage oder per Link zu einem versionierten Trust Center.

### Zustimmungsvorbehalt

Ein **Zustimmungsvorbehalt der Kanzlei vor Hinzunahme oder Wechsel von Subunternehmern** ist nicht durch das Berufsrecht zwingend gefordert, aber sehr empfehlenswert. Die DAV-Stellungnahme stellt klar, dass die Kanzlei für die Auswahl die berufsrechtliche Verantwortung trägt (Sorgfaltsanforderung Abs. 2 der Dienstleisterregelung).

### Weiterverpflichtung in Textform

Der Vertrag muss den Dienstleister verpflichten, jeden Subunternehmer **in Textform** zur Verschwiegenheit zu verpflichten — mit denselben inhaltlichen Anforderungen, die für den Dienstleister selbst gelten (gegenüber jedermann, zeitlich unbegrenzt, alle Berufsgeheimnisse, Belehrung).

### Belehrung über strafrechtliche Folgen

Auch die Subunternehmer müssen über §§ 203, 204 StGB belehrt werden (Abs. 4 Satz 2 Nr. 1 StGB).

## Prüfschema

| Punkt | Fundstelle | Ampel | Bemerkung |
|---|---|---|---|
| Festlegung Befugnis im Vertrag | | | |
| Aktuelle Subunternehmerliste vorhanden | | | |
| Zustimmungsvorbehalt der Kanzlei | | | |
| Weiterverpflichtungspflicht (Textform) | | | |
| Belehrungspflicht für Subunternehmer | | | |
| Informationspflicht bei Wechsel | | | |

## Typische Lücken

- "Wir setzen Subunternehmer nach unserem Ermessen ein" — Pflicht zur Festlegung verletzt
- Subunternehmerliste nur als unverbindlicher FAQ-Eintrag
- Wechsel ohne Vorankündigung
- Nur AVV-rechtliche Weiterverpflichtung (Art. 28 Abs. 4 DS-GVO) ohne berufsrechtliche Komponente
- Keine berufsrechtliche Belehrung der Subunternehmer

## Sonderkonstellation Microsoft Azure OpenAI

Der häufige Aufbau "Frontend-Anbieter — Azure-Mietservice für OpenAI-Modelle" ist berufsrechtlich besonders zu prüfen:

- Azure ist Hoster und Subunternehmer
- OpenAI als Modellanbieter ist ggf. weiterer Subunternehmer
- US-Konzern-Mutter aller Beteiligten — Cloud Act greift (siehe `cloud-act-und-drittstaat-pruefen`)
- Datenfluss Azure → OpenAI muss explizit beleuchtet werden

## Output

Tabellarische Bewertung. Lücken fließen in den Rückfragebrief ein (etwa: "Bitte legen Sie die aktuelle, abschließende Subunternehmerliste mit Sitz und Funktion vor").
