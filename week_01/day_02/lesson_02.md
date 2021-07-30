# La librairie NumPy
Tu t'inquiétais de n'avoir toujours pas croisé de tableaux ? Rassure-toi, les tableaux NumPy sont dans la place 🤘🤘

## 1. Introduction
NumPy est une bibliothèque Python destinée à manipuler des matrices ou tableaux multidimensionnels ainsi que des fonctions mathématiques opérant sur ces tableaux. Dit comme ça, ça fait un peu peur mais en gros, dis toi que tu utiliseras NumPy quand tu travailleras avec des tableaux.

## 2.Historique et contexte
Comme on l'a déjà vu, le langage Python n'a pas été conçu à l'origine pour le calcul numérique. Cependant, il a très tôt attiré l'attention de la communauté scientifique et technique.

En 1995, le groupe d'intérêt spécial (SIG) *Matrix-sig* a été fondé dans le but de créer un paquet de calcul matriciel. Parmi ses membres, Guido van Rossum, concepteur et développeur de Python, a étendu sa syntaxe, et en particulier, la syntaxe d'indexation, afin de faciliter le calcul des tableaux. Une première implémentation d'un paquetage matriciel a été réalisée par Jim Fulton, puis amélioré par Jim Hugunin et appelée Numeric, également connu sous le nom de "Numerical Python extensions" ou "NumPy".

NumPy est la base de SciPy, regroupement de bibliothèques Python autour du calcul scientifique 💣💣.

> Pour info, au cas où tu es largué dans ces histoires de calcul : le calcul scientifique est une discipline aux contours pas toujours franchement définis, mais qui regroupe un ensemble de champs mathématiques et informatiques permettant la simulation numérique des phénomènes de la physique, chimie, biologie, et sciences appliquées en général.

## 3. La ressource
On va découvrir ici à quoi la librairie NumPy va te servir.

A chaque fois que tu en auras besoin, n'oublie pas de l'importer au début de ton script : 

`import numpy as np`

### 3.1. Les tableaux multidimensionnels
Le principe fondamental de NumPy est l'apport de tableaux multidimensionnels.

Par définition, un tableau (ou *array*) en anglais est une structure de données constituée d’une collection d’éléments (du même type) identifiés par un index.

![Un exemple de tableau](https://codeforwin.org/wp-content/uploads/2015/07/array-and-array-index-representation.png)

L’image ci-dessus nous donne un exemple d’un tableau à 1 dimension. Ainsi, on parlera de tableaux multidimensionnels lorsqu’on aura au minimum deux dimensions 🙃. On peut définir la dimension d’un tableau comme le nombre d’indices (d’axes) nécessaires pour spécifier de manière unique un élément dans le tableau. 

![Les dimensions](https://www.w3resource.com/w3r_images/numpy-array-xyz-axis.png)

On voit ici des exemples de tableaux à une, deux et trois dimensions. *C’est un peu plus compliqué de représenter les dimensions supérieures à 3*.


>Attention, il ne faut pas confondre les listes et les tableaux. Contrairement aux listes en Python, les tableaux Numpy ne peuvent contenir des membres que d'un seul type. Par ailleurs, la grande différence entre ces deux structures de données se trouve au niveau des fonctions que vous pouvez leur appliquer. Par exemple, vous pouvez diviser un tableau (valeurs numériques) par 5, et chaque nombre dans le tableau sera divisé par 5 et vous aurez le résultat voulu. Cependant, si vous essayez de diviser une liste (valeurs numériques) par 5, l’interpréteur Python vous retournera une erreur.

Enfin, les attributs principaux d'un tablea sont les type de données (dtype), l'allure (shape), la taille (size), la taille de l'élément (itemsize), la donnée (data) et la dimension N (ndim). 

### 3.2. Manipulations de tableaux
blabla

### 3.2. Intérêt des tableaux



## 4. Points importants à retenir
NumPy permet une manipulation aisée et flexible des tableaux. Nous n'avons qu'effleurer la surface de cette fabuleuse librairie Python. NumPy contient davantage de caractéristiques à étudier pour sa redoutable efficacité. 

Les éléments du tableau sont stockés dans des emplacements de mémoire contigus. L’idée est de stocker plusieurs éléments du même type ensemble dans le but d’améliorer les performances de calcul.

## 5. Pour aller plus loin
Il existe aussi un guide complet sur ce sujet par le concepteur de NumPy lui-mêm : Guide to NumPy.
