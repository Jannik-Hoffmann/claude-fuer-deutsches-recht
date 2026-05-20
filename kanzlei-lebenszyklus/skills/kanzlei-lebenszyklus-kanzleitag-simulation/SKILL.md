---
name: kanzlei-lebenszyklus-kanzleitag-simulation
description: "Führt im Simulationsmodus durch einen achtstündigen Kanzleitag mit Mandatsannahme GwG KYC Postlauf beA E-Mail Messenger Schreib-Canvas Fristen Zeitnarrativen Rechnung UStVA Eingangsrechnungen und Tagesabschluss."
---

# Kanzleitag-Simulation

## Zweck

Dieser Skill führt durch einen realistisch wirkenden Kanzleitag, ohne echte Systeme zu benötigen. Er eignet sich für Training, Demo, Testakte und Onboarding junger Anwältinnen und Anwälte.

## Startfragen

1. Echtzeit oder beschleunigt?
2. Welche Integrationen sind echt angeschlossen?
3. Welche Integrationen sollen simuliert werden?
4. Welche Akten sollen vorkommen?
5. Soll der freundliche Copilot aktiv Hinweise geben?
6. Soll nach jeder Station angehalten oder automatisch weitergeführt werden?

## Acht-Stunden-Ablauf

```text
09:00 Tagesstart, offene Fristen, Kalender, Integrationen
10:00 Intake aus E-Mail, Messenger, Fax oder Screenshot
11:00 Postlauf mit beA-Journal, EB-Prüfung, ZIP-Archiv
12:00 Schreib-Canvas für Schriftsatz oder Mandantenbrief
13:00 Zeitnarrative und kurze Pause
14:00 Neue Mandatsanfrage: Konfliktcheck, GwG, KYC, PEP, Kontoblatt, Vorschuss
15:00 Eingangsrechnungen, Betriebsausgaben, UStVA-Vorbereitung, ELSTER-Fallback
16:00 HR, Urlaub, Krankheit, Kanzleikalender und Payroll-Vorbereitung
17:00 Rechnung, E-Rechnung oder Mandatsvereinbarung vorbereiten
17:30 Versandcheck, beA/Fax/E-Mail simulieren oder echt vorbereiten
18:00 Tagesabschluss, Fristen, offene Fragen, Zeit, Rechnung und Personal
```

## Tempo

Im beschleunigten Modus kann eine Stunde als fünf bis zehn Minuten simuliert werden. Vor risikoreichen Handlungen immer anhalten:

- Fristübernahme.
- EB-Abgabe.
- beA-Versand.
- Rechnung finalisieren.
- Mandat annehmen.
- Ausweisdokumente auslesen oder ablegen.
- Verdachtsmeldung oder Unstimmigkeitsmeldung vorbereiten.
- E-Rechnung validieren.
- UStVA übermitteln.
- Lohnabrechnung, SV-Meldung oder Lohnsteuer-Anmeldung übermitteln.
- Krankheitsdaten oder Personalakte ausgeben.

Wenn ELSTER oder Buchhaltung nicht angeschlossen ist, an `kanzlei-lebenszyklus-ustva-simulation` übergeben und zwischen ELSTER-Online-Simulation, manuellem Eingabebogen, XML-Upload-Prüfung und Steuerberater-Paket wählen lassen.

Wenn Kalender, HR- oder Lohnsoftware nicht angeschlossen ist, an `kanzlei-lebenszyklus-kanzleikalender`, `kanzlei-lebenszyklus-hr-personal`, `kanzlei-lebenszyklus-abwesenheiten-urlaub` und `kanzlei-lebenszyklus-lohn-sv` übergeben und ausdrücklich als Simulation markieren.

Wenn Mandatsannahme oder GwG nicht echt angebunden ist, an `kanzlei-lebenszyklus-mandatsannahme-gwg` übergeben und Ausweis-, Register-, PEP-, Mittelherkunfts- und Kontoblattprüfungen als Simulation markieren.

## Ausgabe

`assets/templates/kanzleitag-simulation.md` verwenden.
