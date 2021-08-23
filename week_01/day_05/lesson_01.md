# Première étape : la collecte des données
Commençons par le commencement : comment obtient-on des données dans la pratique ?

## 1. Introduction
Maintenant que tu connais les langages indispensables à un bon Data Analyst, il faut que tu comprennes le processus général d'analyse de données. Ce processus se compose de différentes étapes. La première étape est sans aucun doute l'obtention des données. En effet, pour tout projet, l'entreprise doit en premier lieu identifier la ou les sources de données intéressantes puis voir comment utiliser ces sources.

## 2. Historique et contexte
Pendant des siècles, l’humanité a stocké ses données dans les livres 📝. L’arrivée du digital au XXème siècle a donné une dimension exponentielle et globale à cette pratique. Cette révolution des données, qui n’est encore qu’à ses prémices, est en train de multiplier les sources de données et de nous donner, à chacun, la possibilité d'étudier ces multiples données.

Plus précisément, environ 2,5 trillions d'octets de données sont produits chaque jour. Ce sont des informations provenant de sources divers : messages, vidéos, informations climatiques, signaux GPS, transactions etc. Sur Facebook seulement, nous envoyons 10 milliards de messages par jour. La quantité de données digitales produites double tous les 2 ans. En d'autres termes, on a produit autant de données digitales ces 2 dernières années que tout ce qui a été produit auparavant. 

Maintenant que l'on sait que toutes ces données existent, nous allons voir comment on récupère ces données ⭐️⭐️.

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

On peut schématiser le fonctionnement ainsi :
![fonctionnement](https://github.com/TheHackingProject/data-analyst/blob/master/week_01/day_05/Capture%20d%E2%80%99e%CC%81cran%202021-08-23%20a%CC%80%2017.56.06.png)


Mais s'il n'y a pas d'application déjà codée comme lorsque tu réserves tes billets de train, c’est un programme Python qui peut jouer le rôle d’application intermédiaire. Le dialogue se fera avec un SGBD, comme le SGBD SQLite3 par exemple. La plupart des langages de programmation ont des bibliothèques permettant à un programme de dialoguer avec la plupart des SGBD existants. Le couple Python-SQLite3 ne déroge pas à la règle, et c’est le module 'sqlite3' qu'il faut utiliser.

Pour interagir avec la base de données via Python, il y a plusieurs étapes et ça peut être fastidieux. 
Retrouve ces différentes étapes dans [ce cours](https://python.antoinepernot.fr/cours.php?course=chap6). 

Retiens-les 3 étapes principales : 
1) Installer puis importer le connecteur (ex : 'mysql.connector' ou 'sqlite3')
2) Se connecter à la base de données en inscrivant la bonne configuration
3) Extraire des données à partir de la base puis fermer la connexion.


#### 3.2.3 Accéder à des données en scrapant le web

Le web scraping est une technique d'extraction des données de site Internet afin de les enregistrer puis de les analyser. En Python, l'extraction des données depuis le web est souvent réalisée à l'aide du module 'BeautifulSoup'.

Pour apprendre à scraper avec Python, je te recommande [cet article](https://medium.com/france-school-of-ai/web-scraping-avec-python-apprenez-%C3%A0-utiliser-beautifulsoup-proxies-et-un-faux-user-agent-d7bfb66b6556) ou cette [vidéo Youtube](https://www.youtube.com/watch?v=Wvc2ZqdIPpk), en fonction du format que tu préfères.


#### 3.2.4 Accéder à des données via une API

Même si le web scraping a son utilité, ce n’est pas la méthode à privilégier pour obtenir des données des sites Internet. En effet, il existe souvent une meilleure méthode : de nombreux exploitants de sites Internet mettent à disposition les données dans un format structuré, lisible par une machine. Pour accéder aux données, on utilise alors des interfaces de programmation spéciales, appelées *Application Programming Interfaces* (API).

Les avantages de l’utilisation d’une API sont significatifs :
- L’API est explicitement mise à disposition par le fournisseur pour accéder aux données : les risques juridiques sont donc plus faibles et le fournisseur est mieux à même de réglementer l’accès aux données. Une clé API peut par exemple être exigée pour accéder aux données. Par ailleurs, le fournisseur peut mettre en place une limitation plus précise du débit.
- L’API fournit directement les données dans un format lisible par la machine : par conséquent, il n’est pas nécessaire d’extraire les données du code source, une étape fastidieuse dans le web scraping. D’autre part, la structure des données est séparée de la représentation visuelle. La structure est ainsi conservée même si le design du site Internet est modifié.

En Python, la librairie la plus utilisée est Requests. Voici un tuto qui t'explique [comment démarrer avec la librairie Requests en Python](https://www.digitalocean.com/community/tutorials/how-to-get-started-with-the-requests-library-in-python-fr).


## 4. Points importants à retenir
Le processus d'analyse de données (ou *Data Analysis*) peut être décomposé en plusieurs phases. La première étape est la collecte de données, en provenance d’une ou plusieurs sources. 


## 5. Pour aller plus loin

