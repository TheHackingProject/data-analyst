# Première étape : obtenir des données
Commençons par le commencement : comment obtient-on des données dans la pratique ?

## 1. Introduction
Maintenant que tu connais les langages indispensables à un bon Data Analyst, il faut que tu comprennes le processus général d'analyse de données. Ce processus se compose de différentes étapes. La première étape est sans aucun doute l'obtention des données. En effet, pour tout projet, l'entreprise doit en premier lieu identifier la ou les sources de données intéressantes puis voir comment utiliser ces sources.

## 2. Historique et contexte
Pendant des siècles, l’humanité a stocké ses données dans les livres 📝. L’arrivée du digital au XXème siècle a donné une dimension exponentielle et globale à cette pratique. Cette révolution des données, qui n’est encore qu’à ses prémices, est en train de multiplier les sources de données et de nous donner, à chacun, la possibilité d'étudier ces multiples données.

Plus précisément, environ 2,5 trillions d'octets de données sont produits chaque jour. Ce sont des informations provenant de sources divers : messages, vidéos, informations climatiques, signaux GPS, transactions etc. Sur Facebook seulement, nous envoyons 10 milliards de messages par jour. La quantité de données digitales produites double tous les 2 ans. En d'autres termes, on a produit autant de données digitales ces 2 dernières années que tout ce qui a été produit auparavant. 

Maintenant que l'on sait que toutes ces données existent, nous allons voir comment on récupère ces données, pour ensuite les traiter ⭐️⭐️.

## 3. La ressource

### 3.1. Les sources de données
Une source de données est l’endroit d’où proviennent les données utilisées. Elle peut être l’endroit où les données ont été créées ou celui où les informations physiques ont été numérisées. 

Concrètement, une source de données peut être : 
- un fichier plat, 
- une base de données, 
- des mesures provenant directement d’appareils physiques, 
- des données obtenues par web scraping ou 
- l’une des nombreux services de données en streaming qui abondent sur Internet (analyse du parcours de navigation des internautes, jeux en ligne, e-commerce etc.).

Voici un exemple d’une source de données en action. Imaginez une marque de mode qui vend des produits en ligne. Pour indiquer qu’un article est en rupture de stock, le site web collecte des informations dans une base de données d’inventaire. Dans ce cas de figure, les tableaux d’inventaire sont une source de données, à laquelle accède l’application web pour afficher le site web aux clients.


### 3.2. Comment accéder à ces sources de données via Python

#### 3.2.1 Accéder à des données dans un fichier 
Comme nous l'avons déjà vu, la bibliothèque Pandas de Python permet de récupérer des données depuis quasiment tous les types de fichiers (CSV, JSON, Excel ...). Cf. la [doc](https://pandas.pydata.org/pandas-docs/dev/user_guide/io.html) pour voir tous les types d'inputs qui peuvent être traités. 

Pour lire un fichier CSV par exemple et obtenir un DataFrame, il faudra faire ceci : 
```
>>> import pandas as pd
>>> filename = 'chemin/vers/fichier.csv'
>>> df = pd.read_csv(filename)
```

#### 3.2.2 Accéder à des données dans une base de données
Lors des journées de mercredi et jeudi, vous avez interrogé une base de données en dialoguant avec un SGBD. Mais cela ne se passe pas toujours comme ça. 

___

💡💡  LUMIERE 💡💡

Dans la plupart des cas auxquels tu es habitué, l’utilisateur final se trouve devant un programme, qui peut être par exemple une application standard ou une page web, qui sert d’intermédiaire entre l’utilisateur et le SGBD. L’utilisateur n’interagit donc pas directement avec le SGBD, mais avec l’application intermédiaire. Selon les interactions avec l’utilisateur, l’application se charge de construire des requêtes au SGBD et de renvoyer le résultat à l’utilisateur de manière conviviale.

À titre d’exemple, considérons une application fictive de recherche d’horaires de train. Voici un scénario possible de fonctionnement de cette application :
1. L’application demande à l’utilisateur : « Quelle est la ville de départ ? ».
2. L’utilisateur répond « Caussade ».
3. L’application demande à l’utilisateur : « Quelle est la ville d’arrivée ? ».
4. L’utilisateur répond « Brive-la-Gaillarde ».
5. L’application envoie au SGBD la requête SQL :
```
SELECT heureDep, heureArr FROM trains
WHERE villeDep = ’Caussade’ AND villeArr = ’Brive-la-Gaillarde’;
```
6. Le SGBD répond au programme en envoyant l’ensemble de tuples {(15h47, 17h22); (18h21, 19h58)}
7. Le programme affiche à l’utilisateur :
Résultats pour le trajet Caussade -> Brive-la-Gaillarde
Premier train : 15h47 -> 17h22
Second train : 18h21 -> 19h58

___

Dans notre cas précis, c’est un programme Python qui peut jouer le rôle d’application intermédiaire. Le dialogue se fera avec le SGBD SQLite3 par exemple. La plupart des langages de programmation ont des bibliothèques permettant à un programme de dialoguer avec la plupart des SGBD existants. Le couple Python-SQLite3 ne déroge pas à la règle, et c’est le
module sqlite3 qu'il faut utiliser.


#### 3.2.3 Accéder à des données en scrapant le web

#### 3.2.4 Accéder à des données via une API


## 4. Points importants à retenir
La ressource en quelques points importants.

## 5. Pour aller plus loin
Quelques éléments en ligne pour aller plus loin
