---
tags:
  - exercises
  - java
---

# Exercice 03 : usine automobile

## Consignes

Créez une classe `Car` avec :

- un **attribut** `numberOfCars` (nombre entier, accessible par toutes les instances de la classe `Car`) qui compte le nombre total de voitures créées
- un **attribut** `serialNumber` (nombre entier, fixe et immuable) initialisé dans le constructeur
- un **constructeur** qui incrémente `numberOfCars` à chaque création d'une voiture

Dans `main()`, créez plusieurs objets et affichez leurs numéros de série ainsi que le nombre total de voitures crées.

## Conseil

Pour afficher le nombre total de voitures crées, vous devez passer directement pas la **classe**, et non pas par un **objet**.
