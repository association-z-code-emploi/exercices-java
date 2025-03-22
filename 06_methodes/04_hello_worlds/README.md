---
tags:
  - exercises
  - java
---

# Exercice 04 : Hello World**s** !

Ayons un aperçu des tableaux ("_arrays_") qui sont utilisés pour stocker plusieurs valeurs dans une seule variable, au lieu de déclarer des variables distinctes pour chaque valeur.

Il y aura un cours dédidé aux tableaux, mais en attendant, voyons comment en déclarer un et comment l'utiliser.

Pour déclarer un tableau, on définit le type de la variable avec des **crochets** puis on insère les valeurs, séparées par des virgules, entre accolades :

```java
String[] languages = {"Java", "PHP", "Javascript"};

int[] notes = {2, 15, 20, 7};
```

Pour accéder aux valeurs, il faut faire référence à son **index**, en appelant le nom du tableau et en indiquant cet index entre crochets :

```java
languages[0]; // un tableau commence toujours à 0
// "Java"

notes[2];
// "20"
```

Vous pouvez connaître la _longueur_ d'un tableau avec la propriété `length` :

```java
System.out.println(languages.length);
// "3" car il y a trois éléments dans le tableau "languages"

System.out.println(notes.length);
// "4" car il y a quatre éléments dans le tableau "notes"
```

Maintenant, rassemblons plusieurs éléments des exercices précédents pour filtrer un tableau de personnes en fonction de leurs rôles !

## Consignes

Créer une nouvelle classe `Greeting.java` et codez une méthode `sayHelloToPersons` qui prend en paramètre un **tableau de personnes** et qui _print_ pour chaque élément du tableau `"Hello, <personne>!"`.

Par exemple :

```java
sayHelloToPersons(persons);
/*
Hello, Jim!
Hello, Zack!
...
*/
```

## Conseil

On ne pourra pas toujours connaître le nombre d'éléments contenus dans un tableau. Il faudra donc trouver une astuce pour boucler sur le tableau, avec une condition d'arrêt qui se basera sur la longueur de ce tableau !
