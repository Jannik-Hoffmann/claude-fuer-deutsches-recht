---
name: kanzlei-lebenszyklus-abwesenheiten-urlaub
description: "Verwaltet Urlaub Krankmeldungen Fehlzeiten Vertretung Kalenderabstimmung Resturlaub und Teamabdeckung. Erstellt Abwesenheitsregister und fragt freundlich nach Nachweisen Vertretung Fristen und Kanzleikalender-Konflikten."
---

# Abwesenheiten, Urlaub und Krankheit

## Zweck

Dieser Skill verwaltet Urlaubsanträge, Krankheit, Fehlzeiten, Vertretungen und Resturlaub. Er achtet darauf, dass Fristen, beA, Postlauf und Mandantenkommunikation abgedeckt bleiben.

## Abwesenheitsarten

- Erholungsurlaub.
- Krankheit mit Arbeitsunfähigkeitsmeldung.
- Kind krank.
- Fortbildung.
- Homeoffice.
- Überstundenausgleich.
- Sonderurlaub.
- Unbezahlter Urlaub.
- Elternzeit, Mutterschutz, Pflegezeit als Stoppschild.

## Ablauf Urlaubsantrag

1. Person und Zeitraum erfassen.
2. Resturlaub und Überschneidungen prüfen.
3. Kalender, Fristen, Gerichtstermine, Postlauf und beA-Abdeckung prüfen.
4. Vertretung vorschlagen.
5. Entscheidung: genehmigen, ablehnen, Rückfrage, alternativer Zeitraum.
6. Kanzleikalender und Abwesenheitsregister aktualisieren.

## Ablauf Krankmeldung

1. Krankmeldung aufnehmen.
2. Zeitraum, voraussichtliche Rückkehr und Nachweisstatus erfassen.
3. Vertretung für Fristen, Termine, Telefon, beA und Postlauf bestimmen.
4. Lohn/SV-Hinweis an `kanzlei-lebenszyklus-lohn-sv` geben.
5. Datenschutz beachten: Diagnose nicht erfassen, wenn nicht erforderlich.

## Ausgabe

`assets/templates/abwesenheiten-register.md` verwenden.
