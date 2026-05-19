# Installation in einfach — wenn der Marketplace-Weg nicht klappt

> Diese Seite richtet sich an alle, die in Claude Desktop / Cowork **keinen GitHub-Pfad eingeben können** und einfach nur die Plugins ausprobieren wollen. Es ist kein bisschen blöd, dort etwas zu suchen — der GitHub-Pfad gehört in ein anderes Dialogfeld, das je nach Version unterschiedlich heißt oder gar nicht angeboten wird.
>
> Der schnellste Weg ist: **ZIP herunterladen → hochladen → fertig.** Genau dort, wo auch das Plugin „Legal Plugin" landet.

## Kurzfassung

1. Auf [die Releases-Seite](https://github.com/Klotzkette/claude-fuer-deutsches-recht/releases/latest) gehen.
2. Pro gewünschtem Rechtsgebiet **eine ZIP-Datei** herunterladen, z. B. `liquiditaetsplanung.zip`.
3. In Claude Desktop / Cowork auf **Customize → Skills** klicken und zum Abschnitt **Persönliche Plugins / Personal plugins** scrollen — genau die Stelle, an der auch „Legal Plugin" installiert wird.
4. Auf das **+** neben „Persönliche Plugins" klicken und im Dialog das soeben heruntergeladene ZIP auswählen (alternativ: erst auf **Create**, dann **Upload plugin**).
5. Schritte 2–4 für jedes weitere Rechtsgebiet wiederholen, das gebraucht wird.

Das war's. In der Plugin-Liste erscheint das Plugin direkt, kann aktiviert werden, und der Skill ist beim nächsten Chat verfügbar.

## Welches ZIP brauche ich?

Auf der [Releases-Seite](https://github.com/Klotzkette/claude-fuer-deutsches-recht/releases/latest) liegen 17 ZIPs — eines pro Rechtsgebiet. Es muss nicht alles installiert werden; nur das, was gerade gebraucht wird.

| ZIP | Was steckt drin |
| --- | --- |
| `arbeitsrecht.zip` | Kündigung, Aufhebungsvertrag, Abmahnung, BR-Anhörung, KSchG-Klage |
| `betreuungsrecht.zip` | Jahresbericht, Vermögensverzeichnis, Genehmigungspflichten |
| `datenschutzrecht.zip` | DSGVO/BDSG/TTDSG, Auskunft Art. 15, Datenpannenmeldung |
| `forderungsmanagement-klagewerkstatt.zip` | Standardklage aus eigenen Mustern, Zuständigkeitsprüfung |
| `gesellschaftsrecht.zip` | GmbH/AG-Beschlüsse, Due Diligence, HRB-Anmeldung |
| `gewerblicher-rechtsschutz.zip` | Marke, Design, UWG-Abmahnung, Urheberrecht |
| `insolvenzrecht.zip` | §§ 17, 19 InsO, Antragspflicht § 15a InsO, BGH-Volltexte als PDF |
| `jurastudium.zip` | Karteikarten, Gutachten-Coaching, Lernsitzungen |
| `kanzlei-builder-hub.zip` | Werkzeuge zum Bauen eigener kanzleiinterner Skills |
| `ki-governance.zip` | KI-VO, KI-Inventar, Vendor Review |
| `liquiditaetsplanung.zip` | 3-Wochen-Vorschau, 13/26/52-Wochen-Planung, BGH-Schema |
| `produktrecht.zip` | Launch-Review, Impressum, PAngV, Marketing-Claims |
| `prozessrecht.zip` | Mahnbescheid, einstweilige Verfügung, Schutzschrift, Zwangsvollstreckung |
| `rechtsberatungsstelle.zip` | Pro-Bono, studentische Beratung |
| `regulatorisches-recht.zip` | Regulatorisches Monitoring nach Branche |
| `steuerberater-werkzeuge.zip` | BWA-/SuSa-Prüfung, Krisenfrüherkennung |
| `vertragsrecht.zip` | NDA, AGB, SaaS, Lieferantenverträge |

Wer **nur die Liquiditätsplanung** ausprobieren will, lädt sich nur `liquiditaetsplanung.zip` herunter. Wer sich umsehen möchte, lädt drei oder vier ZIPs.

## Bonus: die Beispielakte

Wer die Liquiditätsplanung an einem konkreten Fall durchspielen will, lädt sich zusätzlich `beispielakte-edelholz-berlin.zip` herunter. Das ist ein fingierter Mandant mit fingierten Bankauszügen, BWA, offenen Forderungen und allem, was eine Drei-Wochen-Vorschau braucht.

## Hilfe, kein „+" da

Je nach Claude-Desktop- / Cowork-Version sieht der Plugin-Dialog leicht anders aus. Die typischen Stellen, an denen der Upload-Knopf sitzt:

- **Customize → Skills → Persönliche Plugins → +** (häufigste Variante)
- **Customize → Skills → Personal plugins → + → Upload from .zip**
- **Customize → Plugins → Add → Install from file** (ältere Versionen)

Wichtig ist nur: gesucht wird der Punkt, an dem **eine einzelne ZIP-Datei** vom Rechner ausgewählt werden kann. Wenn dort stattdessen nach einem GitHub-Pfad gefragt wird, ist das das **andere** Dialogfeld — auf **Cancel** und einen Schritt zurück.

## Wenn nichts davon klappt

In aktuelleren Claude-Code- / Cowork-Versionen geht auch direkt der Marketplace-Befehl (im Terminal):

```text
/plugin marketplace add Klotzkette/claude-fuer-deutsches-recht
/plugin install liquiditaetsplanung
```

Falls das ebenfalls kein Dialogfeld findet, ist die Cowork-Version zu alt für Marketplaces — dann ist der ZIP-Upload oben der einzige Weg, und das ist völlig in Ordnung. Er funktioniert in jeder Version, die Plugin-Upload überhaupt kennt.

## Sanity-Check

Nach der Installation in eine neue Konversation gehen und schreiben:

> „Bitte mache eine 3-Wochen-Liquiditätsvorschau für eine kleine GmbH."

Wenn Claude jetzt nach Sachverhalt, Bankstand, offenen Forderungen und Daueraufträgen fragt und am Ende eine Excel-Tabelle vorschlägt, ist die Installation gelungen.

## Probleme?

[Issue auf GitHub aufmachen](https://github.com/Klotzkette/claude-fuer-deutsches-recht/issues/new) — Screenshot vom Dialog mit dabei hilft enorm. Es ist kein bisschen nervig; jede Rückmeldung macht die Anleitung besser.
