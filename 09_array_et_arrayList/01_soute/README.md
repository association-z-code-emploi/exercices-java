---
tags:
  - exercises
  - java
---

# Exercice 01 : ajouter une soute à la navette spatiale

Vous aviez commencé à coder l'interface d'une navette spatiale dans un précédent exercice. On y retourne pour ajouter de nouvelles fonctionnalités comme une gestion du stockage de la soute ! Mais avant ça, reprenons la base de cette navette, que vous l'ayez déjà fait ou non.

## Consignes

Dans un fichier `Spaceship.java`, créer une classe `Cargo` avec :

- un attribut `storage` qui sera un **tableau de String**, pour représenter les marchandises stockées dans la soute
- une méthode `displayStorage()`, qui utilisera et affichera chaque élément de `storage`, sous forme de liste ordonnée dans le terminal, comme indiqué plus bas
- un constructeur avec `storage`

Créez ensuite une classe `Spaceship` qui contiendra votre méthode `main()`, pour instancier un objet depuis la classe `Cargo` et appeler sa méthode `displayStorage()` :

```shell
1. Oxygen
2. Food
3. Water
4. Equipment
5. Weapons
...
```


## Conseils

- Quelle devrait-être le modificateur d'accès de `storage`, pour éviter d'être accessible de partout ?
- La longueur du tableau `storage` n'est pas importante - pour le moment.
- Plot twist : vous allez réutiliser ce code lors du prochain exercice ! Assurez-vous qu'il fonctionne comme demandé.
