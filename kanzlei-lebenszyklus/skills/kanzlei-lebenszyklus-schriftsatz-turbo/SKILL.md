---
name: kanzlei-lebenszyklus-schriftsatz-turbo
description: "Erstellt schnell Klage Replik Antrag Klageerwiderung oder Schriftsatzantwort samt Anlagenlogik. Führt Anfänger durch Antrag Sachverhalt Beweise Recht Fristen Zuständigkeit beA-Versand und Qualitätsgate."
---

# Schriftsatz-Turbo: Klage, Replik, Antrag

## Zweck

Dieser Skill bringt aus ungeordneten Informationen schnell einen gerichtsfähigen Entwurf: Klage, Replik, Antrag, Klageerwiderung, Schriftsatzantwort, einstweiliger Antrag oder Mandantenentwurf. Er priorisiert Nutzbarkeit: erst Struktur und Pflichtteile, dann Verfeinerung.

## Schnellstart

Wenn wenig Zeit ist, fragen:

1. Wer ist Gericht oder Gegner?
2. Was soll das Gericht entscheiden?
3. Welche Frist läuft?
4. Welche Tatsachen sind sicher?
5. Welche Beweise oder Anlagen gibt es?
6. Was ist der dringendste Antrag?

Danach sofort ein Gerüst erzeugen, auch wenn Details offen sind.

## Produktionspfade

### Klage in 20 Minuten

1. Rubrum aus Akte, Registerabruf oder Mandatsblatt vorbereiten.
2. Antrag als Arbeitsfassung formulieren.
3. Anspruchsgrundlage wählen und hilfsweise Alternativen markieren.
4. Chronologie aus Quellen bauen.
5. Anlagen automatisch durchnummerieren.
6. Rechtsprechungsbedarf markieren und bei streitigen Rechtsfragen `kanzlei-lebenszyklus-rechtsprechungsrecherche` anstoßen.
7. Fehlende Beweise als TODO im Text markieren.
8. Qualitätsgate `Schnellcheck` ausführen.

### Replik in 20 Minuten

1. Klageerwiderung oder Gegenschreiben in einzelne Behauptungen zerlegen.
2. Jede Behauptung als `zugestanden`, `bestritten`, `unerheblich`, `neu`, `verspätet` oder `klärungsbedürftig` einordnen.
3. Substantiierte Antwort mit Quelle und Beweis bauen.
4. Rechtsprechung zu streitentscheidenden Rechtsfragen gezielt nachziehen und Fundstellen im Register ablegen.
5. Pauschales Bestreiten vermeiden.
6. Am Ende nur die wirklich nötigen Anträge wiederholen oder anpassen.

### Antrag oder Eilsache

1. Eilbedürftigkeit und Frist zuerst klären.
2. Glaubhaftmachungsmittel vorziehen.
3. Sachverhalt knapp, aber datiert darstellen.
4. Risiken der Zuständigkeit und des Rechtsschutzbedürfnisses markieren.

## Schriftsatz-Bausteine

1. Rubrum oder Beteiligte.
2. Aktenzeichen und Betreff.
3. Antrag.
4. Kurzüberblick.
5. Sachverhalt chronologisch mit Quellen.
6. Rechtliche Würdigung.
7. Beweisangebote oder Glaubhaftmachung.
8. Anlagenverzeichnis.
9. Frist- und Zustellhinweise.
10. Kosten- und Streitwertnotiz.
11. Signatur und Versandcheck.

## Replik-Modus

Bei Replik:

- Gegenseitigen Vortrag in Streitpunkte zerlegen.
- Zugestanden, bestritten, unerheblich, neu, verspätet markieren.
- Pro Streitpunkt Tatsachen, Beweis, Recht und Antrag ergänzen.
- Keine pauschalen Bestreitenssätze ohne Substanz stehen lassen.

## Anfängerführung

Wenn der Nutzer nur Stichworte gibt:

- Aus Stichworten eine Chronologie erzeugen.
- Fehlende Pflichtdaten als TODO in eckigen Klammern markieren.
- Nur die wichtigsten Rückfragen stellen: Gericht, Antrag, Frist.
- Einen Rohentwurf liefern, der sichtbar unfertige Stellen enthält, statt zu blockieren.

## Profi-Härtung

Wenn genug Material vorhanden ist:

- Anspruchsgrundlagen in Haupt- und Hilfsvortrag ordnen.
- Vortrag nach Darlegungs- und Beweislast strukturieren.
- Einwendungen der Gegenseite antizipieren.
- Rechtsprechungs- oder Zitierbedarf markieren.
- Amtliche Rechtsprechungsfundstellen über `kanzlei-lebenszyklus-rechtsprechungsrecherche` verifizieren.
- Anlagenreihenfolge so wählen, dass das Gericht die Chronologie ohne Suche nachvollziehen kann.

## Anlagenlogik

Jede Anlage braucht:

- Anlagenkürzel.
- Dateiname.
- Quelle.
- Beweisthema.
- Fundstelle im Schriftsatz.
- Datenschutzcheck.
- beA-PDF-Check.

Bei Anlagen immer prüfen:

- Ist die Anlage im Text wirklich verwendet?
- Ist das Beweisthema konkret genug?
- Sind personenbezogene Daten Dritter geschwärzt?
- Ist die Datei lesbar, nicht beschädigt und passend benannt?
- Gibt es Screenshots oder Videos, die in ein gerichtstaugliches Protokoll übersetzt werden müssen?

## Qualitätsgate

Vor Ausgabe immer `kanzlei-lebenszyklus-qualitaetsgate-hardening` ausführen. Vor Versand zusätzlich `kanzlei-lebenszyklus-output-versand`.

## Ausgabe

- `assets/templates/schriftsatz-turbo-geruest.md`.
- `assets/templates/rechtsprechungsfundstellen-register.md`, wenn Rechtsprechung gesucht wurde.
- `assets/templates/klage-replik-pruefmatrix.md`.
- `assets/templates/anlagenverzeichnis-schriftsatz.md`.
