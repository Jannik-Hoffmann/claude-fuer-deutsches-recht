---
name: kanzlei-lebenszyklus-integrationen-simulation
description: "Prüft Kanzlei-Integrationen für E-Mail Outlook Word beA Fax Messenger Telefon DMS Kalender Buchhaltung und Ordner. Fragt freundlich nach Anschluss oder Simulationsmodus und führt Workflows auch ohne echte Verbindung weiter."
---

# Integrationen und Simulationsmodus

## Zweck

Dieser Skill klärt, welche Systeme wirklich angeschlossen sind. Wenn etwas fehlt, fragt er freundlich, ob der Nutzer es verbinden oder simulieren möchte. So bleibt der Workflow testbar, ohne echte beA-, Outlook-, Word-, Messenger-, Fax- oder Buchhaltungszugänge zu benötigen.

## Integrationsmatrix

Prüfen:

- Word oder Dokumenteneditor.
- Outlook oder E-Mail.
- beA.
- Fax.
- WhatsApp, iMessage, Telegram, Teams.
- Telefonnotizen.
- DMS oder E-Akte.
- Fristenkalender.
- Buchhaltung oder Steuerkanzlei.
- Geschäftskonto, Bankimport, CSV, CAMT, MT940 oder Kontoauszug.
- ELSTER oder UStVA-Fachsystem.
- HR-, Lohn- oder Personalsoftware.
- Kanzleikalender oder Teamkalender.
- Scanner, Screenshot-Ordner, Download-Ordner.

## Fragefolge

Für jeden relevanten Anschluss:

1. Ist er technisch verfügbar?
2. Darf das System darauf zugreifen?
3. Soll der Nutzer ihn jetzt einrichten?
4. Wenn nein: Soll der Vorgang simuliert werden?
5. Wo wird im Simulationsmodus protokolliert, dass es keine echte Übermittlung gab?

## Simulationsregeln

- Simulierte Vorgänge immer deutlich markieren.
- Keine echten Versand-, Abgabe- oder Zahlungserfolge behaupten.
- Für beA, EB, UStVA, Rechnung und Fristen immer `Simulation` oder `Echtlauf` ausweisen.
- Simulierte Screenshots, Nachrichten, ZIP-Archive, Protokolle und Eingangsrechnungen dürfen genutzt werden, müssen aber als Testdaten erkennbar bleiben.
- Bei ELSTER unterscheiden: manuelle Online-Eingabe, Fachsoftware/XML-Upload, Steuerberater-Paket oder reine Simulation. Kein beliebiges Dokument als echte UStVA-Abgabe behandeln.
- Bei HR und Payroll unterscheiden: Register/Simulation, Fachsoftware-Übergabe, Steuerkanzlei-Übergabe oder echte Lohnsoftware. Keine echte Lohn- oder SV-Meldung behaupten.
- Bei Geschäftskonto unterscheiden: echte Bankanbindung, Dateiimport, manueller Kontoauszug oder Simulation. Keine Bankzugangsdaten im Chat und keine Zahlungsaufträge ohne Freigabe.

## Beispiel

> beA ist nicht angeschlossen. Soll ich Sie beim Anschluss unterstützen oder den beA-Eingang für diese Testakte simulieren?

Wenn der Nutzer `simulieren` wählt:

1. Simulierten Eingang erzeugen.
2. Journal- und ZIP-Platzhalter verwenden.
3. Fristen und EB so behandeln, als müssten sie fachlich geprüft werden.
4. Klar ausgeben, dass kein echter Versand und keine echte EB-Abgabe erfolgt.

## Ausgabe

`assets/templates/integrationsstatus-und-simulation.md` verwenden.
