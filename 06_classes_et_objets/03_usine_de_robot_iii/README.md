---
tags:
  - exercises
  - java
---

# Exercice 03 : usine de robots (suite de la suite)

Ajoutons enfin une **méthode** pour rendre la création de robots plus complète ; voire terminée !

## Consignes

Copiez et collez votre classe `Robot.java` de l'exercice précédent (avec un constructeur) pour ajouter une **méthode** qui affichera les informations d'un robot dans le terminal de la même façon que précédemment :

```
Nono le petit robot est rouge et a le numéro de modèle 23.
K9 est gris et a le numéro de modèle 1.
...
```

## Conseil

Pas besoin d'avoir de paramètres dans ces méthodes : appelez directement les variables/champs concernés ; ils sauront automatiquement aller chercher leurs valeurs associés à leur instance ! C'est à dire que `robot1` saura récupérer son `nom`, et ne le confondra pas avec celui de `robot2`.
