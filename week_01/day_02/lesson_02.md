# La librairie NumPy
Tu t'inquiétais de n'avoir toujours pas croisé de tableaux ? Rassure-toi, les tableaux NumPy sont dans la place 🤘🤘

## 1. Introduction
NumPy est une bibliothèque Python destinée à manipuler des matrices ou tableaux multidimensionnels ainsi que des fonctions mathématiques opérant sur ces tableaux. Dit comme ça, ça fait un peu peur mais en gros, dis toi que tu utiliseras NumPy quand tu travailleras avec des tableaux.

📌 *Utilité pour le projet* : 1/5<br/>
📊 *Utilité pour être Data Analyst* : 4/5<br/> 
💡 *Pourquoi cette ressource ?* : En fait, NumPy te sera très utile quand tu auras acquis de l'expérience (ou que tu feras de la data science) car de très gros tableaux (numpy arrays) sont plus efficaces que de très gros dataframes (pandas). Néanmois, la librairie est traditionnellement présentée en tout début de formation car tu dois l'importer si tu veux utiliser les opérateurs arithmétiques de base comme la moyenne, la racine carrée etc.

## 2. Historique et contexte
Comme on l'a déjà vu, le langage Python n'a pas été conçu à l'origine pour le calcul numérique. Cependant, il a très tôt attiré l'attention de la communauté scientifique et technique.

En 1995, le groupe d'intérêt spécial (SIG) *Matrix-sig* a été fondé dans le but de créer un paquet de calcul matriciel. Parmi ses membres, Guido van Rossum, concepteur et développeur de Python, a étendu sa syntaxe, et en particulier, la syntaxe d'indexation, afin de faciliter le calcul des tableaux. Une première implémentation d'un paquetage matriciel a été réalisée par Jim Fulton, puis améliorée par Jim Hugunin et appelée Numeric, également connue sous le nom de "Numerical Python extensions" ou "NumPy".

NumPy est la base de SciPy, regroupement de bibliothèques Python autour du calcul scientifique 💣💣

> Pour info, au cas où tu es largué dans ces histoires de calcul : le calcul scientifique est une discipline aux contours pas toujours franchement définis, mais qui regroupe un ensemble de champs mathématiques et informatiques permettant la simulation numérique des phénomènes de la physique, chimie, biologie, et sciences appliquées en général.

## 3. La ressource
On va découvrir ici à quoi la librairie NumPy va te servir.

A chaque fois que tu en auras besoin, n'oublie pas de l'importer au début de ton script : 

`import numpy as np`

### 3.1. Les tableaux multidimensionnels
Le principe fondamental de NumPy est l'apport de tableaux multidimensionnels.

Par définition, un tableau (ou *array*) en anglais est une structure de données constituée d’une collection d’éléments (du même type) identifiés par un index.

![Un exemple de tableau](https://codeforwin.org/wp-content/uploads/2015/07/array-and-array-index-representation.png)

L’image ci-dessus nous donne un exemple d’un tableau à 1 dimension. Ainsi, on parlera de tableaux multidimensionnels lorsqu’on aura au minimum deux dimensions 🙃 On peut définir la dimension d’un tableau comme le nombre d’indices (d’axes) nécessaires pour spécifier de manière unique un élément dans le tableau. 

![Les dimensions](https://www.w3resource.com/w3r_images/numpy-array-xyz-axis.png)

On voit ici des exemples de tableaux à une, deux et trois dimensions. *C’est un peu plus compliqué de représenter les dimensions supérieures à 3*.

>Attention, il ne faut pas confondre les listes et les tableaux. Contrairement aux listes en Python, les tableaux Numpy ne peuvent contenir des membres que d'un seul type. Par ailleurs, la grande différence entre ces deux structures de données se trouve au niveau des fonctions que vous pouvez leur appliquer. Par exemple, vous pouvez diviser un tableau (valeurs numériques) par 5, et chaque nombre dans le tableau sera divisé par 5 et vous aurez le résultat voulu. Cependant, si vous essayez de diviser une liste (valeurs numériques) par 5, l’interpréteur Python vous retournera une erreur.

Enfin, dis toi que tu vas pouvoir analyser beaucoup de choses en tant que tableaux de nombres. Par exemple, une image peut être considérée comme un tableau de deux dimensions (une matrice) où chaque nombre représente l'intensité lumineuse d'un pixel. 


### 3.2. Manipulations de tableaux

Regarde comment créer et manipuler des tableaux sur [ce cours d'introduction à NumPy](https://courspython.com/apprendre-numpy.html).

### 3.2. Intérêt des tableaux
Mais surtout le plus important est que tu comprennes l'intérêt de NumPy pour l'analyse de données.

Les éléments d'un tableau sont stockés dans des emplacements de mémoire contigus. En fait, l’idée de NumPy est de stocker plusieurs éléments du même type ensemble dans le but d’améliorer les performances de calcul.

Cela est très utile car les boucles peuvent êtres lentes en Python. Si vous voulez savoir pourquoi, l'idée principale est la suivante : l'implémentation de référence de Python, encore appelée CPython, est très flexible, mais cette flexibilité l'empêche d'utiliser toutes les optimisations possibles. Avec des boucles, il faudra plusieurs secondes pour accomplir un million d'opérations. Sachant que les processeurs actuels sont capables d'exécuter des milliards d'opérations par seconde, cette durée peut apparaître absurde. Ce délai est dû à toutes les opérations annexes que doit accomplir l'interprète, comme les appels de fonction et vérifications de type ⏳⏳⏳

___

🔧🔧 ASTUCE 🔧🔧

À chaque fois que tu te retrouves à utiliser une boucle pour effectuer une opération en Python, demande-toi si cette opération ne peut pas s'accomplir grâce à Numpy sans boucle.

___


## 4. Points importants à retenir
- NumPy permet une manipulation aisée et flexible des tableaux. 
- NumPy est important dans l'analyse de donnée pour sa redoutable efficacité. L’idée principale derrière les tableaux est de stocker plusieurs éléments du même type ensemble dans le but d’améliorer les performances de calcul.

## 5. Pour aller plus loin
La [documentation officielle](https://numpy.org/doc/stable/reference/).
