# Testakte Das volle Kanzlei-Workflow-Plugin

Fiktiver Kanzlei-Alltag der **Kanzlei Lindenstraße Rechtsanwältin Jana Reuter**, Berlin. Die Akte ist zum Durchspielen von **Das volle Kanzlei-Workflow-Plugin** (`kanzlei-lebenszyklus`) gebaut: edles Claude-Cowork-Dashboard, Nachtblau/Silber/Orange-Look, Kommandocenter, freundlicher Copilot, Integrationscheck, Simulationsmodus, Mandatsannahme/GwG, KYC, PEP, Kontoblatt, Schreib-Canvas, Klage-/Replik-Turbo, Rechtsprechungsrecherche, Vertragsentwurf, Handelsregisterabruf, Qualitätsgate, beA-Journal, EB, Fristen, Kanzleikalender, HR, Urlaub, Krankheit, Payroll, Zeitnarrative, Rechnung, Geschäftskonto, Bankmatching, E-Rechnung, UStVA und Tagesabschluss.

## Szenario

Jana Reuter ist junge Einzelanwältin. Word und ein lokaler Aktenordner sind vorhanden. Outlook, beA, Fax, WhatsApp, Fristenkalender, Buchhaltung, Geschäftskonto, ELSTER, HR-Software und Lohnsoftware sind in dieser Testakte **nicht echt angeschlossen**. Das Plugin soll deshalb fragen, ob es beim Anschluss helfen oder die Vorgänge simulieren soll.

## Startprompt

```text
Bitte starte Das volle Kanzlei-Workflow-Plugin mit dieser Testakte. Nutze zuerst das edle Cowork-Kommandocenter, zeige eine Statuskarte mit Ampel, prüfe die Integrationen und führe mich im Simulationsmodus durch einen beschleunigten achtstündigen Kanzleitag.
```

## Erwarteter Ablauf

1. Kommandocenter startet mit Ziel, Ampel und nächsten drei Schritten.
2. Integrationsstatus prüfen und Simulation anbieten.
3. 09:00 Tagesstart mit Fristen und offenen Aufgaben.
4. 10:00 E-Mail, WhatsApp-Screenshot und Fax-Verfügung in Intake aufnehmen.
5. 11:00 beA-Journal simulieren, eingegangene ZIP-Archive entpacken, EB-Workflow anbieten.
6. 12:00 Schreib-Canvas öffnen und unsubstantiierten Schriftsatz verbessern.
7. 13:00 Zeitnarrative nachziehen.
8. 14:00 Eingangsrechnungen sammeln und UStVA-Vorbereitungsblatt erstellen.
9. 15:00 Kanzleikalender, Urlaubsantrag, Krankmeldung, Payroll und Jour fixe prüfen.
10. 16:00 Geschäftskonto-Simulation, offene Posten und Zahlungseingang-Matching durchführen.
11. 17:00 Neue Mandatsanfrage mit GwG-/KYC-Prüfung, PEP-Rückfragen, Aktenzeichen, Kontoblatt und Mandatsvereinbarung simulieren.
12. 17:30 Output-Turbo starten: Klage oder Replik samt Anlagenverzeichnis, Rechtsprechungsrecherche, Handelsregisterabruf und Qualitätsgate erzeugen.
13. 18:00 beA- oder E-Mail-Versandcheck simulieren.
14. 18:15 Vertragsentwurf für ein Kanzlei-SaaS samt Register- und Risikoprüfung erstellen.
15. 18:30 Tagesabschluss mit Fristen, offenen Punkten, Zeiten, Personal, Buchhaltung und Rechnungsstatus.

## Enthaltene Testdaten

- Integrationsmatrix mit fehlenden Anschlüssen.
- Kommandocenter-Schnellstart, Cowork-Design-Erwartung und Offenliste für nächste beste Aktion.
- beA-Journal-Screenshot als Platzhalter.
- Eingangs- und Versand-ZIP-Platzhalter.
- E-Mail, WhatsApp-Screenshot, Fax-Verfügung.
- Schreib-Canvas mit juristisch schwachem Rohtext.
- Zeitnarrative-Ledger.
- Ausgangsrechnung mit XRechnung-XML-Platzhalter und ZUGFeRD-PDF/A-3-Platzhalter.
- Eingangsrechnungen für Miete, Strom, Cloud, beA-Token, E-Akte, KI-Anbieter und Fachliteratur.
- UStVA-Vorbereitungsblatt für Mai 2026 mit ELSTER-Ausfall-Szenario, manueller Eingabeliste, unvalidiertem XML-Platzhalter und Steuerberater-Paket.
- Personalstamm, Urlaubsantrag, Krankmeldung, Payroll-Vorbereitung, Kanzleikalender und Jour-fixe-Agenda.
- Geschäftskonto-CSV, offene Posten, Zahlungseingang-Matching, Bankanbindungs-Simulation und DATEV-ähnliche Übergabe.
- Output-Turbo-Testdaten für Klage, Replik, Anlagenverzeichnis, Vertragsentwurf, Handelsregisterabruf und Qualitätsgate.
- Rechtsprechungs-Testdaten für Suchplan, Fundstellenregister, OpenJur/dejure-Ergänzung und simulierte Aktenablage.
- Mandatsannahme-/GwG-Testdaten mit Erstkontakt, Ausweisplatzhalter, Handelsregisterplatzhalter, PEP-/Mittelherkunftsfragen, Kontoblatt und Mandatsvereinbarungsbausteinen.

Alle Daten sind frei erfunden.
