# Cod reducere Douglas — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Douglas** de pe [shopilo.ro](https://shopilo.ro/magazin/douglas.ro). Returneaza **cupoane Douglas** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-douglas](https://shopilo-ro.github.io/cod-reducere-douglas/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-douglas
cd cod-reducere-douglas
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Douglas",
    "code": "SHOPILO25",
    "discount": "25%",
    "description": "Pana la 25% reducere plus livrare gratuita",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/douglas.ro"
  }
]
```

## Cupoane Douglas disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 25% | Pana la 25% reducere plus livrare gratuita | [shopilo.ro](https://shopilo.ro/magazin/douglas.ro) |

Codurile active: **[shopilo.ro/magazin/douglas.ro](https://shopilo.ro/magazin/douglas.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Douglas?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/douglas.ro), adauga produsele in cos pe Douglas, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Douglas?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Douglas?
Pagina [shopilo.ro/magazin/douglas.ro](https://shopilo.ro/magazin/douglas.ro) este actualizata zilnic cu cele mai noi cod reducere Douglas, voucher Douglas si cupon promotional Douglas.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Douglas

Douglas este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/douglas.ro) cele mai bune cod reducere Douglas, cupoane Douglas verificate si voucher Douglas active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-douglas
```

```javascript
const { fetchCoupons } = require('cod-reducere-douglas');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
