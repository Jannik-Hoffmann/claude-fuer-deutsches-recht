---
name: kanzlei-lebenszyklus-look-and-feel
description: "Gestaltet Ausgaben für Das volle Kanzlei-Workflow-Plugin innerhalb der Claude-Cowork-Grenzen hochwertig, ruhig und edel. Nutzt Markdown-Dashboards, Statuskarten, Freigabeampeln, bläulich-silberne Grundtöne und warmen Orange-Akzent ohne CSS-Abhängigkeit."
---

# Look and Feel

## Zweck

Dieser Skill sorgt dafür, dass die Kanzlei-Workflows in Claude Cowork nicht wie lose Checklisten wirken, sondern wie ein ruhiges, hochwertiges Kanzlei-Cockpit. Er nutzt nur robuste Markdown-Mittel: klare Abschnitte, kurze Karten, Tabellen, Ampelstatus, Trennlinien und konsistente Benennungen.

## Designprinzipien

- Ruhig vor laut.
- Wenige starke Entscheidungen statt vieler Hinweise.
- Maximal drei nächste Schritte.
- Status immer sichtbar.
- Aktenname, Frist, Risiko und nächste Aktion oben.
- Keine dekorativen Symbole, keine unnötigen Trennzeichen, keine langen Textwände.
- Fachlich präzise, optisch luftig.

## Farb- und Tonwelt

Da Cowork-Markdown keine verlässliche freie CSS-Färbung garantiert, Farben als wiederkehrende Status- und Abschnittsbegriffe führen:

- `Nachtblau`: Kernarbeit, Akte, gerichtliche Arbeit, Kommandocenter.
- `Silber`: neutrale Struktur, Ablage, Register, Protokoll, Zusammenfassung.
- `Orange`: Aufmerksamkeit, Frist, Freigabe, offene Entscheidung.
- `Rot`: Stopper.
- `Grün`: freigegeben oder arbeitsfähig.

Nicht versuchen, HTML/CSS zu erzwingen, wenn Cowork es nicht sicher rendert.

## Standardlayout

Jede zentrale Ausgabe soll so beginnen:

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

Danach erst Details.

## Kartenlogik

Für Kanzlei-Cowork-Ausgaben drei Kartentypen verwenden:

- `Statuskarte`: Akte, Ampel, Frist, Verantwortlicher.
- `Arbeitskarte`: Ziel, nächster Schritt, benötigte Unterlagen.
- `Freigabekarte`: was darf passieren, was darf noch nicht passieren.

## Stilregeln

- Überschriften kurz halten.
- Tabellen nur für Vergleich, Status oder Register nutzen.
- Keine verschachtelten Listen.
- Kein Marketingtext im Arbeitsmodus.
- Keine Scheinpräzision. Unbekanntes als `offen` markieren.
- Bei Risiken klar sein: `Nicht versenden`, `Nicht annehmen`, `Nicht buchen`, `Nicht melden`.

## Übergabe

Dieser Skill ergänzt besonders:

- `kanzlei-lebenszyklus-kommandocenter`
- `kanzlei-lebenszyklus-freundlicher-copilot`
- `kanzlei-lebenszyklus-qualitaetsgate-hardening`
- `kanzlei-lebenszyklus-kanzleitag-simulation`

## Ausgabe

- `assets/templates/cowork-designsystem.md`
- `assets/templates/cowork-dashboard.md`
- `assets/templates/cowork-statuskarte.md`
- `assets/templates/cowork-freigabekarte.md`
