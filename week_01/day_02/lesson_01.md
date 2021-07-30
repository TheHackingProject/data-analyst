# Modules et librairies

## 1. Introduction
Hier, nous avons vu que le langage Python peut servir pour des projets très divers (de la création d'applications à l'analyse de données). Nous allons découvrir aujourd'hui ce qui a fait le succès de Python dans la data : ses librairies spécialisées pour l'analyse de données. Mais comprenons d'abord ce que sont les modules et les librairies 📚📚.

## 2. La ressource
Peut-être qu'hier, lors de ta première journée Python, tu as été bloqué par moments car tu ne trouvais pas de fonction native correspondant à ce que tu voulais faire. Par exemple, pour calculer la racine carrée d'un nombre. Ou alors, peut être que dans tes recherches, tu es tombé sur des programmes qui commençaient par plusieurs `import` à la suite. A la fin de la journée, tu connaîtras tous ces concepts sur le bout des doigts.

### 3.1. Les modules

#### 3.1.1 Définition d'un module
On appelle **module** tout fichier constitué de code Python (c’est-à-dire tout fichier avec l’extension .py) importé dans un autre fichier ou en mode interactif. Les modules permettent la séparation et donc une meilleure organisation du code. Autre avantage : certains modules te font économiser du temps car ils contiennent déjà des fonctions que tu n'auras pas besoin de détailler à ton tour.

En Python, on peut distinguer trois grandes catégories de module en les classant selon leur éditeur :
- Les modules standards qui ne font pas partie du langage en soi mais sont intégrés automatiquement par Python ;
- Les modules développés par des développeurs externes qu’on va pouvoir utiliser ;
- Les modules qu’on va développer nous-mêmes.

#### 3.1.2 Utiliser un module
Un programme Python va généralement être composé d’un script principal qui va importer différents modules (c’est-à-dire différents fichiers Python) pour pouvoir les utiliser.
Pour importer un module, on utilise la syntaxe `import nom-de-mon-module`. 

Dans un second temps, pour utiliser les éléments du module dans notre script, il faudra préfixer le nom de ces éléments par le nom du module et un point. Cela permet d’éviter les conflits dans le cas où on aurait défini des éléments de même nom que ceux disponibles dans le module.

Par exemple, prenez votre éditeur favori et créez un fichier `fibo.py` dans le répertoire courant qui contient :
```
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

Vous pouvez donc appeler les fonctions via le nom du module :
```
> fibo.fib(1000)
0 1 1 2 3 5 8 13 21 34 55 89 144 233 377 610 987
> fibo.fib2(100)
[0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]
```


#### 3.1.3 Modules standards

Comme tu l'as lu au début de cette leçon, nous importerons bien souvent des modules créés par d’autres développeurs ou des modules mis à notre disposition par Python lui même.
En effet, il existe un grand nombre de modules préconçus et prêts à l’emploi qui sont fournis d’office avec Python. Ces modules vont étendre le langage et nous permettre de réaliser toutes sortes d’opérations, notamment grâce aux fonctions qu’ils nous fournissent. Pour importer un module Python, nous allons à nouveau tout simplement utiliser une instruction `import` comme si on importait l’un de nos modules.

Les modules Python standards à connaitre sont les suivants :
- Le module `cgi` (“Common Gateway Interface” ou “Interface de Passerelle Commune” en français) fournit des éléments permettant à des programmes Python de s’exécuter sur des serveurs HTTP ;
- Le module `datetime` fournit des classes pour manipuler de façon simple ou plus complexe des dates et des heures ;
- Le module `json` permet l’encodage et le décodage de données au format JSON ;
- Le module `math` fournit un ensemble de fonctions permettant de réaliser des calculs mathématiques complexes ;
- Le module `os` fournit une manière portable d’utiliser les fonctionnalités dépendantes du système d’exploitation ;
- Le module `random` implémente des générateurs de nombres pseudo-aléatoires pour différentes distributions ;

Vous pouvez retrouver la liste complète des modules standards Python sur le site de [la documentation](https://docs.python.org/fr/3/library/index.html).


### 3.2. Les librairies
blabla

## 4. Points importants à retenir
La ressource en quelques points importants.

## 5. Pour aller plus loin
Quelques éléments en ligne pour aller plus loin
