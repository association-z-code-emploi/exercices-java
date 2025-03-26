---
tags:
  - exercises
  - java
---

# Exercice 03 : Objet de quête

Parfois, un objet n'est ni équipable, ni consommable. Il attend juste le bon moment pour être utilisé, faire progresser l'aventure ... ou être oublié au fond de l'inventaire.

Tant qu'il est vendu, ce n'est de toutes façons plus votre problème !

## Consignes

Reprenez le code de votre exercice précédent ("[02_multiples_objets](../02_multiples_objets/README.md)"), créez un nouvelle classe `QuestItem` qui :

- hérite toujours de `Item`
- ajoute un nouvel **attribut** `description`, qui sera une **string**
- lors d'un appel de `displayInfos()`, seule le nom et la description doivent s'afficher

> Même si on ne l'affichera pas, un objet de quête a tout de même un poids.

Reprenez vos précédentes **instance** de `Item`, `Weapon` et `Armor`, et créez mainteant une **instance** de `QuestItem`. Appelez `displayInfos()` pour chacune des instances :

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
-----------------------------------
Name: Mystic Crystal
Description: It's glowing when you touch it.
```

## Conseils

- Cette fois, la méthode `displayInfos` doit être remplacée entièrement dans la nouvelle classe `QuestItem`, puisque vous n'avez plus besoin d'afficher le poids.
- Seriez-vous surpris si vous deviez réutiliser le code de cet exercice dans le prochain ?
