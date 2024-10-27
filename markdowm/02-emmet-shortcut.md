# [Emmet](https://emmet.io/)

<center>
<img src="./img/emmet.png" alt="Emmet logo" width="100">
</center>

> Emmet est un moteur d’autocomplétion intégré à Visual Studio Code qui permet d’accélérer votre production de code grâce à une syntaxe raccourcie.

Par **Rachid EDJEKOUANE ⭐️**

---

## Sommaire

1. **[Insérer le code de base d'une page HTML](#1-insérer-le-code-de-base-d-une-page-html)**
2. **[Insérer une balise](#2-insérer-une-balise)**
3. **[Créer une balise qui a une ou des classes](#3-créer-une-balise-qui-a-une-ou-des-classes)**
4. **[Créer plusieurs éléments qui se suivent](#4-créer-plusieurs-éléments-qui-se-suivent)**
5. **[Imbriquer des éléments](#5-imbriquer-des-éléments)**
6. **[Multiplier des éléments](#6-multiplier-des-éléments)**
7. **[Insérer du texte](#7-insérer-du-texte)**

---

### 1. Insérer le code de base d' une page HTML

_Si vous souhaitez ajouter le squelette de base d'une page HTML, vous tapez un point d'exclamation puis entrée._

```emmet
!
```

---

### 2. Insérer une balise

_Si vous souhaitez ajouter une balise seule, par exemple une "div", vous tapez son nom puis entrée._

```emmet
div
```

---

### 3. Créer une balise qui a une ou des classes

_Si notre div doit comporter un attribut "class", nous allons l'inclure de la même façon lors de la saisie._

```emmet
p.le-nom-de-ma-class
```

---

### 4. Créer plusieurs éléments qui se suivent

_Si nous souhaitons créer 3 sections qui auront des classes différentes, nous pouvons les enchainer au moyen du "+" qui, ici, signifiera "suivant"_

```emmet
h2+p+a
```

---

### 5. Imbriquer des éléments

_Si un élément doit être créé à l'intérieur d'un autre élément, nous pourrons, comme en CSS, utiliser le symbole ">"_

```emmet
div>p
```

---

### 6. Multiplier des éléments

_Si un élément doit être créé plusieurs fois, nous pourrons utiliser le symbole "\*"_

```emmet
li*3
```

---

### 7. Insérer du texte

_Dans l'exemple précédent nous n'avons pas mis le texte, nous pouvons le faire en l'ajoutant entre accolades "{texte}"_

```emmet
p.le-nom-de-ma-class{coucou}
```

---

**[⬆ retour au sommaire](#)**
