# [Git](https://git-scm.com/book/fr/v2)

<center>
<img src="img/git-logo-white.png" alt="Javascript Logo" width="150">
</center>

<br>

Par **Rachid EDJEKOUANE ⭐️**

---

## Sommaire

1. **[Initialisation](#1-initialisation)**
2. **[Commande de base](#2-commande-de-base)**
3. **[Git branch](#3-git-branch)**
4. **[Git checkout](#4-checkout)**
5. **[Tags](#5-nous-pouvons-créer-des-tags-pour-mieux-nous-repérer)**

<br>

---

## 1. Initialisation

### On initialise un nom + email, qu'on peut modifier à tout moment avec :

-   git config --global user.name "John doe"
-   git config --global user.email "johndoe@gmail.com"

<br>

### On initialise un dépôt avec :

-   git init

<br>

---

## 2. Commande de base

### On s'informe du statut de notre dépôt, par rapport aux fichiers ajoutés/modifiés avec :

-   git status

<br>

### On rajoute les fichiers dans une zone de transit avec :

-   git add index.html

<br>

### On sauvegarde l'état du dossier avec un commit :

-   git commit -m "Ajout de xxx"

<br>

### On regarde l'historique des commits (des sauvegardes) :

-   git log

<br>

### Pour rattraper un commit dans lequel on aurait oublié d'intégrer un fichier, on ajoute d'abord le ou les fichiers oubliés :

-   git commit --amend

<br>

### Afin de visualiser les changements qui ont eu lieu dans les fichiers modifiés, on peut éxécuter :

-   git diff

<br>

---

## 3. Git branch

### Pour lister les branches :

-   git branch

<br>

### Pour créer une branche :

-   git branch maBranche

<br>

### Pour se déplacer sur une branche

-   git switch maBranche

<br>

### Afin de créer une branche et de se déplacer dessus intantanément, on éxécute :

-   git switch -c maBranche

<br>

### Lorsqu'on veut changer le nom d'une branche, on navigue dessus, puis on lance :

-   git branch -m changementDeNom

<br>

### Pour faire fusionner une ou plusieurs branches, on se déplace d'abord sur la branche qu'on veut fusionner avec une autre puis :

-   git merge autreBranche

<br>

### Afin de supprimer une branche, on doit se situer sur une branche différente de celle qu'on veut supprimer, puis :

-   git branch -d maBranche

<br>

_De base, vous pouvez tomber sur trois types de fusion :_

_Fusion simple "Fast Forward", les historiques de commits se lient sans conflit, car il y avait des changements seulement sur une branche._

_Fusion par récursion, lorsque il y a des commits différents sur plusieurs branches qu'on "merge", mais que ces commits ne rentrent pas en conflit._

_Fusion avec conflit, lorsqu'il y a des commits différents sur plusieurs branches que l'on "merge" et que ces commits modifient des choses similaires(ajout de code à la même ligne, changement du code initial, supression de fichiers) ._

<br>

---

## 4. Checkout

### Nous avons vu que nous pouvons également nous déplacer parmi les commits avec checkout :

-   git checkout idDeCommit(ex: 45645645)

<br>

### Pour revenir en haut de la liste de commits, nous pouvons faire au choix :

-   git switch nomDeLaBrancheEnCours

-   git checkout nomDeLaBrancheEnCours

<br>

---

## 5. Nous pouvons créer des Tags pour mieux nous repérer

### On se déplace d'abord sur le commit que l'on veut "taguer", puis :

-   git tag nomDuTag

<br>

### Nous pouvons désormais nous déplacer vers le commit du tag correspondant :

-   git checkout nomDuTag

<br>

### Nous pouvons visualiser la liste de tags :

-   git tag

<br>

### Nous pouvons supprimer un tag :

-   git tag -d nomDuTag

<br>

---

## 6. Reset et Restore

### Si on a effectué des changements et qu'ils ne nous plaisent plus :

-   git restore nomDuFichier

_Cela permet de rapidement remettre à zéro un fichier sur lequel on travaillait, ça ne veut pas dire que le fichier sera forcement vide, il reaffiche simplement le contenu du commit sur lequel on se trouve._

<br>

### Nous pouvons également supprimé les fichiers en zone de transit avec :

-   git restore --staged index.html

<br>

### Pour afficher l'historique de commits sur une ligne :

- git log --oneline

<br>

### Pour supprimer des commits jusqu'à un commit passé :

- git reset idCommit

<br>

### Pour supprimer des commits jusqu'à un commit passé tout en supprimant les changements qu'il peuvent avoir été éffectués :

- git reset --hard idCommit

<br>


### Pour sauter un ou des commits et atterir dans un nouveau commit contenant le contenu d'un ancien commit :

- git revert idDuCommitÀRetrouver

<br>

---

## 7. Cherry-pick

### Pour intégrer seulement un commit ou des commits qui nous intéressent mais pas une branche entière :

- git cherry-pick idDuCommit

<br>

---

**[⬆ retour au sommaire](#)**
