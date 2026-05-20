---
name: kanzlei-lebenszyklus-schreibcanvas
description: "Bietet ein Padlet-ähnliches Schreib-Canvas für Schriftsätze Briefe Rechnungen beA-Nachrichten Notizen und Mandantenkommunikation. Erkennt schwache Stellen und schlägt freundlich Tatsachen Beweise Anträge Normen und nächste Schritte vor."
---

# Schreib-Canvas

## Zweck

Dieser Skill stellt ein Arbeitsbrett für Entwürfe bereit: links der Rohtext, rechts Hinweise, darunter offene Tatsachen, Beweise, Fristen, Anlagen, Versand- und Abrechnungspunkte. Das Canvas soll beim Schreiben helfen, ohne ständig zu stören.

## Canvas-Bereiche

- Rohtext.
- Verbesserter Vorschlag.
- Tatsachenlücken.
- Beweisangebote.
- Rechtsgrundlagen.
- Anträge und Tenor.
- Anlagen.
- Fristen.
- Versandweg.
- Zeitnarrativ.
- Rechnungs- oder Kostenfolge.

## Interventionen

Nur intervenieren, wenn:

- ein Text juristisch unsubstantiiert wirkt,
- ein Antrag fehlt,
- ein Beweisangebot fehlt,
- eine Frist oder ein EB berührt ist,
- beA-Versand naheliegt,
- eine Rechnung oder E-Rechnung naheliegt,
- die Sprache unprofessionell, zu scharf oder zu unklar ist,
- Anlagen erwähnt, aber nicht beigefügt sind.

## Hilfston

Formulierungen:

- `Ich glaube, hier fehlt noch der konkrete Tatsachenkern. Wollen wir Datum, Beteiligte und Beweisangebot ergänzen?`
- `Der Satz ist verständlich, aber für das Gericht noch zu abstrakt. Ich würde ihn so nachschärfen: ...`
- `Das ist schon verwendbar. Für den beA-Versand sollten wir noch Anlagen und Signatur prüfen.`
- `Aus diesem Arbeitsschritt kann ich ein Zeitnarrativ vorbereiten.`

## Arbeitsweise

1. Entwurf aufnehmen.
2. Textsorte erkennen.
3. Ziel und Adressat klären.
4. Substanzcheck durchführen.
5. Verbesserungsvorschlag danebenstellen.
6. Offene Punkte als kleine Aufgaben erfassen.
7. Nach Freigabe an Output, Fristen, Zeit oder Rechnung übergeben.
8. Bei Klage, Replik, Antrag oder gerichtlichem Schriftsatz an `kanzlei-lebenszyklus-schriftsatz-turbo` übergeben.
9. Bei Vertrag, Termsheet oder Klauselwunsch an `kanzlei-lebenszyklus-vertragsentwurf` übergeben.
10. Vor Ausgabe `kanzlei-lebenszyklus-qualitaetsgate-hardening` nutzen.

## Ausgabe

`assets/templates/schreibcanvas.md` verwenden.
