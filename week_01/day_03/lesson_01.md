# Bases de données et SQL 

Aujourd'hui nous allons découvrir les bases de données, le modèle relationnel et SQL.

## 1. Introduction
Il y a un des aspects du web que tu n'as pas encore vu lors des 3 premières semaines d'introduction au code : il s'agit des bases de données ! 

Or quand tu crées des applications web, il est indispensable de stocker les données (utilisateurs, messages échangés, etc.) quelque part. Dans cette ressource nous allons t'apprendre comment fonctionnent les bases de données et les logiciels dédiés au stockage des données : les SGBD (ou systèmes de gestions de bases de données).

A la fin de cette ressource, tu devrais :
- Savoir comment marche une base de données, un élément que tu retrouveras dans TOUTE application web ;
- Te projeter facilement dans le quotidien d'un Data Analyst, ce métier où l'on passe ses journées à miner dans des BDD.

## 2. Historique
Très rapidement dans l'informatique, nous eûmes besoin de stocker les informations, traitées par nos programmes, quelque part : ainsi furent créées les bases de données. En 1970, un certain Edgar Codd, ingénieur chez IBM, a inventé un moyen de lier en base des tables entre elles. Ainsi, une entrée, comme un `Message`, pourrait être liée à une autre entrée, par exemple en le faisant appartenir à un `User`. **Le modèle relationnel a révolutionné l'informatique puisqu'aujourd'hui, il reste le format le plus répandu dans les applications.**

Au début des années 70, deux ingénieurs chez IBM nommées Donald Chamberlin et Raymond Boyce, grâce aux travaux de "Ted" Codd ont inventé **un langage pour créer, modifier et lire une base de donnée relationnelle : le SQL** ou Structured Query Language. Leur invention est devenue tout aussi importante que celle de Mr Codd dans le monde de l'informatique : aujourd'hui le SQL est le langage de gestion de données le plus utilisé sur notre petite planète.

## 3. La ressource
### 3.1. Introduction aux bases de données

Suite aux projets que tu as réalisés avec les fichiers csv, tu peux imaginer que stocker tous les objets liés à un site web dans un fichier CSV, c'est fonctionnel mais pas toujours très pratique. En effet, supprimer une entrée n'est pas simple, chercher un élément donné peut être long et encore, tu n'as pas testé avec des milliers de lignes…

Nous allons ici commencer à étudier de vraies bases de données. Pour te faire un avis, regarde cette vidéo de [LucidChart](https://www.youtube.com/watch?v=wR0jg0eQsZA) où ils expliquent le concept des bases de données. Ensuite, je t'invite à regarder cette [vidéo de Khan Academy](https://www.youtube.com/watch?v=IXycPq7MnwE) qui explique les bases de données.

Comme tu l'as compris, une base de données permet de stocker facilement de la donnée et d'y avoir accès. On peut se représenter une base de données comme un ensemble de gros tableurs Excel, avec des lignes et des colonnes, qu'on appellerait des tables.

> Techniquement, une base de données n'est que votre ensemble de données. Le système de gestion de base de données (SGBD) est le logiciel que vous utilisez pour structurer et gérer ces données. Le simple terme de « base de données » est couramment utilisé pour désigner un SGBD. Cet abus de langage est assez répandu et permet d'éviter les phrases interminables. 

Le SGBD est donc un outil logiciel assurant l'interface Utilisateur/Base de données. Parmi les logiciels de base de données les plus célèbres, on peut citer : MySQL, PostgreSQL, SQL Server, Oracle, SQLite, etc.

___

🔴 ALERTE 🔴

Outre les SGBD classiques (ou SGBDr avec r pour relationnelles), on parle aujourd'hui de NoSQL et de big data. Il n'y a donc pas que les SGBDr et le langage SQL pour manipuler les données. Mais nous verrons cela demain. Aujourd'hui, nous restons dans le monde des bases de données relationnelles.

___


### 3.2. Le modèle relationnel 

Pour bien comprendre les concepts fondamentaux du modèle relationnel, nous te demandons de suivre le cours OpenClassrooms [Initiez-vous à l'algèbre relationnelle avec le langage SQL](https://openclassrooms.com/fr/courses/4449026-initiez-vous-a-lalgebre-relationnelle-avec-le-langage-sql). Commence par faire les deux premiers chapitres. Ils pourront te paraître théoriques mais ils constitueront un très bon socle de connaissances pour appréhender ensuite la pratique de SQL et de Python. Le cours est très bien fait et surtout il est vraiment réalisé pour des futurs Data Analysts. 

Une fois les deux premiers chapitres réalisés (jusqu'au Quizz "xxxx), tu pourras lire ce récapitulatif de toute la terminologie du monde relationnel : 

copier-coller cours GK ...


Voir si on laisse ça : 
Il existe trois types de relations entre les tables d'une base de données :
Relation 1-1 : Assez rare, elle sert à modéliser l'exclusivité. Par exemple : dans une hypothétique base de données "session THP en cours", un moussaillon a un unique ordinateur et chaque ordinateur appartient à un moussaillon. Bref, c'est du 1-1 entre 2 tables cabin_boys et computers.
Relation 1-N : Très courante, elle sert à modéliser une appartenance. Par exemple : dans une hypothétique base de données "France", chaque habitant vit dans une ville unique mais chaque ville a plusieurs habitants. C'est du 1-N entre la table cities et la table people.
Relation N-N : Très courante aussi, elle permet de modéliser un lien mais sans aucune unicité. Par exemple : un docteur a plusieurs patients et un patient peut avoir plusieurs docteurs. C'est du N-N entre la table doctors et la table patients.

Dans cette vidéo de O'Reilly, tu pourras comprendre ce qu'est qu'une base de données relationnelle.

### 3.3. SQL

2 autre chapitres OC 






## 4. Points importants à retenir


## 5. Pour aller plus loin
Voici quelques ressources pour être au top du SQL.

Le cours de W3 Schools, qui contient une doc exhaustive de ce que l'on veut faire en SQL. Très pratique pour vérifier des syntaxes de méthodes.
Plein d'exercices chez SQL Zoo, idéal pour s'entraîner et se sentir un Data-Analyst
SQL avec des exercices
Le cours de Khan Academy



