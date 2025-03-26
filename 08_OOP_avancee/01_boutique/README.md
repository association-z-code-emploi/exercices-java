---
tags:
  - exercises
  - java
---

# Exercice 01 : Boutique de RPG

Dans un jeu RPG, tous les objets possèdent des caractéristiques, comme un **nom** ou un **poids**. Ceertains objets sont des armes, des armures, des consommables, etc... Dans cette série d'exercices, vous allez créer une boutique qui pourra contenir tous ces objets grâce aux **notions avancées de l'OOP** !

> On vous conseillera de créer un nouveau projet pour chaque projet ou de renommer différemment vos fichiers des autres exercices, pour éviter :
> - de n'écrire que dans un seul et même fichier
> - d'avoir des conflits avec le nom des classes

## Consignes

Dans un fichier `Shop.java`, codez une classe `Item`, avec les **attributs** suivants :

- `name` pour le nom de l'objet, qui sera une **string**
- `weight` pour son poids, qui sera une **un nombre décimal**

Ces deux attributs doivent être **protégés**.

Ajoutez un **méthode** `displayInfo()` qui affichera les caractéristiques de l'objet, comme montré dans l'exemple ci-dessous.

Créez ensuite une **instance de cette classe**, puis appelez la méthode pour afficher les caractéristiques d'un objet dans le terminal :

```
-----------------------------------
Name: Potion
Weight: 0.5 kg
```

## Conseils

- Le faux "trait" (`----`) n'est là que pour séparer visuellement les différents objets affichés. À vous de décider de le mettre ou non !
- N'oubliez pas d'utiliser un **constructeur** pour plus facilement créer un nouvel objet de `Item`.
- Vous ne devez pas utiliser de **paramètres** dans la méthode : appelez directement les **attributs** de l'objet concerné, donnez par le **constructeur**.
- Vous allez réutiliser ce code lors du prochain exercice : assurez qu'il fonctionne comme demandé !
