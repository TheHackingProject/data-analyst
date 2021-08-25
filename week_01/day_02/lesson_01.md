# Modules et librairies

## 1. Introduction
Hier, nous avons vu que le langage Python peut servir pour des projets très divers (de la création d'applications à l'analyse de données). Nous allons découvrir aujourd'hui ce qui a fait le succès de Python dans la data : ses librairies spécialisées pour l'analyse de données. Mais comprenons d'abord ce que sont les modules et les librairies 📚📚

## 2. La ressource
Peut-être qu'hier, lors de ta première journée Python, tu as été bloqué par moments car tu ne trouvais pas de fonction native correspondant à ce que tu voulais faire. Par exemple, pour calculer la racine carrée d'un nombre. Ou alors, peut être que dans tes recherches, tu es tombé sur des programmes qui commençaient par plusieurs `import` à la suite. A la fin de la journée, ces situations n'auront plus de secret pour toi.

### 3.1. Les modules

#### 3.1.1 Définition d'un module
On appelle **module** tout fichier constitué de code Python (c’est-à-dire tout fichier avec l’extension .py) importé dans un autre fichier ou en mode interactif (cad quand tu es sur ton Notebook). Les modules permettent la séparation et donc une meilleure organisation du code. Autre avantage : certains modules te font économiser du temps car ils contiennent déjà des fonctions que tu n'auras pas besoin de ré-écrire à ton tour.

En Python, on peut distinguer trois grandes catégories de module en les classant selon leur éditeur :
- Les modules standards qui ne font pas partie du langage en soi mais sont intégrés automatiquement par Python ;
- Les modules développés par des développeurs externes qu’on va pouvoir utiliser ;
- Les modules qu’on va développer nous-mêmes.

#### 3.1.2 Utiliser un module
Un programme Python va généralement être composé d’un script principal qui va importer différents modules (c’est-à-dire différents fichiers Python) pour pouvoir les utiliser.
Pour importer un module, on utilise la syntaxe `import nom-de-mon-module`. 

Dans un second temps, pour utiliser les éléments du module dans notre script, il faudra préfixer le nom de ces éléments par le nom du module et un point. Cela permet d’éviter les conflits dans le cas où on aurait défini des éléments de même nom que ceux disponibles dans le module.

Par exemple, prenez votre éditeur favori et créez un fichier `fibo.py` dans le répertoire courant qui contient :
```python
# Fibonacci numbers module

def fib(n):    # write Fibonacci series up to n
    a, b = 0, 1
    while a < n:
        print(a, end=' ')
        a, b = b, a+b
    print()

def fib2(n):   # return Fibonacci series up to n
    result = []
    a, b = 0, 1
    while a < n:
        result.append(a)
        a, b = b, a+b
    return result
```
Maintenant, ouvrez un interpréteur et importez le module en tapant :

`> import fibo`

Vous pouvez maintenant appeler les fonctions via le nom du module que vous venez de créer :
```python
> fibo.fib(1000)
0 1 1 2 3 5 8 13 21 34 55 89 144 233 377 610 987
> fibo.fib2(100)
[0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]
```

___

💡💡 ASTUCE 💡💡

Si vous ne souhaitez pas réécrire le nom du module à chaque fois, vous avez deux autres options :
- soit donner un alias au nom de votre module, pour n’avoir à écrire que l’alias :
`import fibo as fb`
- soit importer des fonctions spécifiques que vous pourrez ensuite utiliser comme des fonctions/variables Python natives (sans la notation .) :
`from fibo import fib`

Un cas particulier de cette dernière méthode est d’importer en une ligne tous les objets contenus dans un module via la notation  `*`. Néanmoins, ce n’est pas la méthode préconisée, afin d’éviter par exemple les conflits entre plusieurs modules qui pourraient avoir un nom de fonction identique.
`from fibo import *`

___



#### 3.1.3 Modules standards

Comme tu l'as lu au début de cette leçon, nous importons bien souvent des modules créés par d’autres développeurs ou des modules mis à notre disposition par Python lui-même.
En effet, il existe un grand nombre de modules préconçus et prêts à l’emploi qui sont fournis d’office avec Python. Ces modules vont étendre le langage et nous permettre de réaliser toutes sortes d’opérations, notamment grâce aux fonctions qu’ils nous fournissent. Pour importer un module Python, nous allons à nouveau tout simplement utiliser une instruction `import` comme si on importait l’un de nos modules.

Les modules Python standards à connaitre sont les suivants :
- Le module `cgi` (“Common Gateway Interface” ou “Interface de Passerelle Commune” en français) fournit des éléments permettant à des programmes Python de s’exécuter sur des serveurs HTTP ;
- Le module `datetime` fournit des classes pour manipuler de façon simple ou plus complexe les dates et les heures ;
- Le module `json` permet l’encodage et le décodage de données au format JSON ;
- Le module `math` fournit un ensemble de fonctions permettant de réaliser des calculs mathématiques complexes ;
- Le module `os` fournit une manière portable d’utiliser les fonctionnalités dépendantes du système d’exploitation ;
- Le module `random` implémente des générateurs de nombres pseudo-aléatoires pour différentes distributions.

Vous pouvez retrouver la liste complète des modules standards Python sur le site de [la documentation](https://docs.python.org/fr/3/library/index.html).


### 3.2. Les librairies

#### 3.2.1 Définition d'une librairie

Quand on a un grand nombre de modules, il peut être intéressant de les organiser dans des dossiers. Un dossier qui rassemble des modules est appelé un *package* (paquet ou librairie en français).

Une librairie est donc une collection, un ensemble de modules Python. Comme vous l’avez vu ci-dessus, un module est un fichier Python. Un package est simplement un dossier contenant plusieurs fichiers Python (.py) et un fichier additionnel nommé  __init__.py. Ce dernier différencie un package d’un dossier lambda contenant uniquement des codes Python.

On va pouvoir importer des paquets de la même façon que des modules et accéder à un module ou à un élément en particulier en utilisant la syntaxe `nom-paquet.nom-module.nom-element`.

Par exemple, on crée un dossier `package1` dans lequel on place le fichier `module1.py` suivant :
```python
def fonction1(a):
    return a**2
```
On peut ensuite utiliser la fonction `fonction1()` définie dans `module1.py,` en important `package1.module1` comme dans l’exemple qui suit :
```python
import package1.module1

u = package1.module1.fonction1(3)
print("u vaut", u)
```

#### 3.2.2 Les librairies dans l'analyse de données
Les packages sont omniprésents dans l’analyse de données avec Python. En effet, de nombreux packages ont été créés spécifiquement pour répondre aux problématiques du domaine. Au fur et à mesure de la formation data, tu vas être amené à :
- manipuler des données pour en faciliter l’analyse ;
- réaliser différents graphiques pertinents représentant le comportement de tes données ;
- utiliser des méthodes statistiques ;
- faire tourner des algorithmes de machine learning plus ou moins compliqués ;
etc.

Et pour réaliser tout cela, il te sera indispensable de maîtriser les différents objets et fonctions issus des librairies correspondantes. Avec les autres ressources du jour, tu vas déjà découvrir deux librairies indispensables pour l'analyse de données. J'espère que tu es au taquet 💪💪

## 4. Points importants à retenir
Dans cette leçon, nous avons vu ensemble les bases de l’utilisation des modules et des packages :
- un module est un fichier contenant du code Python qui peut définir des fonctions, des classes et/ou des variables ;
- vous pouvez importer n’importe quel module Python via le mot clé `import`;
- pour utiliser une fonction d’un module, ou une classe ou une variable, il faut utiliser l’opérateur `.`;
- une librairie ou package est un ensemble de plusieurs modules Python ;
- il existe de nombreux packages spécifiquement créés pour l’analyse de données.

## 5. Pour aller plus loin
- Découvrir le module `random` avec [le cours OC](https://openclassrooms.com/fr/courses/6204541-initiez-vous-a-python-pour-lanalyse-de-donnees/6252451-manipulez-des-nombres-aleatoires-avec-le-module-random) et faire le quizz qui suit 👣👣
