---
tags:
  - exercises
  - java
---

# Exercice 02 : ajouter un scanner dans la soute

Maintenant que la soute est installée, vous allez pouvoir ajouter une fonctionnalité qui permettra de voir/revoir le contenu de la soute.

> ℹ️ Il est conseillé de créer un nouveau projet ou de vous assurer d'avoir des noms de classes `Spaceship` distincts pour ne pas coder que sur un seul fichier entre les exercices.

## Consignes

Dans un fichier `Spaceship.java`, copiez votre précédente classe `Cargo` et ajoutez une nouvelle méthode `searchStorage()`. Celle-ci prendra en paramètre d'entrée (d'*input*) une **String**, qui représentera la marchandise à retrouver. Cette méthode doit **retourner** un **nombre entier** qui représentera l'indice/l'emplacement dans la soute ; sinon retourner `null` dans le cas où on ne trouverait pas l'objet en question.

Reprenez ensuite votre classe `Spaceship` de l'exercice précédent (celle contenant votre méthode `main()`), pour toujours instancier un objet depuis la classe `Cargo` et appeler maintenant `searchStorage()` pour retrouver une marchandise. Affichez dans le terminal (depuis `main()`) d'une façon similaire à ci-dessous :

```java
// avec un tableau de marchandises contenant : Oxygen, Food, Water, Equipment et Weapons
// on veut chercher "Food"
System.out.println(mySpaceship.searchStorage("Food")); // Found at location: 2
// on veut chercher "BFG"
System.out.println(mySpaceship.searchStorage("BFG")); // Not found
...
```


## Conseils

- `null` est une valeur particulière qui peut se faire passer pour une autre ; n'essayez donc pas de mettre un type de retour `null` mais plutôt le type attendu "si tout se passait bien" et que l'on trouvait la marchandise.
- Vous pourriez aussi créer une méthode à l'intérieur de `main()` pour afficher plus facilement le résultat de la recherche ; cela vous de répéter évitera du code!
- Préparez-vous à de nouveau reporter ce nouveau code dans le dernier exercice !
