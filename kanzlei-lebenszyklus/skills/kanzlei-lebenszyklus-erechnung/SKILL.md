---
name: kanzlei-lebenszyklus-erechnung
description: "Bereitet elektronische Kanzleirechnungen in XRechnung und ZUGFeRD vor. Prüft EN 16931 Pflichtdaten GoBD-nahe Aufbewahrung strukturierte XML-Daten PDF-A-3-Hybrid bei ZUGFeRD Validierung Rechnungskorrektur und Freigabe."
---

# E-Rechnung, XRechnung, ZUGFeRD und GoBD

## Zweck

Dieser Skill ergänzt `kanzlei-lebenszyklus-rechnung`, sobald eine Rechnung als E-Rechnung erstellt, geprüft, archiviert oder versandt werden soll. Er erzeugt keine Steuerberatung und keine finale Buchung, sondern ein prüfbares Datenblatt, eine Formatentscheidung und eine Validierungs- und Archivierungscheckliste.

## Grundentscheidung

Zuerst klären:

1. Rechnungsempfänger: Verbraucher, Unternehmer, öffentliche Stelle, Rechtsschutzversicherung, Dritter.
2. Bereich: B2B, B2G, B2C oder intern.
3. Formatwunsch oder Formatpflicht: XRechnung, ZUGFeRD, PDF, Papier, sonstiges Format.
4. Leitweg-ID oder Buyer Reference: nur erforderlich, wenn Empfänger oder B2G-Prozess sie verlangt.
5. Versandweg: E-Mail, Portal, Peppol, Mandantenportal, beA nur wenn passend.
6. Archivsystem: GoBD-konformes DMS, Kanzleisoftware, Dateisystem mit Verfahrensdokumentation oder Übergabe an Steuerkanzlei.

## Aktualitätscheck

Vor technischer Aussage zur Gültigkeit immer die aktuelle Format- und Validatorlage prüfen:

- XRechnung: aktuelle KoSIT-/XRechnung-Version und Validator-Konfiguration.
- B2G: aktuelle Vorgaben der jeweiligen Eingangsplattform, Leitweg-ID und Portal-/Peppol-Anforderungen.
- ZUGFeRD: aktuelles Profil, PDF/A-3-Anforderungen und XML-Profil.
- BMF-/USt-Hinweise zur E-Rechnung, soweit für B2B/B2G relevant.

Wenn diese Prüfung nicht durchgeführt wurde, nur `Validierung offen` ausgeben.

## Formate

### XRechnung

- Reines strukturiertes XML-Format.
- Für öffentliche Auftraggeber im B2G-Kontext zentral.
- Enthält keinen menschenlesbaren PDF-Rechnungsteil.
- Muss gegen den passenden XRechnung-Validator und die jeweils geltenden Geschäftsregeln geprüft werden.
- Bei B2G Empfängeranforderungen wie Leitweg-ID, Portal, Peppol und Attachments abfragen.

### ZUGFeRD

- Hybridformat aus PDF/A-3-Sichtrechnung und eingebetteter XML-Datei.
- Der strukturierte XML-Teil ist für E-Rechnungszwecke führend.
- Profil bewusst wählen: typischerweise EN 16931 oder ein zulässiges höheres Profil; MINIMUM und BASIC-WL nicht als vollwertige E-Rechnung behandeln.
- PDF und XML müssen inhaltlich konsistent sein.
- PDF/A-3-Validierung, XML-Validierung und Dateianhänge prüfen.

## Pflichtdaten

Für jede E-Rechnung eine Datenvollständigkeitsprüfung erstellen:

- Rechnungsnummer, Rechnungsdatum, Leistungsdatum oder Leistungszeitraum.
- Verkäufer: Name, Anschrift, Steuernummer oder USt-IdNr., Bankverbindung.
- Käufer: Name, Anschrift, Buyer Reference oder Leitweg-ID, soweit erforderlich.
- Akte, Mandant, Kostenschuldner und abweichender Rechnungsempfänger.
- Positionsdaten: Leistung, Menge oder Zeit, Einheit, Einzelpreis, Nettobetrag, Steuersatz, Steuerbetrag.
- RVG-Gebühren, Auslagen, Post- und Telekommunikationspauschale, Dokumentenpauschale, Gerichtskosten, Fremdgelder getrennt ausweisen.
- Vorschüsse, Zahlungen, Anrechnungen und Rechtsschutzanteile.
- Zahlungsziel, IBAN, Verwendungszweck.
- Steuerhinweise, Reverse Charge, Kleinunternehmer oder Steuerbefreiung nur nach Prüfung.

## GoBD-nahe Rechnungsakte

Vor Freigabe immer ein `GoBD-Prüfprotokoll` erzeugen:

1. Rechnungsversion eindeutig benennen.
2. Entwurfsfassung und freigegebene Fassung trennen.
3. Finales XML unverändert archivieren.
4. Bei ZUGFeRD zusätzlich PDF/A-3 und eingebettetes XML archivieren.
5. Validierungsbericht speichern.
6. Versandnachweis speichern.
7. Korrekturen nur als Storno, Gutschrift, Korrekturrechnung oder neue Rechnungsversion dokumentieren.
8. Zugriffsrechte, Änderungsprotokoll, Aufbewahrungsfrist und Exportfähigkeit notieren.

## Validierung

Keine finale E-Rechnung ohne:

- Formatentscheidung.
- Pflichtdatencheck.
- Summenprüfung netto, Steuer, brutto.
- Rundungsprüfung.
- Prüfung strukturierter Daten gegen die Sichtrechnung.
- Technische Validierung mit geeignetem Validator.
- Freigabe durch verantwortliche Person.

Wenn kein Validator verfügbar ist, nicht behaupten, dass die E-Rechnung gültig sei. Stattdessen einen `Validierung offen`-Vermerk und eine konkrete Tool-Anforderung ausgeben.

## Ausgabe

- `assets/templates/erechnung-datenblatt.md`.
- `assets/templates/gobd-rechnungsprotokoll.md`.
- Bei normaler Rechnungsarbeit zusätzlich `assets/templates/rechnungsdatenblatt.md`.
