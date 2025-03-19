---
tags:
  - exercises
  - java
---

# Exercice 08 : s'échapper de l'hotel infini !

L'[Hôtel de Hilbert](https://fr.wikipedia.org/wiki/H%C3%B4tel_de_Hilbert) est une paradoxe sur les ensembles infinis en mathématique ... mais ici, c'est simplement une excuse pour coder une boucle infinie, et en sortir avec `break` !

## Consignes

Codez dans la classe `InfiniteHotel.java` qui est fourni dans ce dossier et initialisez une variable à 0 (nombre) qui représentera le dernier numéro de chambre visitée.

Utilisez ensuite la boucle `while` déjà présente : celle-ci ne s'arrêtera jamais d'elle-même puisque "vrai" est toujours "vrai" !

Permettez à l'utilisateur de choisir jusqu'à quelle chambre aller ; en commençant par la 1, puis la 2, etc...

Affichez enfin un message dans le terminal lorsqu'on "sort de l'hôtel" indemne.

## Conseil

Dans votre terminal, faîtes Ctrl+C pour terminer prématurément l'exécution de votre code si vous ne le voyez pas s'arrêter : votre boucle n'a pas trouvé de condition d'arrêt et est devenue infinie !
