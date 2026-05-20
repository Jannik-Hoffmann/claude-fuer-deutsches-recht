---
name: kanzlei-lebenszyklus-lohn-sv
description: "Bereitet Lohnabrechnung Sozialversicherungsbeiträge Lohnsteuer ELStAM Minijob Meldungen Bonus Gratifikation und Payroll-Übergabe vor. Rechnet nicht verbindlich ab und übermittelt nichts ohne Fachsystem und Freigabe."
---

# Lohn, Sozialversicherung und Payroll

## Zweck

Dieser Skill bereitet die monatliche Lohnabrechnung der Kanzlei vor. Er erstellt keine verbindliche Entgeltabrechnung und übermittelt keine Meldungen. Abrechnung, ELStAM, Lohnsteuer-Anmeldung, SV-Meldungen und Beitragsnachweise laufen über Lohnsoftware, Steuerkanzlei, ELSTER, SV-Meldeportal oder ein anderes zulässiges Fachsystem.

## Payroll-Daten

Für jeden Abrechnungsmonat erfassen:

- Mitarbeiter.
- Bruttogehalt oder Stundenlohn.
- Arbeitszeit, Überstunden, Zuschläge.
- Bonus, Gratifikation, Sonderzahlung.
- Sachbezüge.
- Fehlzeiten: Urlaub, Krankheit, Kind krank, unbezahlter Urlaub.
- Eintritt, Austritt, Unterbrechung.
- Steuerklasse oder ELStAM-Status.
- Krankenkasse, Rentenversicherung, Arbeitslosenversicherung, Pflegeversicherung.
- Minijob-Status, Personengruppenschlüssel und Beitragsgruppe, soweit relevant.
- Arbeitgeberanteile und Arbeitnehmeranteile als Fachsystem-Prüfpunkte.

## Monatlicher Ablauf

1. Personalstamm prüfen.
2. Arbeitszeiten und Fehlzeiten übernehmen.
3. Sonderzahlungen, Bonus und Gratifikation erfassen.
4. Veränderungen im Monat markieren.
5. Lohnsoftware- oder Steuerberater-Übergabe vorbereiten.
6. Lohnsteuer-Anmeldung und SV-Meldungen als Fachsystem-Aufgaben markieren.
7. Zahlungs- und Freigabeliste erzeugen.
8. Nach Abrechnung Entgeltabrechnung, Beitragsnachweis und Übermittlungsprotokolle ablegen.

## Stoppschilder

Immer anhalten bei:

- neuer Beschäftigung,
- Minijob-Grenze,
- Krankheit über Entgeltfortzahlung hinaus,
- Mutterschutz, Elternzeit, Pflegezeit,
- Bonus oder Gratifikation mit unklarer Zusage,
- Austritt, Kündigung, Freistellung,
- fehlender Steuer-ID, Krankenkasse oder Sozialversicherungsnummer,
- fehlender Betriebsnummer,
- nicht angeschlossener Lohnsoftware.

## Ausgabe

`assets/templates/lohnabrechnung-vorbereitung.md` verwenden.
