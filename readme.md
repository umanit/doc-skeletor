# Doc Skeletor

![Skeletor IMG](https://static.comicvine.com/uploads/original/4/49448/2444870-skeletor__1_.jpg)

Doc Skeletor est outil de génération de structure de documentation unifiée au travers de tous les projets UmanIT.

## Usage

Configurez votre fichier composer.json comme suit :

```javascript
{
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/umanit/doc-skeletor"
        }
    ],
    "require": {
        "umanit/doc-skeletor": "dev-master"
    },
    "scripts": {
        "post-install-cmd": "cp -an vendor/umanit/doc-skeletor/skeleton/. ./ || true"
    }
}

```
Puis, `composer update`

Un fichier readme.md et un répertoire doc seront créés à la racine du projet

## Note

Cet outil génère un squelette de doc mais celle-ci rester libre, vous modifier la structure et le contenu selon vos besoins.

## Contribuer

Si vous constatez du boilerplate à rajouter au squelette, n'hésitez pas à créer des pull-requests.