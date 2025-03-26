---
tags:
  - exercises
  - java
---

# Exercice 04 : Utiliser un objet

Avoir de l'équipement est important. Bien l'utiliser est vital !

## Consignes

Reprenez le code de votre exercice précédent ("[03_objet_de_quete](../03_objet_de_quete/README.md)"), et créez une **interface** `Using` avec une **méthode** `use()` qui aura un retour `void`. Lorsqu'on utilisera cette méthode, on affichera un message indiquant l'effet d'un objet, selon l'objet.

> Celui de `Item` et de `QuestItem` seront toujours les mêmes, comme montrés dans l'exemple ci-dessous.

En conservant les appels de `displayInfos()`, appelez aussi `use()` pour chacune des instances :

```
-----------------------------------
Name: Potion
Weight: 0.5 kg
-----------------------------------
Using Potion : It's useful!
-----------------------------------
Name: Sword
Weight: 2.5 kg
Damage: 10
-----------------------------------
Using Sword : Inflicting 10 damage!
-----------------------------------
Name: Helmet
Weight: 1.2 kg
Protection: 2
-----------------------------------
Using Helmet : Absorbing 2 incoming damage!
-----------------------------------
Name: Mystic Crystal
Description: It's glowing when you touch it.
-----------------------------------
Using Mystic Crystal : You can't use it now.
```

## Conseil

- Un dernier copier/coller pour la route ?
