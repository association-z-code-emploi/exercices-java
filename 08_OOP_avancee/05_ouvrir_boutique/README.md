---
tags:
  - exercises
  - java
---

# Exercice 05 : Ouvrir boutique

Vous y êtes : vous allez enfin ouvrir botre boutique d'objets !

Ou presque car vos objets "classiques" ne le sont jamais vraiment : armes, armures, objets de quête, ou consommables dans le cas d'une Potion.

Modifiez une dernière fois votre code pour avoir un résultat "de pro" !

## Consignes

Reprenez le code de votre exercice précédent ("[04_utiliser_un_objet](../04_utiliser_un_objet/README.md)"), et modifiez votre classe `Item` pour qu'elle devienne **abstraite** : cette classe représentera maintenant un objet général, avec toujours un nom, un poids et une méthode `use()` qui sera toujours une **interface** mais maintenant **abstraite** via `Item`.

Créez aussi une classe `Aid` qui :
- hérite toujours de `Item`
- ajoute un nouvel **attribut** `healAmount`, qui sera un **nombre entier** pour représenter un soin
- lors d'un appel de `displayInfos()`, affichez la valeur de `healAmount` en plus du nom et du poids

Réutilisez vos précédentes **instances** de la classe `Item`, en ajoutant désormais `Aid`, avec toujours l'**implémentation** de la méthode `use()` en fonction de leur type spécifique.

Le résultat doit ressembler à ceci, dans le terminal :

```
-----------------------------------
Name: Healing Potion
Weight: 0.5 kg
Heal Amount: 50
-----------------------------------
Using Healing Potion: Restoring 50 HP!
-----------------------------------
Name: Sword
Weight: 2.5 kg
Damage: 10
-----------------------------------
Using Sword: Inflicting 10 damage!
-----------------------------------
Name: Helmet
Weight: 1.2 kg
Protection: 2
-----------------------------------
Using Helmet: Absorbing 2 incoming damage!
-----------------------------------
Name: Crystal
Description: It's glowing.
-----------------------------------
Using Crystal: You can't use it right now.
```
