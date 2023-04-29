# [Git](https://git-scm.com/book/fr/v2)

<center>
<img src="img/git-logo-white.png" alt="Javascript Logo" width="150">
</center>

<br>

Par **Rachid EDJEKOUANE ⭐️**

---

## Sommaire

1. **[Introduction à Php](#module-1--introduction-a-php)**
2. **[Fonctions, tableaux et manipulation de fichiers](#module-2--fonctions-tableaux-et-manipulation-de-fichiers)**
3. **[Gestion des formulaires et des sessions](#module-3--gestion-des-formulaires-et-des-sessions)**
4. **[Bases de données avec PHP et MySQL](#module-4--bases-de-données-avec-php-et-mysql)**
5. **[Introduction aux frameworks PHP et déploiement)](#module-5--introduction-aux-frameworks-php-et-déploiement)**

<br>

---

### On initialise un nom + email, qu'on peut modifier à tout moment avec :

<br>

-   git config --global user.name "John doe"
-   git config --global user.email "johndoe@gmail.com"

<br>

---

### On initialise un dépôt avec :

<br>

-   git init

<br>

---

### On s'informe du statut de notre dépôt, par rapport aux fichiers ajoutés/modifiés avec :

<br>

-   git status

<br>

---

### On rajoute les fichiers dans une zone de transit avec :

<br>

-   git add index.html

<br>

---

### On sauvegarde l'état du dossier avec un commit :

<br>

-   git commit -m "Ajout de xxx"

<br>

---

### On regarde l'historique des commits (des sauvegardes) :

<br>

-   git commit -m "Ajout de xxx"

<br>

---

### Pour rattraper un commit dans lequel on aurait oublié d'intégrer un fichier, on ajoute d'abord le ou les fichiers oubliés :

<br>

-   git commit --amend

<br>

---

## Git branch

<br>

### Pour lister les branches :

<br>

-   git branch

<br>

---

### Pour créer une branche :

<br>

-   git branch maBranche

<br>

---

<br>

### Pour se déplacer sur une branche

<br>

-   git switch maBranche

<br>

---

<br>

### Afin de créer une branche et de se déplacer dessus intantanément, on éxécute :

<br>

-   git switch -c maBranche

<br>

---

<br>

### Lorsqu'on veut changer le nom d'une branche, on navigue dessus, puis on lance :

<br>

-   git branch -m changementDeNom

<br>

---

<br>

### Pour faire fusionner une ou plusieurs branches, on se déplace d'abord sur la branche qu'on veut fusionner avec une autre puis :

<br>

-   git merge autreBranche

<br>

`De base, vous pouvez tomber sur trois types de fusion :`

`Fusion simple "Fast Forward", les historiques de commits se lient sans conflit, car il y avait des changements seulement sur une branche.`

`Fusion par récursion, lorsque il y a des commits différents sur plusieurs branches qu'on "merge", mais que ces commits ne rentrent pas en conflit.`

`Fusion avec conflit, lorsqu'il y a des commits différents sur plusieurs branches que l'on "merge" et que ces commits modifient des choses similaires(ajout de code à la même ligne, changement du code initial, supression de fichiers) .`

<br>

---

<br>

### Afin de supprimer une branche, on doit se situer sur une branche différente de celle qu'on veut supprimer, puis :

<br>

-   git branch -d maBranche

<br>

---

<br>

**[⬆ haut de page](#)**
