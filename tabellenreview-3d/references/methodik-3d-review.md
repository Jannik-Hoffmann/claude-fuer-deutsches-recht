# Methodik des dreidimensionalen Tabellenreviews

## Bild

Stellen Sie sich eine Excel-Mappe vor. Auf jedem Tabellenblatt eine Tabelle: Zeilen sind Dokumente, Spalten sind Fragen, Zellen sind Antworten mit woertlichem Zitat und Fundstelle. Bisher: eine Mappe pro Pruefdimension. Jetzt: eine Mappe mit mehreren Tabellenblaettern uebereinander, jedes Blatt ist eine andere Perspektive auf denselben Dokumentenstapel.

Das ist der Würfel.

## Drei Achsen

### Achse 1: Spalten (Datenpunkte)

Die Fragen die für ALLE Dokumente identisch gestellt werden. Macht den Stapel vergleichbar. Beispiel: "Welche Kuendigungsfrist gilt?" — die gleiche Frage an 200 Vertraege. Spaltenprompt-Änderungen wirken über alle Dokumente.

### Achse 2: Zeilen (Dokumente)

Die einzelnen Dokumente plus deren optionale Sonderanweisungen (Zeilenprompts). Erlaubt Genauigkeit dort wo ein Dokument abweicht. Beispiel: "Anlage 7 fehlt — als Lücke markieren" bei genau einem Vertrag.

### Achse 3: Arbeitsblätter (Perspektiven)

Mehrere Pruefdimensionen über denselben Stapel. Beispiel: Recht / Steuer / Wirtschaft / Datenschutz uebereinander. Jede Perspektive hat eine Auswahl gemeinsamer Spalten plus eigener Zusatzspalten plus eigener Pruefer-Rolle.

## Warum drei Achsen?

Eine flache Tabelle (2D) zwingt einen Vertrag zur einen Antwort. Aber:
- Rechtlich kann eine Klausel wirksam sein
- Steuerlich kann sie eine Folge haben
- Wirtschaftlich kann sie ein Risiko sein
- Datenschutzrechtlich kann sie unzureichend sein

Alle vier Antworten sind richtig — aus unterschiedlichen Perspektiven. Die dritte Achse macht das sichtbar ohne Verwirrung.

## Kreuzblatt-Konsistenz

Wenn das Recht-Blatt sagt "Vertragsdatum 2021-03-15" und das Wirtschaft-Blatt sagt "Vertragsdatum 2021-03-25" — das ist ein Fehler, nicht eine Perspektive. Skill `kreuzblatt-konsistenzpruefung` findet beides: echte Widersprueche (Datenfehler) und legitime perspektivische Abweichungen.

## Belegkette

Jede Zelle ist ein Hinweis kein Befund. Die Belegkette macht jeden Hinweis rueckverfolgbar:

```
Zelle = Antwort + Zitat + Fundstelle (Datei-Hash + Seite + Absatz) + Prompt-Version
```

Ohne Belegkette ist eine Zelle wertlos. Mit Belegkette ist sie pruefbar.

## Pruefer-Flag

Der Würfel sagt nicht "ich weiss es nicht" — er sagt "ich vermute X mit Konfidenz Y und Pruefer schaut bitte hin". Untermarkierung verbirgt Probleme. Uebermarkierung kostet den Pruefer zehn Sekunden pro Flag und schafft den noetigen Vertrauensvorschuss.

## Audit-Trail und Reproduzierbarkeit

Jeder Reviewlauf, jede Prompt-Änderung, jede Pruefer-Abnahme wird unveraenderlich protokolliert. Wer in zwei Jahren fragt "wie kam der Würfel zustande?" bekommt eine Antwort, nicht ein Schulterzucken.

## Verhaeltnis zum 2D-Skill

Der 2D-Skill `gesellschaftsrecht/tabellenpruefung` ist die Grundlage: Spaltenprompts + Zeilenprompts. Das 3D-Plugin erweitert ihn um die dritte Achse (Arbeitsblätter) und die ganze Pipeline (Cache, Audit-Trail, Belegkette, Pruefer-Paket).

## Grenzen

Der Würfel ist Vorbereitung. Die Mandatsabnahme ist Rechtsdienstleistung (RDG Paragraph 2) und darf nur durch einen zugelassenen Rechtsanwalt erfolgen.
