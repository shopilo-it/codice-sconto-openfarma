# Codice sconto OpenFarma, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto OpenFarma** da [shopilo.it](https://shopilo.it/negozi/openfarma.it). Restituisce **coupon OpenFarma** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-openfarma](https://shopilo-it.github.io/codice-sconto-openfarma/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-openfarma
cd codice-sconto-openfarma
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "OpenFarma",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su farmaci da banco e parafarmaci",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/openfarma.it"
  }
]
```

## Coupon OpenFarma disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su farmaci da banco e parafarmaci | [shopilo.it](https://shopilo.it/negozi/openfarma.it) |

Codici attivi: **[shopilo.it/negozi/openfarma.it](https://shopilo.it/negozi/openfarma.it)**

## Domande frequenti

### Come utilizzo un codice sconto OpenFarma?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/openfarma.it), aggiungi i prodotti al carrello su OpenFarma e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon OpenFarma?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher OpenFarma piu recenti?
La pagina [shopilo.it/negozi/openfarma.it](https://shopilo.it/negozi/openfarma.it) viene aggiornata quotidianamente con i codici sconto OpenFarma, voucher OpenFarma e coupon promozionali OpenFarma piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su OpenFarma

OpenFarma e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/openfarma.it) trovi i migliori codici sconto OpenFarma, coupon OpenFarma verificati e voucher OpenFarma attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-openfarma
```

```javascript
const { fetchCoupons } = require('codice-sconto-openfarma');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
