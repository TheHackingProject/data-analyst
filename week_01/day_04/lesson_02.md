# Modéliser une base de données relationnelle


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







## 1. Introduction
Une introduction sur la ressource.

## 2.Historique et contexte
Cette partie peut être plus ou moins longue. Elle explique l'histoire ou le contexte sur la notion que l'on veut enseigner.

## 3. La ressource
Cette partie est le nerf de la ressource, elle expliquera les notions de cette ressource.


La modélisation permet d'avoir un langage commun. 
Le schéma Entité/Relation
La représentation entité-association : Merise
Entité-association : UML


Expliquer les 3 types de modélisation

https://odile-papini.pedaweb.univ-amu.fr/sources/BD/cours-BD-2.pdf


### 3.1. Première sous partie
blabla

### 3.2. Deuxième sous partie
blabla

## 4. Points importants à retenir
La ressource en quelques points importants.

## 5. Pour aller plus loin
Quelques éléments en ligne pour aller plus loin
