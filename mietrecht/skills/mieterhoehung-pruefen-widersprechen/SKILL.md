---
name: mieterhoehung-pruefen-widersprechen
description: Mietersicht — pruefe ein Mieterhoehungsverlangen nach ortsueblicher Vergleichsmiete (§§ 558 ff. BGB) auf Form Frist Kappungsgrepze Begruendung und entwirf bei Bedarf eine Zustimmungsverweigerung oder Teilzustimmung. Pruefroutine deckt Textform Wartefrist Kappungsgrenze (zwanzig Prozent oder fuenfzehn Prozent in Spannungsgebieten) und Begruendungsmittel (Mietspiegel Sachverstaendigengutachten Vergleichswohnungen) ab. Erzeugt Entwurf mit Disclaimer.
---

# Mieterhoehung pruefen und widersprechen

## Disclaimer (Schluesselstelle)

Diese Pruefung und der nachstehende Entwurf ersetzen **keine Rechtsberatung**. Vor Versand des Schreibens an den Vermieter ist eine anwaltliche oder mietervereinsseitige Kontrolle dringend zu empfehlen. Fristversaeumnisse fuehren zu gesetzlicher Zustimmung nach § 558b Abs. 2 BGB.

## Workflow

### Schritt 1 — Daten beschaffen

- Mieterhoehungsverlangen im Wortlaut.
- Datum des Zugangs (Briefkasten-Eintrag, E-Mail-Empfang).
- Lage- und Ausstattungsprotokoll aus dem Skill `lage-und-ausstattung-erheben`.
- Auszug aus dem aktuellen amtlichen Mietspiegel der Stadt aus `references/mietspiegel-quellen.md`.

### Schritt 2 — Formpruefung

- **Textform** nach § 558a Abs. 1 BGB (Brief, Fax, E-Mail mit Unterschriftstext genuegen).
- **Empfaengerangabe** alle Mieter namentlich.
- **Begruendung** auf Mietspiegel, Sachverstaendigengutachten oder drei Vergleichswohnungen gestuetzt (§ 558a Abs. 2 BGB).
- **Beilage** falls Mietspiegelauszug, dann gut lesbar.

### Schritt 3 — Wartefrist und Sperrjahr

- Die neue Miete darf fruehestens **fuenfzehn Monate** nach Einzug oder nach der letzten Erhoehung verlangt werden (§ 558 Abs. 1 BGB).
- Berechnung dokumentieren.

### Schritt 4 — Kappungsgrenze (§ 558 Abs. 3 BGB)

- Regelgrenze **zwanzig Prozent** in drei Jahren.
- In Gebieten der Kappungsgrenzenverordnung **fuenfzehn Prozent** in drei Jahren — Pruefung anhand der Landesverordnung (siehe `references/mietspiegel-quellen.md`).

### Schritt 5 — Materielle Pruefung der ortsueblichen Vergleichsmiete

- Wohnlage einordnen.
- Spanne im qualifizierten Mietspiegel suchen.
- Einordnung innerhalb der Spanne nach Orientierungshilfe (Auf- und Abschlaege fuer Ausstattungsmerkmale).
- Vergleichsmiete je m² ermitteln, mit Wohnflaeche multiplizieren.

### Schritt 6 — Reaktionsfristen

- **Zustimmungsfrist** § 558b Abs. 2 BGB. Ablauf des zweiten Kalendermonats nach Zugang.
- Bei Schweigen: Vermieter kann auf Zustimmung klagen (§ 558b Abs. 2 Satz 2 BGB).

### Schritt 7 — Entwurfsoptionen

- **Volle Zustimmung** wenn Begehren formal und materiell richtig ist.
- **Teilzustimmung** bis zur tatsaechlich ortsueblichen Vergleichsmiete.
- **Verweigerung** bei Formfehlern, Verstoss gegen Wartefrist oder Kappungsgrenze.

## Schreiben-Entwurf

Erzeuge ein hoeflich-bestimmtes Schreiben mit:

1. Bezugnahme auf das Verlangen vom (Datum).
2. Rechtliche Pruefung punktweise (Form, Frist, Kappungsgrenze, ortsuebliche Vergleichsmiete).
3. Eindeutige Erklaerung (Zustimmung, Teilzustimmung, Verweigerung).
4. Aufforderung zur schriftlichen Bestaetigung.
5. **Disclaimer am Ende** — Hinweis, dass dies kein anwaltliches Schreiben ist und der Mieter sich beraten lassen sollte.
