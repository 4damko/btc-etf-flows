# BTC Spot ETF — Inflow / Outflow

Lokálny dashboard denných tokov do/z amerických spotových Bitcoin ETF.

## 👉 Použitie

Dvojklik na **`BTC ETF Flows.html`** → otvorí sa v prehliadači a **sám si stiahne
aktuálne dáta**. Kedykoľvek chceš čerstvé čísla → stlač **↻ Obnoviť** (alebo refresh
v prehliadači, Cmd+R).

- **Nič nebeží na pozadí** — žiadny server, žiadny démon, nulová záťaž CPU/energie,
  kým stránku neotvoríš.
- Dáta sa ťahajú naživo priamo z prehliadača (SoSoValue OpenAPI, bez kľúča).
- Potrebuje len internet (kvôli dátam + Chart.js z CDN).

## Čo ukazuje
- Karty: denný čistý tok, kumulatív, AUM, denný obrat, BTC v držbe
- **Prehľad** — súhrn + zoznamy za posledné **3 / 7 / 30 dní**
- Graf denných tokov (zelená inflow / červená outflow) + prepínač 30D/90D/180D/1R/Max
- Kumulatívny graf
- Tabuľka po jednotlivých ETF (IBIT, FBTC, GBTC, ARKB…)

## Pojmy
- **Denný tok** – koľko peňazí čisto pritieklo/odtieklo za 1 deň.
- **Kumulatív** – súčet všetkých denných tokov od štartu ETF (vstupný kapitál).
- **AUM** – dnešná trhová hodnota všetkého BTC vo fondoch (vrátane rastu ceny).

## Ethereum ETF
V `BTC ETF Flows.html` (sekcia `<script>`) zmeň `const ASSET = "us-btc-spot"`
na `"us-eth-spot"`.

---
_Pozn.: súbory `update.py`, `dashboard.html`, `flows.json`, `btc_etf_flows.pine`
a `Aktualizuj BTC ETF.command` sú zo staršieho prístupu (generovanie + Pine) a už
nie sú potrebné — pokojne ich zmaž._
