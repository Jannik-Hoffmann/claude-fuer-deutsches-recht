---
name: kanzlei-lebenszyklus-zeitnarrative
description: "Erzeugt stündliche oder manuelle Zeiterfassungsabfragen mit abrechenbaren Narrativen. Erfasst Akte Dauer Takt Bearbeiter Tätigkeit Quelle Honorargrundlage Abrechenbarkeit Rechnungsfähigkeit und Datenschutzreduktion."
---

# Zeitnarrative und Timesheet

## Zweck

Dieser Skill macht aus Arbeitsschritten abrechenbare oder interne Zeitnarrative. Er fragt nach, welcher Akte die Tätigkeit zugeordnet werden soll, und erzeugt klare Zeiteinträge, die später in Rechnung, E-Rechnung, Prüfprotokoll oder interne Controlling-Auswertung übernommen werden können.

## Standardfrage

> Soll ich für die letzte Stunde einen Zeiteintrag vorbereiten? Ich habe folgende mögliche Tätigkeiten erkannt: ... Welcher Akte soll ich das zuordnen?

## Ablauf

1. Beobachtete oder geschilderte Tätigkeit zusammenfassen.
2. Aktenzuordnung vorschlagen und Unsicherheit markieren.
3. Bearbeiter, Rolle und Verantwortlichen erfassen.
4. Start, Ende, Dauer, Mindesttakt und Rundung erfragen oder vorschlagen.
5. Tätigkeit klassifizieren: Intake, Aktenprüfung, Frist, Recherche, Schriftsatz, Telefonat, Mandantenkontakt, Gegnerkontakt, Gerichtskontakt, beA, Rechnung, intern.
6. Abrechenbarkeit markieren: abrechenbar, nicht abrechenbar, pro bono, intern, Pauschale enthalten, RVG-Nachweis.
7. Honorargrundlage: RVG, Stundenhonorar, Pauschale, Vorschuss, Rechtsschutz, Kulanz.
8. Rechnungsfähigkeit prüfen: mandantenfähig, verständlich, quellenbasiert, ohne unnötige Geheimnisse.
9. Narrative formulieren: knapp, mandatsbezogen, prüfbar.
10. Freigabe abfragen.
11. Übergabe an `kanzlei-lebenszyklus-rechnung` vormerken, wenn abrechnungsreif.

## Narrative-Stil

Gut:

- „Prüfung beA-Eingang und Fristnotierung; Entwurf Rückfrage an Mandant.“
- „Analyse Klageerwiderung und Strukturierung der Gegenargumente.“
- „Telefonat mit Mandant zur Sachverhaltsergänzung und Abstimmung der nächsten Schritte.“
- „Entwurf und Überarbeitung Schriftsatzantwort einschließlich Anlagenabgleich.“

Nicht gut:

- interne Gedankengänge,
- überflüssige Geheimnisse,
- unsichere Spekulationen,
- personenbezogene Details ohne Abrechnungsnutzen.

## Granularität

Für Rechnungen lieber mehrere saubere Einträge als einen Sammelblock erzeugen:

- beA-Eingang prüfen.
- Frist und Vorfrist notieren.
- Anlagen sichten.
- Rechtsfrage prüfen.
- Mandantenrückfrage entwerfen.
- Schriftsatz entwerfen.
- Schriftsatz finalisieren.
- Versand vorbereiten.

Nicht künstlich zersplittern, wenn ein zusammenhängender Arbeitsblock fachlich besser passt. Ziel ist prüfbare, verständliche Abrechnung.

## Datenschutzreduktion

Narrative sollen genug Inhalt für Rechnung und Prüfung enthalten, aber keine unnötigen Mandatsgeheimnisse offenlegen. Namen Dritter, Gesundheitsdaten, Bankdaten, Kinder, Strafvorwürfe und interne Prozessstrategie nur aufnehmen, wenn sie für die Abrechnung wirklich erforderlich sind.

## Rechnungsschnittstelle

Jeder freigegebene abrechenbare Eintrag bekommt:

- Rechnungsstatus: offen, gesperrt, abgerechnet, nicht abrechenbar.
- Rechnungsposition oder RVG-Nachweis.
- Leistungszeitraum.
- Bearbeiter.
- Nettofähige Beschreibung.
- Hinweis, ob die Narrative in eine Anlage zur E-Rechnung übernommen werden darf.

## Ausgabe

`assets/templates/zeit-narrative-ledger.md` verwenden.

## Automationshinweis

Wenn Automationen verfügbar sind, nach Zustimmung stündliche Erinnerung vorschlagen. Keine stille Dauerüberwachung.
