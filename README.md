# Code promo Castorama, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Castorama** depuis [shopilo.fr](https://shopilo.fr/reductions/castorama.fr). Renvoie les **coupons Castorama** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-castorama](https://shopilo-fr.github.io/code-promo-castorama/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-castorama
cd code-promo-castorama
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Castorama",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur le bricolage et l'amenagement",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/castorama.fr"
  }
]
```

## Coupons Castorama disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur le bricolage et l'amenagement | [shopilo.fr](https://shopilo.fr/reductions/castorama.fr) |

Codes actifs : **[shopilo.fr/reductions/castorama.fr](https://shopilo.fr/reductions/castorama.fr)**

## Questions frequentes

### Comment utiliser un code promo Castorama ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/castorama.fr), ajoutez les produits a votre panier sur Castorama et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Castorama ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Castorama les plus recents ?
La page [shopilo.fr/reductions/castorama.fr](https://shopilo.fr/reductions/castorama.fr) est mise a jour quotidiennement avec les codes promo Castorama, bons de reduction Castorama et coupons promotionnels Castorama les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Castorama

Castorama est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/castorama.fr), retrouvez les meilleurs codes promo Castorama, coupons Castorama verifies et bons de reduction Castorama actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-castorama
```

```javascript
const { fetchCoupons } = require('code-promo-castorama');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
