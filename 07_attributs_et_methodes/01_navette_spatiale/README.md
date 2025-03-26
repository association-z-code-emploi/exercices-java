---
tags:
  - exercises
  - java
---

# Exercice 01 : Navette spatiale

Imaginons une navette spatiale ... mais dont l'interface utilisateur manque encore de pas mal de fonctionnalités. Commençons par afficher ses informations grâce à des **méthodes** !

## Consignes

Créez une classe `Spaceship`, avec les **attributs** suivants :

- `name` qui sera une **string**
- `model` qui sera aussi une **string**

Ajoutez deux **méthodes** :

- `greeting()` qui affichera `"Welcome aboard, Captain!"`
- `displayInfos()` qui affichera les informations de la navette

Créez ensuite une **instance de cette classe**, puis appelez ces deux méthode pour un résultat comme celui-ci dans le terminal :

```
"Welcome aboard, Captain!"
"The Kestrel (Kestrel A) is at your service."
```

## Conseils

- N'oubliez pas d'utiliser un constructeur pour plus facilement créer un nouvel objet de `Spaceship`.
- Vous n'êtes -pour le moment- pas obligé à utiliser des **paramètres** dans les méthodes : vous pouvez directement appeler et utiliser les **attributs** de vos objets.
