# Bases de données et SQL pour débutants

Aujourd'hui nous allons découvrir les bases de données, le modèle relationnel et SQL.

## 1. Introduction
Il y a un des aspects du web que tu n'as pas encore vu lors des 3 premières semaines d'introduction au code : il s'agit des bases de données ! 

Or quand tu crées des applications web, il est indispensable de stocker les données (utilisateurs, messages échangés, etc.) quelque part. Dans cette ressource nous allons t'apprendre comment fonctionnent les bases de données et les logiciels dédiés au stockage des données : les SGBD (ou systèmes de gestions de bases de données).

A la fin de cette ressource, tu devrais :

Savoir comment marche une base de données, un élément que tu retrouveras dans TOUTE application web ;

Te projeter facilement dans le quotidien d'un Data Analyst, ce métier où l'on passe ses journées à miner dans des BDD.

## 2. Historique
Très rapidement dans l'informatique, nous eûmes besoin de stocker les informations, traitées par nos programmes, quelque part : ainsi furent créées les bases de données. En 1970, un certain Edgar Codd, ingénieur chez IBM, a inventé un moyen de lier en base des tables entre elles. Ainsi, une entrée, comme un Message, pourrait être liée à une autre entrée, par exemple en le faisant appartenir à un User. Ce modèle de base de données relationnelle a révolutionné l'informatique puisqu'aujourd'hui, il reste le format le plus répandu dans les applications.

Au début des années 70, deux ingénieurs chez IBM nommées Donald Chamberlin et Raymond Boyce, grâce aux travaux de "Ted" Codd ont inventé un langage pour créer, modifier et lire une base de donnée relationnelle : le SQL ou Structured Query Language. Leur invention est devenue tout aussi importante que celle de Mr Codd dans le monde de l'informatique : aujourd'hui le SQL est le langage de gestion de données le plus utilisé sur notre petite planète.

## 3. La ressource
### 3.1. Introduction aux bases de données
#### 3.1.1. Un gros classeur Excel
Les projets de la semaine passée t'ont montré que stocker tous les objets liés à notre application dans un fichier CSV, c'est fonctionnel mais pas toujours très pratique. En effet, supprimer une entrée n'est pas simple, chercher un élément donné peut être long et encore, tu n'as pas testé avec des milliers de lignes…
Nous allons donc commencer à utiliser les VRAIES bases de données pour nos applications. Pour te faire un avis, regarde cette vidéo de LucidChart où ils expliquent le concept des bases de données. (Ils parlent même des ERD (Entity–Relationship Diagram) qui permettent de les dessiner ; on verra plus bas quelques outils à ce sujet). Ensuite, je t'invite à regarder cette vidéo de Khan Academy qui explique les bases de données.

Comme tu l'as compris, une base de données permet de stocker facilement de la donnée et d'y avoir accès. On peut se représenter une base de données comme un ensemble de gros tableurs Excel, avec des lignes et des colonnes, qu'on appellerait des tables.

Voici un exemple d'une table d'utilisateurs (users) :

id	first_name	last_name	age	city
1	Martin	Dupond	27	Paris
---	---	---	---	---
2	Jack	Quilley	38	London
---	---	---	---	---
3	Vittorio	Piccolini	18	Milan
---	---	---	---	---
Tu remarqueras que la première colonne est un peu étonnante : elle s'appelle "id". Son rôle est d'ordonner les éléments de la BDD et de facilement y faire référence : l'id est un identifiant unique associé à chaque entrée dans la table.

