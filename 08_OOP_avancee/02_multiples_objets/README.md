---
tags:
  - exercises
  - java
---

# Exercice 02 : Remplir la boutique

Dans une boutique, avoir un objet, c'est bien. En avoir plusieurs, et donc du choix, c'est mieux !

## Consignes

Reprenez le code de votre exercice précédent ("[01_boutique](../01_boutique/README.md)"), et créez deux nouvelles classes nommées `Weapon` et `Armor`, qui :

- héritent de `Item`
- ajoutent un nouvel **attribut** :
  - pour `Weapon` : `damage` qui doit être un **nombre entier** et **privé**, pour indiquer les dégâts que l'arme en question peut infliger
  - pour `Armor` : `protection` qui doit aussi être un **nombre entier** et **privé**, pour indiquer la résistance aux dégâts pouvant être subis
- affiche ce nouvel attribut en supplément lors de l'appel de `displayInfos()`, comme montré dans l'exemple ci-dessous

Reprenez votre précédente **instance** de `Item` et créer aussi une **instance** de `Weapon` et de `Armor`. Appelez `displayInfos()` pour chacune des instances :

```
-----------------------------------
Name: Potion
Weight: 0.5 kg
-----------------------------------
Name: Sword
Weight: 2.5 kg
Damage: 10
-----------------------------------
Name: Helmet
Weight: 1.2 kg
Protection: 2
```

## Conseils

- La méthode `displayInfos()` ne doit pas être entièrement réécrite dans la nouvelle classe `Weapon` et `Armor` : réutilisez celle de `Item` et ajoutez-lui simplement une nouvelle ligne à afficher dans le terminal !
- Une nouvelle fois, vous allez réutiliser ce code lors du prochain exercice : assurez qu'il fonctionne comme demandé !
