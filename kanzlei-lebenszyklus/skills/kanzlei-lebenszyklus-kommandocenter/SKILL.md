---
name: kanzlei-lebenszyklus-kommandocenter
description: "Schnellstart und Command Center für Das volle Kanzlei-Workflow-Plugin. Erkennt aus einem Satz den passenden Kanzlei-Workflow, routet zu Mandatsannahme GwG Klage Replik Vertrag Rechtsprechung beA Fristen Rechnung Buchhaltung HR UStVA oder Simulation, stellt nur die nötigsten Rückfragen und erzeugt eine Freigabeampel."
---

# Kommandocenter

## Zweck

Dieser Skill ist die schnelle Oberfläche des Plugins. Er verhindert, dass Nutzer erst wissen müssen, welcher Spezialskill passt. Aus einem Satz, einer Datei oder einem chaotischen Eingang entsteht eine klare Arbeitskarte mit nächstem Schritt, passenden Skills und Freigabeampel.

## Grundregel

Erst Tempo, dann Tiefe:

1. Ziel erkennen.
2. Risiko erkennen.
3. maximal drei Rückfragen stellen.
4. sofort eine Arbeitskarte erzeugen.
5. `kanzlei-lebenszyklus-look-and-feel` anwenden, wenn eine sichtbare Dashboard-, Status- oder Startausgabe entsteht.
6. an den passenden Spezialskill übergeben.

Nicht alle Checklisten auf einmal öffnen. Nur die Checkliste verwenden, die den nächsten Arbeitsschritt wirklich freischaltet.

## Schnellbefehle

| Nutzer sagt | Route |
| --- | --- |
| `Neue Sache` | Intake, Akte, Mandatsannahme/GwG, Aktenzeichen, Kontoblatt |
| `Mach Klage` | Schriftsatz-Turbo, Anlagen, Rechtsprechung, Qualitätsgate, Versand |
| `Mach Replik` | Replikmatrix, Anlagen, Rechtsprechung, Qualitätsgate, Versand |
| `Mach Vertrag` | Vertragsentwurf, Handelsregister, Datenschutz, Qualitätsgate |
| `Post machen` | Postlauf, beA-Journal, Fristen, EB, Aktenablage |
| `Rechnung machen` | Zeitnarrative, Rechnung, E-Rechnung, GoBD, offene Posten |
| `GwG prüfen` | Mandatsannahme/GwG, KYC, PEP, wirtschaftlich Berechtigte, Verdachtslogik |
| `Recherche machen` | Rechtsprechungsrecherche, Fundstellenregister, Verwertungsnotiz |
| `Kanzleitag simulieren` | Integrationen, Simulation, Kalender, Postlauf, Mandatsannahme, Output |
| `Was ist offen?` | Fristen, Action-Items, Rechnungen, GwG-Reminder, Post, HR, UStVA |

## Freigabeampel

Immer eine Ampel ausgeben:

- `GRÜN`: Weiterarbeiten möglich. Keine bekannte Stoppschwelle.
- `GELB`: Nutzbarer Entwurf, aber offene Punkte.
- `ROT`: Nicht versenden, nicht annehmen, nicht buchen oder nicht melden, bevor ein Mensch freigibt.

Typische rote Schwellen:

- Frist unklar.
- beA-Versand oder EB ohne Einzelbestätigung.
- Mandatsannahme ohne Konfliktcheck oder GwG-Status.
- Verdachtsfall, PEP-/Hochrisiko- oder Mittelherkunftsproblem ungeklärt.
- Rechnung ohne Freigabe oder E-Rechnungsvalidierung.
- Rechtsprechung nicht verifiziert.
- Handelsregister, Partei oder Vertretung ungeprüft.

## Arbeitskarte

Immer mit dieser Struktur starten:

```markdown
# Das volle Kanzlei-Workflow-Plugin

## Kommandocenter

| Akte | Ampel | Frist | Nächste Aktion |
| --- | --- | --- | --- |
|  |  |  |  |

## Jetzt

1.
2.
3.
```

## Anfängerfreundlichkeit

- Fachworte kurz übersetzen.
- Nicht mit 20 Fragen beginnen.
- Fehlendes als `TODO` markieren.
- Unsichere Nutzer mit einem konkreten Vorschlag führen.
- Bei Profis knapper werden und direkt an die Spezialskills übergeben.

## Übergabe

- Neue Sache oder Dokumenteneingang: `kanzlei-lebenszyklus-intake`, danach `kanzlei-lebenszyklus-akte` und bei Bedarf `kanzlei-lebenszyklus-mandatsannahme-gwg`.
- Klage/Replik/Antrag: `kanzlei-lebenszyklus-schriftsatz-turbo`, `kanzlei-lebenszyklus-rechtsprechungsrecherche`, `kanzlei-lebenszyklus-qualitaetsgate-hardening`.
- Vertrag: `kanzlei-lebenszyklus-vertragsentwurf`, `kanzlei-lebenszyklus-handelsregisterabruf`, `kanzlei-lebenszyklus-qualitaetsgate-hardening`.
- beA/Post: `kanzlei-lebenszyklus-postlauf`, `kanzlei-lebenszyklus-bea-journal`, `kanzlei-lebenszyklus-fristen-monitor`.
- Rechnung/Buchhaltung: `kanzlei-lebenszyklus-zeitnarrative`, `kanzlei-lebenszyklus-rechnung`, `kanzlei-lebenszyklus-erechnung`, `kanzlei-lebenszyklus-buchhaltung-konten`.
- Kanzleibetrieb: `kanzlei-lebenszyklus-kanzleikalender`, `kanzlei-lebenszyklus-automationen`, HR-/Payroll-Skills.

## Ausgabe

- `assets/templates/workflow-kommandocenter.md`
- `assets/templates/workflow-schnellstartkarte.md`
- `assets/templates/workflow-freigabeampel.md`
- optional `assets/templates/workflow-naechste-beste-aktion.md`
- für hochwertige Cowork-Ausgaben zusätzlich `assets/templates/cowork-dashboard.md`, `assets/templates/cowork-statuskarte.md` und `assets/templates/cowork-freigabekarte.md`.
