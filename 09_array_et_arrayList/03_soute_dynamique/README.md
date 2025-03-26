---
tags:
  - exercises
  - java
---

# Exercice 03 : gérer une marchandise dans la soute

Évidemment, durant votre voyage, vous allez ajouter ou retirer du contenu dans votre soute. Ne vous souciez pas de sa capacité maximale ; ce sera peut-être pour un futur exercice !

## Consignes

Dans un fichier `Spaceship.java`, copiez votre précédente classe `Cargo` et ajoutez trois nouvelles méthodes pour gérer le stockage :

- `addItem()` pour ajouter une marchandise à la soute :
  - prend en paramètre une **String**
  - affiche un message confirmant l’ajout et l’emplacement utilisé
- `switchItem()` pour remplacer un objet existant par un autre à l’emplacement donné :
  - prend en paramètre un **nombre entier** pour l'indice concerné et une **String** pour le nouvel objet
  - si l’emplacement est vide, ajoute l’objet à la suite grâce à `addItem()`
  - affiche un message indiquant l’échange ou l’ajout d’un nouvel objet
- `removeItem()` pour supprimer un objet de la soute s’il existe :
  - affiche un message confirmant la suppression ou indique si l’objet est introuvable

Reprenez ensuite votre classe `Spaceship` de l'exercice précédent (celle contenant votre méthode `main()`), pour utilisez ces nouvelles méthodes et affichez les résultats dans le terminal, comme dans l’exemple ci-dessous :

```java
// affichage de la soute :
mySpaceship.displayStorage();
/*
1. Oxygen
2. Food
3. Water
4. Scraps
5. Loot
*/

// ajout :
mySpaceship.addItem("Laser"); // "Laser added at location: 6"
//                                                         ↑ et non pas 5 comme son indice,
//                                                         car on veut que ce soit lisible
//                                                         pour des "humains non-devs"

// modifier :
mySpaceship.switchItem(5, "BFG"); // "Laser switched with BFG at location: 6"
mySpaceship.switchItem(10, "Escape pod"); // "Free space : Escape pod added at location 7"

// supprimer :
mySpaceship.removeItem("Scraps"); // "Scraps removed at location: 3"

// affichage de la soute :
mySpaceship.displayStorage();
/*
1. Oxygen
2. Food
3. Water
4. BFG
5. Laser
6. Escape pod
*/
```

## Conseil

`Array` ne permettant pas de modifier la longueur d'un tableau, il faudra passer par *un autre type de tableau*.
