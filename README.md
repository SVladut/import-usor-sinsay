# import-usor-sinsay

Site simplu, fără server, pentru conversia unui fișier TXT de inventar în Excel.
După publicare, site-ul este disponibil la:
https://svladut.github.io/import-usor-sinsay/

## Utilizare

Deschide `index.html` în browser, completează numele magazinului, codul magazinului
și Plan ID-ul inventarului, apoi selectează fișierul `.txt` și apasă „Generează
fișierul Excel”. Pentru biblioteca de generare Excel este necesară o conexiune la
internet.

TXT-ul trebuie să aibă 8 coloane delimitate cu `;`. Excel-ul conține coloanele
`InventoryPlanId`, `StoreCode`, `Code`, `Variant`, `Name`, `Quantity`,
`AcquisitionPrice`, `SellPrice`. `Name` este egal cu `Variant`. Codul de bare este
formatat ca număr fără zecimale. După export sunt afișate numărul rândurilor din TXT,
numărul rândurilor din Excel (fără antet) și suma stocului (`Quantity`).

Fișierul rezultat se descarcă cu numele:
`Import [Numele magazinului] [Cod magazin] inventar [Plan ID].xlsx`.
