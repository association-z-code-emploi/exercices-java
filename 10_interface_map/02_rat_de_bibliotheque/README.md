---
tags:
  - exercises
  - java
---

# Exercice 02 : Créer un mini-gestionnaire de bibliothèque

Pour gérer un ensemble de livres, vous allez devoir utiliser une **`Map<String, Livre>`**, où la **clé est le code d'un livre** et sa **valeur est l'objet `Livre`**.

## Consignes

Reprenez votre code de l'exercice précédent et ajoutez-en une copie dans ce dossier d'exercice.

Écrivez ensuite, dans un fichier séparé, une **classe principale** `Bibliothque` avec une méthode `main`.
Déclarez ensuite une **`Map`** qui contiendra des paires de **codes** et de **livres**, puis ajoutez quelques livres à cette `Map`.

Pour vérifier votre code :
- affichez un livre en le recherchant avec son code
- utilisez une méthode de votre `Map` pour afficher un livre **par défaut**, si le code n'existe pas
- affichez **toute la bibliothèque** (tous les codes et leurs livres)
- remplacez un livre existant (même clé, nouvelle valeur)

## Conseils

- Vous avez vu deux implémentation de `Map` : à vous de décider de laquelle qui serait la plus pertinente ici !
- Pour afficher toute la bibliothèque, pensez à soit parcourir de manière à bien pouvoir afficher les codes (clés) et les titres et auteurs (valeurs).
- Pour afficher un livre inexistant, regardez du côté des méthodes de `Map`.
