---
name: kanzlei-lebenszyklus-kaltstart
description: "Startet Das volle Kanzlei-Workflow-Plugin. Erfragt Kanzleiprofil Kommandocenter Aktenzeichen Eingangskanäle Integrationen Simulation Fristen HR Lohn Urlaub Kanzleikalender Honorar Rechnung UStVA und freundliche Menüführung."
---

# Das volle Kanzlei-Workflow-Plugin Kaltstart

## Zweck

Dieser Skill richtet das Plugin für eine Kanzlei, ein Dezernat oder einen Einzelanwalt ein. Ziel ist ein handhabbares Betriebsprofil, das spätere Workflows nicht blockiert.

## Pflichtfragen

Einmalig am Anfang fragen:

1. Kanzleityp: Einzelanwalt, Bürogemeinschaft, Sozietät, PartG, GmbH, Rechtsabteilung.
2. Rechtsgebiete und typische Mandatsarten.
3. Arbeitsmodus: Kommandocenter zuerst, Spezialskills direkt oder Simulation.
4. Aktenzeichen-Schema.
5. Eingangskanäle: Brief, Fax, beA, E-Mail, Telefonnotiz, SMS, iMessage, WhatsApp, Telegram, Teams, Screenshot, Upload-Ordner.
6. Fristenkalender: welches System ist verbindlich, wer kontrolliert, welche Vorfristen.
7. Honorar: RVG, Stundenhonorar, Pauschale, Vorschuss, Rechtsschutz.
8. Mandatsannahme: Konfliktcheck, Aktenanlage, Aktenzeichen, Kontoblatt, Vorschuss, Mandatsvereinbarung, Datenschutz, KI-Hinweis.
9. GwG: Kataloggeschäfte, Identifizierung, wirtschaftlich Berechtigte, PEP, Hochrisiko, Verdachtsfall, BRAK-Dokumentationsbögen, goAML-Status.
10. Output: Standardwege für Mandant, Gericht, Behörde, Gegner, Versicherung.
11. beA: nur vorbereiten, Versandcheck führen, Nachrichtenjournal sichern, ZIP-Archive herunterladen und entpacken oder technische Versandunterstützung möglich.
12. Zeiterfassung: Taktung, Mindestzeiteinheit, Bearbeiterrollen, Narrative-Stil, Rechnungsfreigabe.
13. Rechnung: Rechnungsnummernkreis, Pflichtangaben, GoBD-Ablage, E-Rechnungsformat, XRechnung, ZUGFeRD, Validierung, Korrekturrechnung.
14. Buchhaltung: Eingangsrechnungen, Betriebsausgaben, Vorsteuer, UStVA-Zeitraum, ELSTER oder Steuerkanzlei.
15. HR: Mitarbeiterstamm, Rollen, Arbeitsverträge, Urlaub, Krankheit, Fehlzeiten, Fortbildung, Zugänge.
16. Lohn/SV: Lohnsoftware oder Steuerkanzlei, ELStAM, Lohnsteuer-Anmeldung, SV-Meldungen, Minijobs, Bonus, Gratifikation.
17. Kanzleikalender: Fristen, Termine, Postlauf, beA, Urlaub, Krankheit, Payroll, UStVA, Jour fixe.
18. Integrationen: Word, Outlook, beA, Fax, Messenger, DMS, Fristenkalender, Buchhaltung, ELSTER, Kalender.
19. Simulationsmodus: fehlende Integrationen anschließen oder realistisch simulieren.
20. Output-Turbo: Klage, Replik, Antrag, Vertragsentwurf, Rechtsprechungsrecherche, Handelsregisterabruf, Anlagenverzeichnis.
21. Begleitmodus: knappe Hinweise, junge-Anwalt-Menüführung, Schreib-Canvas, Substanzcheck.
22. Datenschutz-Sicherheitsstufe: Testdaten, pseudonymisierte Mandate, echte Mandate.

## Sichere Defaults

Wenn der Nutzer nichts vorgibt:

- Aktenzeichen: `JAHR-RECHTSGEBIET-LFDNR`.
- Fristen: Hauptfrist plus Vorfrist; Übertragung in verbindlichen Kanzleikalender ausdrücklich bestätigen lassen.
- Versand: keine automatische Versendung, nur Entwurf und Versandcheck.
- beA: keine PINs oder Token im Chat; bei beA-Connect Journal, Screenshot, ZIP-Archiv, entpackte Nachricht und EB-Entscheidung protokollieren.
- Zeit: 6-Minuten-Takt mit kurzer, mandantenfähiger Narrative.
- Rechnung: Entwurf und GoBD-Protokoll vorbereiten, finale Rechnung erst nach Freigabe; E-Rechnung nur mit Validierungsvermerk.
- Integrationen: nichts heimlich verbinden; bei fehlendem Anschluss Simulationsmodus anbieten.
- Begleitmodus: freundlich, verzeihend, kurze hilfreiche Hinweise statt Daueralarm.
- Mandatsannahme/GwG: keine Annahme ohne dokumentierten Konfliktcheck, Annahmeentscheidung, GwG-Anwendbarkeitsprüfung und Kontoblatt. GwG-Verdacht nie still normalisieren.
- UStVA: nur vorbereiten und Übergabe an ELSTER, Buchhaltung oder Steuerkanzlei markieren.
- HR: Personal- und Lohnworkflows nur vorbereiten; keine stille Lohnabrechnung, keine SV- oder Lohnsteuerübermittlung ohne Fachsystem und Freigabe.
- Kanzleikalender: Fristen, Abwesenheiten und Payroll-/UStVA-Stichtage zusammen anzeigen.
- Kommandocenter: immer zuerst Ziel, Ampel und nächste drei Schritte ausgeben, wenn der Nutzer keinen Spezialskill nennt.

## Ausgabe

Ein `Kanzlei-Lebenszyklus-Profil` mit:

- Konventionen.
- Sicherheitsgattern.
- Ordnerstruktur.
- Integrationsstatus.
- Simulationsregeln.
- Begleitmodus-Regeln.
- Kommandocenter-Regeln.
- HR- und Payroll-Grundregeln.
- Mandatsannahme-, GwG- und Kontoblatt-Regeln.
- Kanzleikalender-Struktur.
- Qualitätsgate-Modus.
- Schriftsatz- und Vertrags-Turbo-Regeln.
- Rechtsprechungsrecherche- und Ablageregeln.
- Standard-Checklisten.
- Offenen Punkten, die noch nicht sicher entschieden sind.

## Übergabe

Danach an `kanzlei-lebenszyklus-kommandocenter`, `kanzlei-lebenszyklus-integrationen-simulation`, `kanzlei-lebenszyklus-freundlicher-copilot`, `kanzlei-lebenszyklus-kanzleikalender`, `kanzlei-lebenszyklus-intake` und bei neuer Akte an `kanzlei-lebenszyklus-mandatsannahme-gwg`, sobald ein Eingang oder eine neue Akte vorliegt.
