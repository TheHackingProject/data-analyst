# Découvrir Python

C'est le moment de faire tes gammes en Python. Accroche-toi bien car dans la data, Python est indispensable !

## 1. Introduction
Sans transition aucune, on se lance ! Comment ça marche Python ? Est-ce que c'est si intuitif que ça ? Quels objets vais-je utiliser en Python ? 

Allons découvrir tout cela 🐣 🐣 ☕️☕️  !

## 2. La ressource
Pour bien comprendre les bases de Python, nous te demandons de suivre le cours OpenClassrooms [Initiez-vous à Python pour l'analyse de données](https://openclassrooms.com/fr/courses/6204541-initiez-vous-a-python-pour-lanalyse-de-donnees).
Ce cours est très bien fait et il est très adapté au niveau débutant.

N'hésite pas à prendre deux heures entières pour faire les 3 premiers chapitres (en réalisant les exercices sur ton Notebook et les quizz). Tu peux t'arrêter avant *Prenez en main les modules et librairies Python* car c'est le programme de la journée de demain.

### 2.1. Jupyter Notebook et Anaconda
Pour ton environnement de développement, nous te recommandons fortement de suivre ce que préconise le cours, c'est-à-dire télécharger Anaconda et utiliser Jupyter Notebook.

Plusieurs outils différents permettent de coder en Python, notamment les IDE populaires comme Pycharm, Spyder, ou encore Visual Studio.
>Un IDE (ou environnement intégré de développement) est un ensemble d'outils pour augmenter la productivité des programmeurs qui développent des logiciels.

Mais pour débuter et avoir un environnement Python complet et prêt à l’emploi, **l’idéal est d’installer la distribution Anaconda**. 

>*Anaconda Individual Edition* est une plateforme de distribution Python recensant plus de 20 millions d’utilisateurs dans le monde, basé sur un écosystème totalement open-source.

En téléchargeant Anaconda, tu bénéficieras à la fois de : 
- une installation de Python
- les packages de data science tels que Numpy, Pandas, Scikit-learn …
- des IDE de dernière génération tels que Jupyter (JupyterLab et Jupyter Notebooks) ou Spyder
- l’outil Conda pour gérer les environnements et les répertoires de packages.

*Quant à Jupyter, de quoi s'agit-il ?*

Créé à partir de Python en 2014, **Jupyter est un notebook de calcul** (computational notebook) open source, gratuit et interactif. 
Avec cet outil, il est possible de visualiser le code et de l’exécuter depuis la même interface utilisateur. On peut même apporter des changements au code et vérifier les résultats de ces modifications instantanément. Des données peuvent également être ajoutées.
**Enfin, cet outil permet de combiner  du code, des équations, des visualisations ou du texte**. Pour cette raison, il s’agit d’un outil idéal et très utile pour les Data Analysts et les Data Scientists.

C'est assez facile de prendre en main Jupyter Notebook mais si tu veux intégrer les fonctionnalités principales, je t'invite à lire ce [guide rapide d'utilisation](https://pyspc.readthedocs.io/fr/latest/03-guide/).


### 3.2. Types de variables et fonctions
Cf. chapitre 2 du cours OpenClassrooms

>Un type est une information sur le contenu de la variable qui indique à l'interpréteur Python la manière de manipuler cette information. 

Il existe plusieurs types de variables pour stocker les éléments en Python : 
- les types numériques : qui peuvent être des nombres entiers `int` ou des nombres réels `float`. Ex : `x = 3` ou `y = 3.5` ;
- les booléens `boolean` : sont le résultat d'opérations logiques et ont deux valeurs possibles : `True` ou `False`. Ex : `x = 4 < 5` ;
- les chaînes de caractères `string` : qui permettent de stocker du texte. Ex : `x = "Hello world"` ;
- les listes `list` : un tableau ordonné, où chaque élément est associé à un indice. Ex : `x = [4,5]` ;
- les tuples `tuple` : un tableau d'objets qui peut être de tout type. Ex : `x = (4,5)` ;
- les dictionnaires `dictionary` : un tableau non ordonné, où chaque élément est associé à une clé. Ex : `symboles = {"H" : "hydrogen", "He" : "helium", "Li" : "lithium"}`
- les sets ou ensembles `set` : une collection d'objets non ordonnée et contenant des éléments uniques. Ex : `s = {1,2,3}`.

Le type d'une variable peut changer, il correspond toujours au type de la dernière affectation.
La fonction `type()` détermine le type d'une variable.

Enfin, il y a des variables **immuables**, c'est-à-dire qu'elles ne peuvent pas être modifiées. Les nombres sont des types immuables, tout comme les chaînes de caractères et les tuples.
Ex : 
  ```
  x = (3,2)
  x[0] = 1
  TypeError: 'tuple' object does not support item assignment.
  ```


### 3.3. Boucles et conditions
Cf. chapitre 3 du cours OpenClassrooms

### 3.4. Gestion des fichiers
La ressource est disponible [ici](https://python.antoinepernot.fr/cours.php?course=chap5). Tu peux réaliser les activités si ça te dit, ou au moins comprendre les codes en solution (pour cela, tu dois d'abord envoyer un code).


## 4. Points importants à retenir
- Comprendre les différents types et comment on les reconnaît (parenthèses, crochets etc).
![Les types sous Python](https://github.com/TheHackingProject/data-analyst/blob/master/week_01/day_01/Capture%20d%E2%80%99e%CC%81cran%20(58).png)

- Se familiariser avec les méthodes les plus utilisées sur ces types (accéder à un élément, ajouter un élément, supprimer un élément, modifier un élément, compter le nombre d’éléments stockés etc.).

- Comprendre la gestion des fichiers avec Python

## 5. Pour aller plus loin
La documentation Python disponible [ici](https://docs.python.org/3/). Quand vous commencerez à être à l'aise avec Python, vous pourrez trouver des renseignements sur tous les packages et méthodes existants en Python.

Par ailleurs, il existe énormément de ressources en ligne pour apprendre à maîtriser Python. Si vous voulez appronfondir certaines notions de Python, voici quelques ressources qui pourront vous être utiles : 
- la chaîne YouTube *Machine Learnia* qui propose plus de 30 vidéos sur [Python pour le Machine Learning](https://www.youtube.com/watch?v=82KLS2C_gNQ&list=PLO_fdPEVlfKqMDNmCFzQISI2H_nJcEDJq)
- un [cours d'introduction à Python](https://courspython.com/)
- un [autre cours pour débutants sur Python](https://python.antoinepernot.fr/index.php)
- le site [Python Doctor](https://python.doctor/) qui vous donne plusieurs exemples

et bien d'autres encore ... à vous d'aller chercher celles qui vous correspondent le mieux ✌️✌️✌️!
