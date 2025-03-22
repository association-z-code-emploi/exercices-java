---
tags:
  - exercises
  - java
---

# Exercice 05 : préparer une navette spatiale

Qui ne rêve pas au moins une fois d'aller dans l'Espace ? Rêvons un peu plus et préparons une navette spatiale pour son décollage ... dans le terminal !

## Consignes

Créer une nouvelle classe `Spaceship.java` et codez deux méthodes :

- `checkFuelLevel` qui prend en paramètre un **nombre entier** et qui _retourne_ une **string** en fonction du niveau de carburant :
  - si le niveau de carburant est supérieur à 20, vous êtes dans le "vert"
  - si le niveau de carburant est comprise entre 10 et 19, vous recevez un avertissement
  - si le niveau de carburant est inférieur à 10, vous recevez une alerte

Par exemple :

```java
String fullFuelLevel = checkFuelLevel(30); // "Fuel level: green"
String midFuelLevel = checkFuelLevel(12); // "Fuel level: yellow"
String lowFuelLevel = checkFuelLevel(1); // "Fuel level: red"
```

- `checkCargoHold` qui prend en paramètre un **tableau de string** et qui _retourne_ une **string** en fonction de l'espace restant :
  - si la cargaison contient quatre articles, vous êtes plein
  - si la cargaison contient moins que quatre articles, affichez le nombre de place restant
  - si la cargaison contient plus que quatre articles, alertez avec le nombre de place qui doivent être libérées

Par exemple :

```java
String fullCargo = checkCargoHold([<4 articles>]); // "Cargo: full"
String spaciouxCargo = checkCargoHold([<1 article>]); // "Cargo : 3 available spaces"
String overfullCargo = checkCargoHold([<8 articles>]); // "Cargo: over capacity by 4 items"
```

## Conseils

- N'oubliez pas de retourner les valeurs : vous les afficherez seulement lorsqu'elles "sortiront" des méthodes appelées.
- Appliquez-vous avec cet exercice : il n'est pas dit qu'on ne puisse pas bientôt faire décoller cette navette ...
