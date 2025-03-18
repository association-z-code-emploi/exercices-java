---
tags:
  - exercises
  - java
---

# Exercice 06 : vos papiers s'il vous plait

Jusqu'à présent, vous avez pu écrire des conditions qui vérifient des valeurs figées, ou _hard codées_.
Et si on laissait l'utilisateur directement nous indiquer la valeur qui devra être testée ?

En Java offre la méthode `scanner` qui va nous permettre de récupérer une valeur d'entrée (appelée plus couramment un _input_).

**Exemple** : pour afficher la saisie d'un utilisateur

```java
import java.util.Scanner; // permet d'utiliser la méthode pour récupérer une saisie au clavier de l'utilisateur

public class Exemple {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in); // va permettre d'utiliser la méthode de saisie
        String word;

        System.out.print("Entrez un mot : "); // ce qui va s'afficher dans le terminal avant de laisser l'utilisateur écrire sa réponse et la valider avec la touche "Entrée"
        word = scanner();

        scanner.close(); // il faudra TOUJOURS fermer le scanner après utilisation, sans quoi votre programme n'arrive plus à correctement s'arrêter
    }
}
```

## Consignes

Créer une classe `PapersPlease.java` et récupérez l'âge de l'utilisateur.

Codez ensuite une condition qui permettra de vérifier et d'afficher si la personne est majeure ou non.

## Conseil

Quel est le type de la valeur récupérée par `scanner` ? Il faudra peut-être trouver un moyen de changer le type de cette valeur pour la passer ensuite dans la condition... Si seulement il existait [une liste qui référence toutes les méthodes de `scanner`](https://www.w3schools.com/java/java_ref_scanner.asp) !
