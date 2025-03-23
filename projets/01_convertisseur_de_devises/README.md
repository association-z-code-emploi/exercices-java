---
tags:
  - exercises
  - java
---

# Projet 01 : convertisseur de devises

Dans ce premier projet, vous allez pouvoir mettre en pratique l'ensemble des notions vues durant les premiers cours : des **variabdes**, des **types de données**, des **opérateurs**, des **conditions**, et des **boucles**.

Vous allez programmer un convertisseur de devises. Il devra permettre à un utilisateur de convertir un montant d'une devise vers une autre parmi trois choix possibles : **Euros** (_EUR_), **Dollars** (_USD_) et **Livres Sterling** (_GBP_). La saisie de l'utilisateur se fera avec la méthode pré-définie `Scanner`.

## Consignes

### Fonctionnalités attendues (dans l'ordre d'exécution)

1. Sélection d'une devise entrante : un utilisateur doit entrer "EUR", "USD" ou "GBP"

2. Saisie du montant : l'utilisateur entre un montant positif (décimal possible)

3. Sélection de la devise sortante : l'utilisateur choisit une devise différente de celle d'entrée

4. Conversion et affichage du résultat : le montant converti s'affiche avec 2 décimales

5. Nouvelle opération : l'utilsateur peut choisir de refaire une conversion ou de quitter

6. Option de sortie à tout moment en tapant "Exit" pour quitter le programme

### Contraintes

- Si une saisie est invalide (dévise incorrecte, montant négatif, devise sortante identique à l'entrante, ...) : il faudra redemander l'entrée jusqu'à obtenir une réponse correcte. Vous ne devez pas recommencer tout le programme après une erreur.

- Le programme doit être écrit dans une seulle classe.

## Conseils

- Lisez et relisez bien les consignes
- Prenez le temps de prendre des notes si nécessaires, ou de faire du pseudo-code
- Donnez des noms clairs à vos variables
- Testez régulièrement ; et faites une pause si vous coincez depuis un moment !
- Faîtes attention aux boucles infinies : n'oubliez pas de faire Ctrl+C dans le terminal pour arrêter de force votre programme
- Quelque chose n'est pas indiqué et vous avez un doute ? Réfléchissez à ce qui vous semble être logique et utile pour l'utilisateur : faut-il absolument écrire la devise en majuscule ou peut-on accepter un mix ? comment indiquer à l'utilisateur qu'il a fait une erreur ?

> ℹ️ Pour convertir une devise vers une autre, vous devrez multiplier le montant par un taux de conversion selon les devises concernées :
>
> - EUR → USD = 1,10
> - EUR → GBP = 0,85
> - USD → EUR = 0,91
> - USD → GBP = 0,77
> - GBP → EUR = 1,18
> - GBP → USD = 1,30
