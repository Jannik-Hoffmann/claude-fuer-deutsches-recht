---
name: kanzlei-lebenszyklus-rechnung
description: "Bereitet Kanzleirechnungen Vorschüsse RVG- und Stundenhonorare vor. Sammelt Timesheet Narrative Auslagen Umsatzsteuer Zahlungen Rechtsschutz Pflichtangaben GoBD-Protokoll und übergibt bei Bedarf an XRechnung oder ZUGFeRD."
---

# Rechnungsvorbereitung und Abschluss

## Zweck

Dieser Skill sammelt abrechnungsreife Informationen und erzeugt einen Rechnungsentwurf, Vorschussvorschlag oder eine Übergabe an den E-Rechnungs-Skill. Er ist die fachliche Rechnungsakte, nicht das Buchhaltungssystem.

## Datenquellen

- Zeit- und Narrative-Ledger.
- Mandatsvereinbarung.
- RVG-Hinweise.
- Auslagen.
- Gerichtskosten.
- Vorschüsse.
- Zahlungen.
- Rechtsschutzdeckung.
- Mandatsabschluss oder Zwischenrechnung.
- beA- und Postlauf-Journal für Versand- und Zustellaufwand.
- Fristen- und Action-Register für fristbezogene Tätigkeiten.
- Kosten- und Fremdgeldvermerke.
- Eingangsrechnungen- und UStVA-Register, soweit Rechnungsausgang und Umsatzsteuer abgestimmt werden sollen.

## Ablauf

1. Akte wählen.
2. Rechnungstyp bestimmen: Vorschuss, Zwischenrechnung, Schlussrechnung, Korrektur, Storno, Gutschrift.
3. Rechnungsempfänger und Kostenschuldner prüfen.
4. Honorargrundlage feststellen: RVG, Stundenhonorar, Pauschale, Vorschuss, Rechtsschutz.
5. Leistungszeitraum und Leistungsbeschreibung bestimmen.
6. Narrative und Zeiten aus `kanzlei-lebenszyklus-zeitnarrative` übernehmen.
7. RVG-Gebühren, Streitwert, Gebührentatbestände und Anrechnungen als Prüfpunkte erfassen.
8. Auslagen, Gerichtskosten, Dokumentenpauschalen, Reisekosten und Fremdgeld getrennt prüfen.
9. Umsatzsteuer, Steuerbefreiung, Reverse Charge oder Kleinunternehmer nur nach konkreter Grundlage markieren.
10. Vorschüsse, Zahlungen und Rechtsschutzleistungen abziehen.
11. Summen netto, Steuer und brutto prüfen.
12. Pflichtangaben und GoBD-nahe Archivierung vorbereiten.
13. Formatbedarf klären: PDF, Papier, XRechnung, ZUGFeRD oder sonstiges.
14. Bei Umsatzsteuerrelevanz Übergabe an `kanzlei-lebenszyklus-ustva-buchhaltung` vormerken.
15. Nach Freigabe und Versand offenen Posten an `kanzlei-lebenszyklus-buchhaltung-konten` übergeben.
16. Rechnungsentwurf erzeugen.
17. Freigabe verlangen.

## Narrative-Übernahme

Aus dem Zeit- und Narrative-Ledger nicht blind alles abrechnen. Für jede Position prüfen:

- Akte und Mandat passen.
- Tätigkeit ist abrechenbar oder bewusst nicht abrechenbar.
- Narrative ist mandantenfähig, knapp und prüfbar.
- Interne Strategie, unnötige Geheimnisse und personenbezogene Drittinformationen sind entfernt.
- Zeit, Mindesttakt, Rundung und Bearbeiter sind nachvollziehbar.
- Bei Pauschale oder RVG wird die Tätigkeit als Nachweis oder Anlage geführt, nicht automatisch als Stundenposition.

## E-Rechnung und GoBD

Wenn der Empfänger Unternehmer oder öffentliche Stelle ist oder der Nutzer eine E-Rechnung verlangt, an `kanzlei-lebenszyklus-erechnung` übergeben.

Immer vorbereiten:

- `assets/templates/rechnungsdatenblatt.md`.
- `assets/templates/gobd-rechnungsprotokoll.md`.

Bei E-Rechnung zusätzlich:

- `assets/templates/erechnung-datenblatt.md`.
- Formatentscheidung XRechnung oder ZUGFeRD.
- Validierungsvermerk.
- Archivierungsvermerk für strukturierte XML-Daten.

## Grenzen

Keine verbindliche RVG-Gebührenberechnung, steuerliche Einordnung, GoBD-Prüfung oder E-Rechnungsvalidierung ohne Prüfung durch verantwortliche Person oder Fachsystem. Bei Streitwert, Gegenstandswert, mehreren Auftraggebern, Vergleich, Terminsgebühr, Anrechnung, Fremdgeld, Umsatzsteuer, Rechtsschutz oder Korrekturrechnung immer Unsicherheit markieren.

## Ausgabe

- Rechnungsdatenblatt.
- Narrative-Liste.
- GoBD-Prüfprotokoll.
- E-Rechnungsdatenblatt, wenn erforderlich.
- Prüfhinweise und Validierungsstatus.
- Entwurf Rechnungstext.
- Offene Punkte.
- Offene-Posten-Übergabe nach Freigabe.
