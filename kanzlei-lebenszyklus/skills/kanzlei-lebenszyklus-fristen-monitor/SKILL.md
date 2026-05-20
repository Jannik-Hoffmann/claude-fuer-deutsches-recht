---
name: kanzlei-lebenszyklus-fristen-monitor
description: "Scannt Akteninhalt auf Fristen Action-Items Wiedervorlagen Empfangsbekenntnisse Zustellungen und Antwortbedarf. Erstellt ein Fristen- und Action-Register mit Vorfrist Verantwortlichem Quelle und Übertragungsvermerk. Betont immer die anwaltliche Fristenkontrolle."
---

# Fristen- und Action-Monitor

## Zweck

Dieser Skill prüft Eingänge und Aktenordner auf Handlungsbedarf. Er führt ein Fristen- und Action-Register, ersetzt aber keinen verbindlichen Kanzlei-Fristenkalender.

## Scanquellen

- Neue Eingänge aus Intake.
- Aktenordner.
- beA-Nachrichten.
- beA-Nachrichtenjournal, beA-ZIP-Archive, EB-Nachweise und beA-Screenshots.
- gerichtliche Verfügungen.
- Behördenbescheide.
- Mandantenmails und Messenger.
- interne Notizen.

## Ablauf

1. **Quelle erfassen**: Dokument, Eingangstag, Zustellart, Akte.
2. **Fristtyp bestimmen**: gesetzliche Frist, richterliche Frist, vertragliche Frist, Wiedervorlage, interne Aufgabe.
3. **Fristbeginn prüfen**: Zustellung, Bekanntgabe, Zugang, Empfangsbekenntnis, Fristsetzung.
4. **Fristende vorschlagen**: nur als Vorschlag, mit Unsicherheitsmarkierung.
5. **Vorfrist setzen**: Standard nach Kanzleiprofil.
6. **Action-Item ableiten**: Antwort, Schriftsatz, Rückfrage, Zahlung, Termin, Recherche.
7. **EB prüfen**: bei beA-Eingang klären, ob ein elektronisches Empfangsbekenntnis verlangt wird, ob es vorbereitet werden soll und welche Fristfolge droht.
8. **Übertragung verlangen**: verbindlicher Kanzleikalender plus Vier-Augen-Kontrolle.

## Ausgabe

`assets/templates/fristen-und-action-register.md` verwenden.

Jede Frist bekommt:

- Quelle.
- Berechnungsannahme.
- Unsicherheiten.
- Verantwortlichen.
- Übertragungsvermerk.
- beA-ZIP, Journal-Screenshot oder EB-Nachweis, wenn der Auslöser aus beA kommt.

## Blockadevermeidung

Wenn Fristberechnung unsicher ist, nicht stehen bleiben:

1. konservativ früheste mögliche Frist markieren,
2. Rückfrage formulieren,
3. sofortige manuelle Prüfung verlangen.
