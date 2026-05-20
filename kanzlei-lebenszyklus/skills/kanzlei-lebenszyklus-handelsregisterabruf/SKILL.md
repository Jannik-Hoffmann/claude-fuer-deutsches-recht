---
name: kanzlei-lebenszyklus-handelsregisterabruf
description: "Führt durch Handelsregisterabruf über offizielle Registerquellen. Sichert Firma Sitz Registergericht Registernummer Vertretung Prokura Gesellschafterliste Gesellschaftsvertrag Dokumente Quelle Zeitstempel und Vertragsprüfung."
---

# Handelsregisterabruf

## Zweck

Dieser Skill führt durch einen Handelsregisterabruf und macht daraus ein verwertbares Registerprotokoll für Klage, Vertrag, Mandatsanlage, KYC, Rechnungsadresse oder Zustellung. Er nutzt offizielle Quellen und dokumentiert Quelle, Zeitstempel und Unsicherheiten.

## Offizielle Quellen

- Gemeinsames Registerportal der Länder: `https://www.handelsregister.de`.
- Unternehmensregister: `https://www.unternehmensregister.de`.
- Nicht auf Drittanbieter verlassen, wenn es um Vertretung, Registerstand oder aktuelle Dokumente geht.

Wenn kein Browser- oder Registerzugang vorhanden ist, einen Simulationsmodus anbieten. Im Simulationsmodus müssen alle Registerdaten als fiktiv oder ungeprüft gekennzeichnet werden.

## Abrufziel klären

1. Firma oder Name.
2. Rechtsform.
3. Sitz.
4. Registergericht.
5. Registernummer.
6. Zweck: Klage, Zustellung, Vertrag, Vollmacht, Rechnung, KYC, Due Diligence.
7. Benötigte Dokumente: aktueller Abdruck, chronologischer Abdruck, Gesellschafterliste, Gesellschaftsvertrag, Registerbekanntmachung.

## Prüfprogramm

- Firma exakt übernehmen.
- Rechtsform und Sitz prüfen.
- Registergericht und Registernummer festhalten.
- Vertretungsberechtigung prüfen.
- Einzel- oder Gesamtvertretung prüfen.
- Prokura prüfen.
- Liquidation, Insolvenz, Löschung oder Umwandlung prüfen.
- Zustellfähige Anschrift nicht blind aus Handelsregister ableiten, wenn Zustellung kritisch ist.
- Dokumentdatum und Abrufzeitpunkt protokollieren.

## Such- und Trefferlogik

- Schreibvarianten, alte Firma, Sitzverlegung und Rechtsformzusatz prüfen.
- Mehrere Treffer nicht zusammenführen, sondern getrennt darstellen.
- Bei UG, GmbH, AG, KG, OHG, PartG und e. K. Rechtsform exakt übernehmen.
- Bei Zweigniederlassungen Hauptniederlassung und Vertretung gesondert prüfen.
- Bei Konzernnamen nicht automatisch die richtige Vertragspartnerin annehmen.

## Verwendung

Für Klage:

- Parteibezeichnung und Vertretung prüfen.
- Zustelladresse gesondert validieren.
- Anlagenbezeichnung für Registerauszug vergeben.

Für Vertrag:

- Parteibezeichnung.
- Vertretung und Zeichnungsberechtigung.
- Handelsregisterdaten in Rubrum oder Präambel.

Für Rechnung und Buchhaltung:

- Rechnungsempfänger mit Firma, Rechtsform und Anschrift abgleichen.
- Debitorenstamm aktualisieren.
- Zahlungszuordnung nicht allein aus Registerdaten ableiten.

## Warnlogik

`STOPP` ausgeben, wenn:

- Firma oder Rechtsform unklar ist.
- Vertretung nicht geprüft ist.
- der Registerstatus Liquidation, Löschung, Insolvenz oder Umwandlung nahelegt.
- die Anschrift für Zustellung oder Vertrag nicht belastbar ist.

`WARNUNG` ausgeben, wenn:

- nur eine Simulation vorliegt.
- Dokumente älter sind als der aktuelle Entscheidungsbedarf.
- Gesellschafterliste, Satzung oder Prokura relevant sein könnten, aber fehlen.

## Ausgabe

`assets/templates/handelsregisterabruf-protokoll.md` verwenden.
