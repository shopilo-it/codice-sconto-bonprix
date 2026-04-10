# Codice sconto Bonprix, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Bonprix** da [shopilo.it](https://shopilo.it/negozi/bonprix.it). Restituisce **coupon Bonprix** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-bonprix](https://shopilo-it.github.io/codice-sconto-bonprix/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-bonprix
cd codice-sconto-bonprix
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Bonprix",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% di sconto sul primo ordine",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/bonprix.it"
  }
]
```

## Coupon Bonprix disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 15% | 15% di sconto sul primo ordine | [shopilo.it](https://shopilo.it/negozi/bonprix.it) |

Codici attivi: **[shopilo.it/negozi/bonprix.it](https://shopilo.it/negozi/bonprix.it)**

## Domande frequenti

### Come utilizzo un codice sconto Bonprix?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/bonprix.it), aggiungi i prodotti al carrello su Bonprix e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Bonprix?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Bonprix piu recenti?
La pagina [shopilo.it/negozi/bonprix.it](https://shopilo.it/negozi/bonprix.it) viene aggiornata quotidianamente con i codici sconto Bonprix, voucher Bonprix e coupon promozionali Bonprix piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Bonprix

Bonprix e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/bonprix.it) trovi i migliori codici sconto Bonprix, coupon Bonprix verificati e voucher Bonprix attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-bonprix
```

```javascript
const { fetchCoupons } = require('codice-sconto-bonprix');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
