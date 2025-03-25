---
tags:
  - exercises
  - java
---

# Exercice 04 : guichet automatique

## Consignes

Créez une classe `BankAccount` avec :

- un **attribut** `balance` (nombre à virgule)
- une **méthode** `deposit()` (nombre à virgule ; qui ne peut pas être modifié depuis la méthode) qui ajoute un montant au solde
- une **méthode** `withdraw()` (nombre à virgule ; qui ne peut pas être modifié depuis la méthode) qui retire un montant si le solde est suffisant
- une **méthode** `displayBalance()` qui affiche "Actual balance : X €"

Dans `main()`, créez un compte, faite quelques opérations et affichez le solde final.

## Conseils

- Il n'est pas nécessaire d'utiliser `Scanner` ; quoi que cela semble logique, mais vous aurez d'autres occasions de l'utiliser !
- Il faudra penser à afficher un message en cas de solde insuffisant lors de la méthode `withdraw()`.
