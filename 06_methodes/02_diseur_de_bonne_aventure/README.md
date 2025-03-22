---
tags:
  - exercises
  - java
---

# Exercice 02 : diseur de bonne aventure

Comme vous l'avez probablement remarqué durant le cours, la plus grande utilité d'une méthode est de pouvoir réutiliser un bloc de code qui s'adaptera aux valeurs qui lui sont données. Comme vous savez à quoi vous attendre en termes de type de valeurs d'entrée (les paramètres), vous allez pouvoir faire des calculs avec les arguments !

## Consignes

Créer une nouvelle classe `FortuneTeller.java` et codez deux méthodes :

- `calculateAge` qui prendra en paramètre deux **nombres** dans cet ordre d'entrée :

  - un âge
  - un nombre d'année

  Cette méthode doit _retourner_ l'âge après le nombre d'année donné.

  Par exemple, si vous entrez "32 ans" et "8 ans", alors la valeur de retour devrait être "40 ans".

  > ⚠️ L'exemple ci-dessus utilise des **string**, mais vous devrez utiliser des **nombres**.

- `tellFortune` qui prend en paramètre deux **string** et un **nombre** et qui va _print_ (ie. afficher dans le terminal) une courte phrase avec ces paramètres. Les paramètres doivent être (dans l'ordre d'entrée) :
  1. un prénom
  2. l'âge actuel ; le premier argument de `calculateAge`
  3. un métier
  4. le nombre d'année ; le second argument de `calculateAge`
  5. l'âge retourné par `calculateAge`

Le résultat doit être : `"Vous êtes <1>, <2> ans, et vous serez <3> dans <4> ans. Vous aurez donc <5> ans."`

> "X" doit donc être un calcul avec l'âge après le nombre d'année choisi.

Un exemple d'output :

```shell
"Vous êtes Jim, 32 ans, et vous serez développeur web dans 2 ans. Vous aurez donc 34 ans."

"Vous êtes Sacha, 10 ans, et vous serez le meilleur dresseur dans 25 ans. Vous aurez donc 30 ans."
```
