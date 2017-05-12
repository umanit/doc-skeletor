# Doc Skeletor

![Skeletor IMG](https://static.comicvine.com/uploads/original/4/49448/2444870-skeletor__1_.jpg)

Doc Skeletor est outil de génération de structure de documentation unifiée au travers de tous les projets UmanIT.

## Installation

Assurez vous d'avoir [composer](https://getcomposer.org/) installé sur votre poste.

Si vous n'avez pas de composer.json existant, lancez la commande `composer init`

Puis lancez `composer require umanit/doc-skeletor`

Ajoutez ce script à votre fichier composer.json.

```javascript
    "scripts": {
        "post-update-cmd": "cp -an vendor/umanit/doc-skeletor/skeleton/. ./ || true"
    }
```
Puis lancez `composer update`

Un fichier readme.md et un répertoire _doc seront créés à la racine du projet

## Note

Cet outil génère un squelette de doc mais celle-ci peut rester libre, vous pouvez modifier la structure et le contenu selon vos besoins, ceux-ci ne seront pas écrasés.

## Contribuer

Si vous constatez du boilerplate à rajouter au squelette, n'hésitez pas à créer des pull-requests.
