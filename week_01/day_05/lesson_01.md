# Modéliser un data warehouse ou système d'information décisionnel

## 1. Introduction
Tu as normalement bien compris la différence entre base de données et système de BI. Pour rappel, les entrepôts de données (ou data warehouses) sont un type spécial de base de données, spécifiquement construit dans le but d'exécuter des analyses. 

Alors que la plupart des bases de données sont des fichiers d'application OLTP, la plupart des entrepôts de données sont des fichiers OLAP (*Online Application Processing*). En raison de la structure des fichiers OLAP, il est beaucoup plus facile d'effectuer des requêtes et des analyses sur les données qu'ils contiennent, et n'importe qui peut interroger l'entrepôt de données avec un logiciel d'entrepôt de données ou une connaissance du SQL.

Alors qu'on s'attend à ce que les bases de données aient un temps de disponibilité de 99,99 %, les entrepôts de données n'ont généralement pas besoin d'avoir ce genre de temps de disponibilité. BLes entrepôts de données ne sont pas constamment lus et écrits comme les bases de données le sont. La plupart des entrepôts de données se rafraîchissent avec les données des bases de données, souvent toutes les 24 heures environ.

On va maintenant voir comment on modélise ces deux types de systèmes. Dans cette ressource, focus sur les data warehouses 👉

## 2. Historique et contexte
**Le concept de data warehousing remonte à la fin des années 1980** lorsque les chercheurs d'IBM Barry Devlin et Paul Murphy ont développé le « business data warehouse ». Essentiellement, le concept d'entreposage de données visait à fournir un modèle architectural pour le flux de données des systèmes opérationnels aux environnements d'aide à la décision.

Le concept a tenté de répondre aux différents problèmes associés à ce flux, principalement les coûts élevés qui y sont associés. En l'absence d'une architecture d'entreposage de données, une énorme quantité de redondance était nécessaire pour prendre en charge plusieurs environnements d'aide à la décision. Dans les grandes entreprises, il était courant que plusieurs environnements d'aide à la décision fonctionnent de manière indépendante. Bien que chaque environnement servait des utilisateurs différents, ils nécessitaient souvent une grande partie des mêmes données stockées. Le processus de collecte, de nettoyage et d'intégration des données provenant de diverses sources, généralement des systèmes opérationnels existants à long terme (souvent appelés systèmes hérités), était en partie répliqué pour chaque environnement.

En 1990, la société Red Brick Systems, fondée par Ralph Kimball, lance Red Brick Warehouse, un système de gestion de base de données spécialement conçu pour l'entreposage de données.

## 3. La ressource

### 3.1 Modéliser une BDD

En fait, la modélisation permet avant tout d'avoir un langage commun.


## 4. Points importants à retenir
Les bases de données relationnelles sont la base de la majorité des applications. Pour concevoir une BDD relationnelle, SQL est le langage de prédilection.

Avant de coder une BDD, il faut se poser pour établir toutes les tables, les relations entre elles et leurs attributs. 

Il faut également se demander s'il s'agit d'une base de données opérationnelle ou alors d'un datawarehouse car la modélisation ne sera pas la même. 

Le Data Analyst doit savoir travailler avec les tous les types de bases de données (même si quand le datawarehouse est déjà mis en place, il travaillera principalement sur le système d'info décisionnel). 

## 5. Pour aller plus loin
- Pour approfondir la modélisation de bases de données classique, cf. le cours [Modélisez et implémentez une base de données relationnelle avec UML](https://openclassrooms.com/fr/courses/4055451-modelisez-et-implementez-une-base-de-donnees-relationnelle-avec-uml)
- Pour approfondir la notion de 
