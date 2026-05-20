---
name: kanzlei-lebenszyklus-aktenzeichen
description: "Erkennt und verknüpft eigene Aktenzeichen mit Gericht Behörde Gegner Versicherung Mandant Rechtsschutz und Altakten. Normalisiert Varianten findet Kollisionen und schlägt eindeutige Verknüpfungen vor. Nutzt nie unsichere Zuordnung ohne Rückfrage."
---

# Aktenzeichen und Verknüpfungen

## Zweck

Dieser Skill verhindert Suchchaos. Er erkennt Aktenzeichen aus Texten, Dateinamen, Betreffzeilen, beA-Nachrichten, PDFs, Screenshots und Notizen und verknüpft sie mit der richtigen Kanzleiakte.

## Typen von Aktenzeichen

- Eigenes Kanzlei-Aktenzeichen.
- Gerichtliches Aktenzeichen.
- Behördenzeichen.
- Gegnerisches Aktenzeichen.
- Versicherungs- oder Schadennummer.
- Rechtsschutz-Schadennummer.
- Mandanteninterne Projektnummer.
- Altaktenzeichen.

## Ablauf

1. Alle Kandidaten extrahieren.
2. Varianten normalisieren: Leerzeichen, Schrägstrich, Bindestrich, führende Nullen.
3. Kontext prüfen: Name, Gericht, Gegner, Datum, Betreff.
4. Kollisionen markieren.
5. Eindeutige Verknüpfung vorschlagen.
6. Unsichere Zuordnung als Rückfrage ausgeben.

## Ausgabe

```markdown
## Aktenzeichen-Verknüpfung

| Typ | Aktenzeichen | Quelle | Akte | Sicherheit | Notiz |
| --- | --- | --- | --- | --- | --- |
```

## Sicherheitsregel

Wenn zwei Akten plausibel sind, nicht automatisch ablegen. Immer nachfragen.
