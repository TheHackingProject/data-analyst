# Bases de données et SQL 

Aujourd'hui nous allons découvrir les bases de données, le modèle relationnel et SQL.

## 1. Introduction
Il y a un des aspects du web que tu n'as pas encore vu lors des 3 premières semaines d'introduction au code : il s'agit des bases de données ! 

Or quand tu crées des applications web, il est indispensable de stocker les données (utilisateurs, messages échangés, etc.) quelque part. Dans cette ressource, nous allons t'apprendre comment fonctionnent les bases de données et les logiciels dédiés au stockage des données : les SGBD (ou systèmes de gestion de bases de données).

A la fin de cette ressource, tu devrais :
- Savoir comment marche une base de données, un élément que tu retrouveras dans TOUTE application web ;
- Te projeter facilement dans le quotidien d'un Data Analyst, ce métier où l'on passe ses journées à miner dans des BDD.

📌 *Utilité pour le projet* : 5/5<br/>
📊 *Utilité pour être Data Analyst* : 5/5<br/>
💡 *Pourquoi cette ressource ?* : Aujourd'hui, c'est simple, tu fonces tête baissée dans les projets et tu requêtes toute la journée en SQL, compétence très présente dans les offres d'emploi de Data Analyst (car nécessaire pour requêter une base de données relationnelle ou pouvoir utiliser certains outils de dataviz). 

## 2. Historique
Très rapidement dans l'informatique, nous eûmes besoin de stocker les informations, traitées par nos programmes, quelque part : ainsi furent créées les bases de données. En 1970, un certain Edgar Codd, ingénieur chez IBM, a inventé un moyen de lier en base des tables entre elles. Ainsi, une entrée, comme un `Message`, pourrait être liée à une autre entrée, par exemple en le faisant appartenir à un `User`. **Le modèle relationnel a révolutionné l'informatique puisqu'aujourd'hui, il reste le format le plus répandu dans les applications.**

Au début des années 70, deux ingénieurs chez IBM nommées Donald Chamberlin et Raymond Boyce, grâce aux travaux de "Ted" Codd ont inventé **un langage pour créer, modifier et lire une base de donnée relationnelle : le SQL** ou Structured Query Language. Leur invention est devenue tout aussi importante que celle de Mr Codd dans le monde de l'informatique : aujourd'hui le SQL est le langage de gestion de données le plus utilisé sur notre petite planète.

## 3. La ressource
### 3.1. Introduction aux bases de données

Suite aux projets que tu as réalisés avec les fichiers csv, tu peux imaginer que stocker tous les objets liés à un site web dans un fichier CSV, c'est fonctionnel mais pas toujours très pratique. En effet, supprimer une entrée n'est pas simple, chercher un élément donné peut être long et encore, tu n'as pas testé avec des milliers de lignes…

Nous allons ici commencer à étudier de vraies bases de données. Pour te faire un avis, regarde cette vidéo de [LucidChart](https://www.youtube.com/watch?v=wR0jg0eQsZA) où ils expliquent le concept des bases de données. Ensuite, je t'invite à regarder cette [vidéo de Khan Academy](https://www.youtube.com/watch?v=IXycPq7MnwE) qui explique les bases de données.

Comme tu l'as compris, une base de données permet de stocker facilement de la donnée et d'y avoir accès. On peut se représenter une base de données comme un ensemble de gros tableurs Excel, avec des lignes et des colonnes, qu'on appellerait des tables.

> Techniquement, une base de données n'est que ton ensemble de données. Le système de gestion de base de données (SGBD) est le logiciel qu'on utilise pour structurer et gérer ces données. Le simple terme de « base de données » est couramment utilisé pour désigner un SGBD. Cet abus de langage est assez répandu et permet d'éviter les phrases interminables. 

Le SGBD est donc un outil logiciel assurant l'interface Utilisateur/Base de données. Parmi les logiciels de base de données les plus célèbres, on peut citer : MySQL, PostgreSQL, SQL Server, Oracle, SQLite, etc.

___

🔴 ALERTE 🔴

Outre les SGBD classiques (ou SGBDr avec r pour relationnelles), on parle aujourd'hui de NoSQL et de big data. Il n'y a donc pas que les SGBDr et le langage SQL pour manipuler les données. Mais nous verrons cela demain. Aujourd'hui, nous restons dans le monde des bases de données relationnelles.

___


### 3.2. Le modèle relationnel 

Pour bien comprendre les concepts fondamentaux du modèle relationnel, nous te demandons de suivre le cours OpenClassrooms [Initiez-vous à l'algèbre relationnelle avec le langage SQL](https://openclassrooms.com/fr/courses/4449026-initiez-vous-a-lalgebre-relationnelle-avec-le-langage-sql). Commence par faire les deux premiers chapitres. Ils pourront te paraître théoriques mais ils constituent un très bon socle de connaissances pour appréhender ensuite la pratique de SQL, et même de Python. Le cours est très bien fait et surtout il est vraiment réalisé pour des futurs Data Analysts. 

Une fois les deux premiers chapitres réalisés (jusqu'au Quiz "L'algèbre relationnelle"), tu peux lire ce récapitulatif de  la terminologie du monde relationnel : 

- Un **SGBDR** est un logiciel pouvant gérer plusieurs bases de données dans une entreprise. Il permet de construire une base, d'assurer son intégrité et ses sauvegardes, de stocker les données de cette base, de manipuler les données et ce via le langage **SQL** (Structured Query Language). Il s'agit donc d'une interface entre l'homme et la machine.
- La structure qui permet de stocker les données se nomme une **table**. Une table contient des **colonnes** et des **lignes**. Une table a toujours une **clé**, que l'on nomme clé primaire. Elle peut avoir plusieurs index. 
- Un **index** est un ensemble de pointeurs, permettant de récupérer les données plus rapidement que s'il fallait lire séquentiellement toutes les lignes d'une table. Il pointe vers une ligne en particulier.
- Les tables peuvent être reliées entre elles par des **contraintes**, dites contraintes d'intégrité référentielle. Quand le concepteur crée une table, il définit son nom, ses colonnes, sa clé. Le SGBDR crée la structure demandée, ainsi qu'une contrainte sur la colonne clé (pour éviter les clés en double), plus un index sur cette colonne clé.
- Enfin, lorsque le concepteur créer une nouvelle base, le SGBDR crée un **journal** pour mémoriser toutes les actions effectuées sur cette base. L'administrateur de la base pourra définir quel **utilisateur** est habilité à manipuler les données de l'entreprise.


### 3.3. SQL

SQL est donc le langage adapté aux bases de données relationnelles.

Pour que tu maîtrises les requêtes principales de ce langage, nous te demandons de faire les deux derniers chapitres du cours OpenClassrooms. Ils commencent [ici](https://openclassrooms.com/fr/courses/4449026-initiez-vous-a-lalgebre-relationnelle-avec-le-langage-sql/4538696-comprenez-les-bases-de-donnees-sql).

Télécharge la base de données, ainsi que le logiciel SQLiteStudio (si vraiment tu n'arrives pas à le télécharger, tu peux toujours utiliser [SQL Online Compiler](https://sqliteonline.com/)). Lis bien le projet fil rouge autour des Panama Papers car c'est le même jeu de données que tu devras étudier cet après-midi dans ton projet 👁👁.

> Tu te demandes pourquoi tu ne vois qu'une partie du langage SQL (LMD, et plus particulièrement la partie lecture des données) ? En fait, c'est l'action principale qui te sera demandée en tant que Data Analyst : interroger la base de données pour en tirer des informations actualisées. Mais ne t'inquiète pas, on te détaillera les autres tâches dans la journée de demain 😏😏.

A la fin du cours OpenClassrooms, tu auras vu toutes les requêtes principales et tu pourras maintenant pratiquer en pleine autonomie le SQL 😊😊


## 4. Points importants à retenir
- Un modèle relationnel n'est rien de plus qu'une représentation de la réalité. Un non-codeur doit pouvoir comprendre ton schéma relationnel, demande à ton petit cousin de 12 ans ou [regarde la méthode qu'utilisait Feynman](https://www.mieuxpenser.com/articles/la-meilleure-maniere-dapprendre-la-methode-feynman) pour expliquer les concepts compliqués
- Savoir pratiquer SQL. Une "cheet sheet" est toujours utile pour se rappeler de la syntaxe.

![ee](https://www.sqltutorial.org/wp-content/uploads/2016/04/SQL-Cheet-Sheet-1.png)

## 5. Pour aller plus loin
C'est le seul jour de la formation consacré au langage SQL. On a choisi cela car SQL est un langage assez intuitif. Et surtout, avec SQL, les automatismes viennent très vite quand on y est confronté pour de vrai. Donc pas d'inquiétude, tu peux laisser le sujet reposer pour l'instant. 

Quand tu auras besoin de t'exercer davantage pour passer des entretiens ou être vite opérationnel, voici deux ressources pour être au top du SQL :
- Le [cours de W3 Schools](https://www.w3schools.com/sql/), qui contient une doc exhaustive de ce que l'on veut faire en SQL. Très pratique pour vérifier des syntaxes de méthodes.
- Plein d'exercices chez [SQL Zoo](https://sqlzoo.net/wiki/SELECT_basics), idéal pour s'entraîner.
