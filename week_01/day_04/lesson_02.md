# Modéliser et créer une BDD relationnelle

## 1. Introduction
Avant de foncer tête baissée dans le codage d'une BDD, il est important de bien la modéliser pour voir les différents éléments qui vont la composer. Sans une vision globale et un dessin de ta BDD entière, tu vas forcément oublier quelque chose et t'en mordre les doigts plus tard.

## 2.Historique et contexte
**Merise** est une méthode d’analyse et de conception de systèmes élaborée par un collectif en 1979. Cette méthode s’est rapidement imposée comme un standard dans les projets informatiques. Elle a fourni un cadre méthodologique et un langage commun et rigoureux à une génération d'informaticiens français.

Par la suite, le monde a changé et un autre standard s’est imposé. Au milieu des années 90, les *Three Amigos* (Grady Booch, Ivar Jacobson and James Rumbaug), se sont associés pour apporter plus de clarté aux programmeurs en créant de nouvelles normes. Les efforts de ces penseurs ont abouti à la création en 1996 d'**UML**, un langage de modélisation commun.

Néanmoins, l'héritage Merise est très important notamment en ce qui concerne l'importance de la modélisation, principe d'abstraction.


## 3. La ressource


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










La modélisation permet d'avoir un langage commun. 
Le schéma Entité/Relation
La représentation entité-association : Merise
Entité-association : UML


Expliquer les 3 types de modélisation

https://odile-papini.pedaweb.univ-amu.fr/sources/BD/cours-BD-2.pdf


## 4. Points importants à retenir
La ressource en quelques points importants.

## 5. Pour aller plus loin
Quelques éléments en ligne pour aller plus loin
