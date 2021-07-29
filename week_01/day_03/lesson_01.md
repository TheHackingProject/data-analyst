# SQL pour débutants

Aujourd'hui nous allons découvrir les bases de données et SQL.

## 1. Introduction
Quand tu crées des applications web, il est indispensable de stocker les données (utilisateurs, potins, etc.) quelque part. Dans cette ressource nous allons t'apprendre comment fonctionnent les bases de données avant de voir pourquoi et comment lier des tables (morceaux de bases de données) entre elles. À l'avenir, nous nous focaliserons uniquement sur SQL quand il s'agira de bases de données : c'est LE langage de référence pour leur gestion.

Après quelques démonstrations du fonctionnement de SQL, tu devrais :

Savoir comment marche une base de données, un élément que tu retrouveras dans TOUTE application web ;
Avoir un aperçu du quotidien d'un Data Scientist, un métier très hype en ce moment où on passe ses journées à miner dans des BDD.
SQL étant omni-présent en informatique, cette journée est plus qu'un simple détour de culture générale... BDD, à toi de jouer !

## 2. Historique
Très rapidement dans l'informatique, nous eûmes besoin de stocker les informations, traitées par nos programmes, quelque part : ainsi furent créées les bases de données. En 1970, un certain Edgar Codd, ingénieur chez IBM, a inventé un moyen de lier en base des tables entre elles. Ainsi, une entrée, comme un Gossip, pourrait être lié à une autre entrée, par exemple en le faisant appartenir à un User. Ce modèle de base de données relationnelle a révolutionné l'informatique puisqu'aujourd'hui, il reste le format le plus répandu dans les applications.

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

#### 3.1.2. La base de données relationnelle
Prenons l'exemple d'une base de données contenant une table de professeurs. Chaque professeur a des attributs comme un nom, un téléphone, etc. Mais on aimerait aussi que notre professeur donne des cours. Chaque cours aura une heure de début, un nom, etc. Plutôt que de faire une gigantesque table contenant chaque professeur et ses cours, il est plus simple d'avoir deux tables distinctes : une pour les profs (nommée teachers) et une pour les cours (nommée classes). Ensuite, pour savoir quel professeur donne quel cours, ça serait top de pouvoir lier les tables entre elles comme le schéma ci-dessous :



En y regardant de plus près, nous n'aurons pas pu mettre toutes ces informations dans une seule table car chaque professeur peut avoir N cours. Parfois il en a un seul (N=1), parfois aucun (N=0), parfois dix (N=10). Il est donc impossible de mettre toutes les informations d'un professeur sur une seule ligne de la table teachers car on ne connaît pas le nombre de colonnes nécessaires (vu qu'il n'y a pas de nombre maximum de cours qu'un prof peut avoir).

Au final, c'est un cas qu'on rencontre couramment quand on fait face à des BDD complexes : on doit créer des tables et les lier entre elles. C'est ce que l'on appelle les bases de données relationnelles.
Dans cette vidéo de O'Reilly, tu pourras comprendre ce qu'est qu'une base de données relationnelle.

Il existe trois types de relations entre les tables d'une base de données :

Relation 1-1 : Assez rare, elle sert à modéliser l'exclusivité. Par exemple : dans une hypothétique base de données "session THP en cours", un moussaillon a un unique ordinateur et chaque ordinateur appartient à un moussaillon. Bref, c'est du 1-1 entre 2 tables cabin_boys et computers.
Relation 1-N : Très courante, elle sert à modéliser une appartenance. Par exemple : dans une hypothétique base de données "France", chaque habitant vit dans une ville unique mais chaque ville a plusieurs habitants. C'est du 1-N entre la table cities et la table people.
Relation N-N : Très courante aussi, elle permet de modéliser un lien mais sans aucune unicité. Par exemple : un docteur a plusieurs patients et un patient peut avoir plusieurs docteurs. C'est du N-N entre la table doctors et la table patients.
3.1.3. Penser une base de données
Avant de foncer tête baissée dans le codage d'une BDD, il est important de bien la modéliser pour voir les différents éléments qui vont la composer. Sans une vision globale et un dessin de ta BDD entière, tu vas forcément oublier quelque chose et t'en mordre les doigts plus tard.
Voici les 3 éléments que tu vas devoir lister pour modéliser ta BDD à tête reposée :

Les tables : ce sont les tableaux qui composeront ta base de données. C'est ce qui demande le plus de réflexion mais qui t'aidera à poser des concepts concrets sur des thèmes abstraits. Tu verras plus tard qu'au final, une table (SQL) et un objet (Ruby) sont très liés... Exemples de tables : users, orders, cities, articles, etc.
Les relations entre tables : il vous faut établir quelles tables sont liées entre elles et via quelle relation (1-1, 1-N et N-N). En général, cette réflexion vient en même temps que celles où on détermine les tables. Par exemple : relation 1-N entre users et cities (un utilisateur vit dans une ville, une ville peut être lié à plusieurs utilisateurs), relation N-N entre users et les items (un utilisateur peut acheter plusieurs articles et chaque article peut avoir été acheté par plusieurs utilisateurs), etc.
Les attributs de chaque table : ce sont en gros les colonnes qui définissent chaque entrée d'une table. Par exemple, dans une table users on aura : first_name, gender, email, phone etc.
Cette phase de réflexion doit être menée en équipe et sans ordinateur. Plusieurs choix :

Sur un tableau blanc, éventuellement à l'aide de post-its ;
En faisant un gros diagramme sur une feuille A4 avec un bon vieux stylo ;
N'hésite pas à utiliser un logiciel d'ERD pour t'aider. Voici une liste :
LucidChart
VisualParadigm Online
DB Diagram.io
Entraîne-toi ! Imagine des idées de startup puis fais un diagramme via un ERD.

### 3.2. SQL
#### 3.2.1. Découverte de SQL
Afin d'interagir avec la base de données, nous allons utiliser le langage SQL ou "Structured Query Language" qui permet facilement d'en récupérer les informations.
Pour créer notre première base de données sur notre machine, nous allons utiliser SQLite3. Pour l'installer :

Sur Ubuntu, fait :
$ sudo apt-get install sqlite libsqlite3-dev
Sur macOS, fait :
$ brew install sqlite
Une fois le logiciel installé, crée un dossier de test, va dedans et rentre :

$ sqlite3 db.sqlite
Cela va créer un fichier nommé db.sqlite qui est ta base de données (⚠️ le fichier ne sera sauvegardé que lorsqu'une table sera créée dedans). Au passage, cela te fait rentrer dans l'interface SQLite3 depuis laquelle tu vas pouvoir passer des commandes SQL sur la BDD.
Pro-tip : Pour sortir de SQLite3, le raccourci est ctrl-D et non ctrl-C.

Pour créer ta première table, voilà la syntaxe à saisir dans l'interface SQLite3 :

CREATE TABLE `doctors` (
`id` INTEGER PRIMARY KEY AUTOINCREMENT, 
`name` TEXT,
`age` INTEGER,
`specialty` TEXT
);
Cette commande va créer une table doctors, avec son fameux id et les valeurs name (un nom sous forme de texte), age (un âge sous forme d'entier) et specialty (une spécialité sous forme de texte).
Avec la commande AUTOINCREMENT, on laisse la base de données s'occuper de l'incrémentation automatique de l'id : à chaque fois qu'une entrée sera créée dans la table doctors, elle portera un nouvel id (égal au dernier id + 1).

🚀 ALERTE BONNE ASTUCE
Les commandes suivantes permettront de visualiser plus facilement le contenu de ta table quand tu taperas la commande SELECT * FROM doctors. Saisis-les une fois dans l'interface de SQlite3 :

.mode column
.headers on
La commande suivante permet de lister toutes les tables qui ont déjà été créées dans ton fichier de base de données.

.tables
Une dernière astuce pour afficher simplement toutes les colonnes d'une table donnée. Il faut que tu ais activé le mode .headers on. Ensuite fais :

SELECT * FROM TableName LIMIT 1;
Cela affichera la première ligne du tableau et donc l'ensemble du header au-dessus.

#### 3.2.2. Faire du CRUD en SQL
Qu'est-ce que le CRUD ? Ce sont les 4 grandes actions qu'on voudra effectuer sur les entrées d'une BDD :

Create : créer une nouvelle entrée dans une table. Il faut utiliser la commande INSERT ;
Read : lire les entrées d'une table. Il faut utiliser la commande SELECT ;
Update : mettre à jour une entrée d'une table. Il faut utiliser la commande UPDATE ;
Delete : supprimer une entrée. Il faut utiliser la commande DELETE.
Ci-dessous, quelques exemples concrets.

Pour créer un docteur dans notre base de données il suffit d'écrire :

INSERT INTO doctors (name, age, specialty) VALUES ('Dr. Dolladille', 45, 'Dentist');
Pour lire l'ensemble des éléments de la table doctors (comme on l'a vu ci-dessus) la commande est :

SELECT * FROM doctors;
Si on veut sélectionner un élément en particulier on peut écrire :

SELECT * FROM doctors WHERE age = 45;
Pour mettre à jour un paramètre, la commande est la suivante :

UPDATE doctors SET age = 40, name = 'John Smith' WHERE id = 3;
Et enfin pour supprimer un élément :

DELETE FROM doctors WHERE id= 3;

#### 3.2.3. Les tables jointes
Nous t'avons présenté la logique des BDD relationnelles. Quand deux tables sont liées par une relation (par exemple 1-N), on parle alors de tables jointes ("join tables" en anglais). Illustrons cela en imaginant deux tables :

La table cities:

id	name
1	Paris
---	---
2	London
---	---
3	Washington D.C.
---	---
4	Rome
---	---
Et la table inhabitants:

id	city_id	first_name	last_name	age
1	3	Donald	Trump	71
---	---	---	---	---
2	4	Matteo	Renzi	43
---	---	---	---	---
3	1	Emmanuel	Macron	40
---	---	---	---	---
4	2	Theresa	May	61
---	---	---	---	---
On peut voir immédiatement que ces deux tables sont liées puisque dans la table inhabitants, j'ai deux clés uniques :

La clé id, aussi appelée clé primaire ou primary key.
La clé city_id, aussi appelée clé étrangère ou foreign key.
C'est la clé étrangère qui permet la liaison entre les deux bases de données. Ainsi, on voit que dans la table inhabitants, l'entrée "Donald Trump" a un attribut city_id = 3 : cette entrée est donc liée à l'entrée portant l'id = 3 dans la table cities. Au final, on a juste indiqué ici que Donald Trump habitait Washington DC.

La force de la relation est qu'il est possible de faire une requête SQL qui me retourne les entrées de la table inhabitants selon un critère de la table cities. Par exemple, pour récupérer les habitants de Paris, il suffit d'écrire :

SELECT * FROM inhabitants
JOIN cities ON cities.id = inhabitants.city_id
WHERE cities.name = 'Paris';
Ici j'ai dit de joindre la table cities tel que l'id que je trouve dans la table cities (cities.id) est le même que le city_id qui se trouve dans la table inhabitants (identifié par inhabitants.city_id).

#### 3.2.4. Plus d'infos sur les relations N-N
Les relations les plus complexes sont les relations N-N. Pour mieux les comprendre voici quelques articles intéressants :

sur Tech Diaries
et sur le CERIG

## 4. Points importants à retenir
Les bases de données relationnelles sont la base de la majorité des applications. Pour concevoir une BDD relationnelle, SQL est le langage de prédilection.

Avant de coder une BDD, il faut se poser pour établir toutes les tables, les relations entre elles et leurs attributs.

Voici une sélection de commandes classiques en SQL :

Créer une table :
CREATE TABLE `doctors` (
`id` INTEGER PRIMARY KEY AUTOINCREMENT, `name` TEXT,
`age` INTEGER,
`specialty` TEXT
);
Créer une entrée dans une table :
INSERT INTO doctors (name, age, specialty) VALUES ('Dr. Dolladille', 45, 'Dentist');
Lire des éléments (avec ou sans critère de sélection) :
SELECT * FROM doctors;
SELECT * FROM doctors WHERE age = 45;
Mettre à jour une entrée :
UPDATE doctors SET age = 40, name = 'John Smith' WHERE id = 3;
Supprimer une entrée :
DELETE FROM doctors WHERE id= 3;
Lire les éléments d'une table selon un critère d'une table liée :
SELECT * FROM inhabitants
JOIN cities ON cities.id = inhabitants.city_id
WHERE cities.name = 'Paris';

## 5. Pour aller plus loin
Voici quelques ressources pour être au top du SQL.

Le cours de W3 Schools, qui contient une doc exhaustive de ce que l'on veut faire en SQL. Très pratique pour vérifier des syntaxes de méthodes.
Plein d'exercices chez SQL Zoo, idéal pour s'entraîner et se sentir un Data-Analyst
SQL avec des exercices
