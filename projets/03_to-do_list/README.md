---
tags:
  - exercises
  - java
---

# Projet 03 : to-do list tracker

## Consignes

Dans ce projet, vous créer une **application en ligne de commande ("CLI")** en Java pour gérer une **liste de tâche ("to-do list")**. Cette application permettra de suivre ce que l'on doit faire, ce que l'on a déjà fait et ce sur quoi on travaille actuellement.

## Notions abordées

Vous trouverez la liste complète des notions abordées ci-dessous, ce qui devrait vous donner des indices sur quelles fonctionnalités faire, et les mots-clés pour effectuer des recherches si besoin :

- manipuler des fichiers (lecture, écriture, création sous condition)
- récupérer un input utilisateur en CLI
- traiter des arguments en CLI
- utilisation de JSON
- gestion du temps et des dates
- gestion d'erreurs et des cas limites
- utilisation d'identifiant unique
- séparation des responsabilité (ne regroupez pas tout dans une seule classe ou un seul fichier)

## Fonctionnalités attendues

Votre application devra :

- ajouter, modifier (et optionnellement) supprimer une tâche

- marquer une tâche comme "en cours" ou "terminée"

- lister toutes les tâches

- (optionnellement) lister uniquement les tâches :
  - terminées
  - non-terminées
  - en cours

## Structure d'une tâche

Chaque tâche devra contenir les propriétés suivantes dans le fichier JSON :
- `id` : identifiant unique de la tâche
- `description` : description courte de la tâche
- `status` : statut actuel (`todo`, `in-progress`, `done`)
- `createdAt` : date et heure de création
- `updatedAt` : date et heure de dernière modification

## Contraintes

- Ce programme doit être **exécutable depuis la ligne de commande**
- Les **arguments doivent être passés en ligne de commande** (pas via des menus interactifs)
- Les données doivent être stockées dans **un fichier JSON dans le dossier courant** ; créer ce fichier s'il n'existe pas lors de la première éxecution du programme
- Pas de bibliothèques externes : que des **méthodes natives de Java** pour et écrire dans le fichier
- Gérer correctement les **erreurs et cas limites** (eg. tâche inexistante lors d'une demande de modification, argument manquant, etc...)

## Exemple de commandes (CLI)

```shell
# ajouter une tâche
task-cli add "Faire les bagages"
# → Task successfully added (ID: 1)
task-cli add "Ranger la maison"
# → Task successfully added (ID: 2)
task-cli add "Laisser le chat chez le voisin"
# → Task successfully added (ID: 2)

# mettre à jour une tâche
task-cli update 1 "Faire les bagages et prendre le passeport"
# → Task successfully updated (ID: 1)

# indiquer le statut d'une tâche comme en cours
task-cli mark-in-progress 1
# → Task successfully marked as in-progress (ID: 1)

# indiquer le statut d'une tâche comme terminée
task-cli mark-done 2
# → Task successfully marked as done (ID: 2)

# lister toutes les tâches
task-cli list
# ↴
# Faire les bagages et prendre le passeport (in-progress)
# Ranger la maison (done)
# Laisser le chat chez le voisin (to do)
```

## Conseils pour réaliser ce projet

Si vous vous sentez submergé, voici une découpage par étape en pseudo-code :

1. Lire les arguments donnés dans la CLI
2. Charger le fichier JSON contenant les tâches ; si le fichier n'existe pas, le créer avec une liste vide
3. Définir une classe ou une structure pour représenter une tâche comme indiquée dans [Structure d'une tâche](#structure-dune-tâche) :
  - id
  - description
  - status
  - createdAt
  - updatedAt
4. Selon la commande, exécuter l'action correspondante :
  - si `add` :
    - créer une nouvelle tâche avec un id unique
    - ajouter la tâche à la liste
    - sauvegarder la liste dans le fichier JSON
  - si `update` :
    - rechercher la tâche par id
    - modifier la description
    - mettre à jour la date de modification
    - sauvegarder les changements
  - etc...
5. Gérer les erreurs :
  - fichier introuvable
  - tâche inexistante
  - mauvais arguments
  - etc...
6. Sauvegarder à chaque modifiction dans le fichier JSON
7. Optionnel :
  - ajouter les actions de listes selon le statut, supprimer une tâche, etc...
  - ajouter des messages utilisateurs clairs pour action réussie ou erreur rencontrée
  - ajouter un fichier "error-logs" listant toutes les erreurs rencontrées par l'utilisateur, avec la date et le message correspondant
