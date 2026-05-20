# Geschäftskonto-Simulation

## Status

- Geschäftskonto nicht angebunden.
- Keine echten Bankzugangsdaten.
- Kontoauszug als CSV-Testdatei vorhanden.
- Keine Zahlungsaufträge erlaubt.

## Erwarteter Workflow

1. Fragen, ob Geschäftskonto angebunden, CSV importiert oder Simulation genutzt werden soll.
2. Bei Simulation `geschaeftskonto_mai_2026.csv` importieren.
3. Offene Posten aus `offene_posten_debitoren.csv` laden.
4. Zahlungseingänge matchen.
5. Schwache Matches und Klärfälle markieren.
6. Keine endgültige Buchung behaupten.
7. DATEV-/Steuerkanzlei-Übergabe simulieren.
