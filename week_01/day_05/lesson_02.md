# Modéliser et créer une base de données

## 1. Introduction
Avant de foncer tête baissée dans le codage d'une BDD, il est important de bien la modéliser pour voir les différents éléments qui vont la composer. Sans une vision globale et un dessin de ta BDD entière, tu vas forcément oublier quelque chose et t'en mordre les doigts plus tard.

## 2. Historique et contexte
Peter Chen a développé les modèles **entité-association** pour la conception de bases de données dans les années 1970. Alors qu'il travaillait comme professeur assistant à la Sloan School of Management du MIT, il a publié en 1976 un article précurseur intitulé « The Entity-Relationship Model: Toward a Unified View of Data » (Le modèle entité-association : vers une vision unifiée des données).

A la même époque à peu près, la méthode d'analyse et de conception de systèmes **Merise** a été élaborée par un collectif français en 1979. Elle a fourni un cadre méthodologique et un langage commun et rigoureux à une génération d'informaticiens français.

Par la suite, le monde a changé et un autre standard s’est imposé, tout en gardant certains principes de la méthodologie Merise. Au milieu des années 90, les *Three Amigos* (Grady Booch, Ivar Jacobson and James Rumbaug) se sont associés pour apporter plus de clarté aux programmeurs en créant de nouvelles normes. Les efforts de ces penseurs ont abouti à la création en 1996 d'**UML**, un langage de modélisation commun.

Finalement, Merise et UML se basent sur un schéma Entité-Relation. En fait, ces 3 standards peuvent être retrouvés aujourd'hui dans les projets informatiques car l'essentiel reste que les parties prenantes du projet se comprennent ! 

## 3. La ressource

### 3.1 Modéliser une BDD

En fait, la modélisation permet avant tout d'avoir un langage commun. 

Un diagramme entité-association est un type d'organigramme illustrant la façon dont des « entités » telles que des personnes, objets ou concepts sont liées les unes aux autres au sein d'un système. Les diagrammes entité-association sont généralement utilisés pour concevoir des bases de données relationnelles. Appelés *ERD* en anglais, ils utilisent une série de symboles prédéfinis tels que des rectangles, losanges et ovales reliés par des lignes pour décrire les interconnexions entre les entités, leurs relations et leurs attributs. Ils imitent une structure grammaticale, où les entités sont des noms et les relations des verbes. Voici un exemple de diagramme entité-association :

![ex](https://d2slcw3kip6qmk.cloudfront.net/marketing/pages/i18n/fr/ER-diagram-images/Exemple-de-diagramme-entite-association-de-base-dedonnees.png)

Voici les 3 éléments que tu vas devoir lister pour modéliser ta BDD à tête reposée :
- **Les tables** : ce sont les tableaux qui composeront ta base de données. C'est ce qui demande le plus de réflexion mais qui t'aidera à poser des concepts concrets sur des thèmes abstraits. Tu verras plus tard qu'au final, une table (SQL) et un objet (Python) sont très liés... Exemples de tables : users, orders, cities, articles, etc.
- **Les relations entre tables** : il vous faut établir quelles tables sont liées entre elles et via quelle relation (1-1, 1-N et N-N). En général, cette réflexion vient en même temps que celles où on détermine les tables. Par exemple : relation 1-N entre users et cities (un utilisateur vit dans une ville, une ville peut être lié à plusieurs utilisateurs), relation N-N entre users et les items (un utilisateur peut acheter plusieurs articles et chaque article peut avoir été acheté par plusieurs utilisateurs), etc.
- **Les attributs de chaque table** : ce sont en gros les colonnes qui définissent chaque entrée d'une table. Par exemple, dans une table users on aura : first_name, gender, email, phone etc.

Cette phase de réflexion doit être menée en équipe et sans ordinateur. Plusieurs choix :
- Sur un tableau blanc, éventuellement à l'aide de post-its ;
- En faisant un gros diagramme sur une feuille A4 avec un bon vieux stylo ;

N'hésite pas à utiliser un logiciel d'ERD (*Entity Relation Diagram*) pour t'aider. Voici une liste :
[LucidChart](https://www.lucidchart.com/),
[VisualParadigm Online](https://online.visual-paradigm.com/fr/),
[DB Diagram.io](https://dbdiagram.io/d).

Entraîne-toi ! Imagine des idées de startup puis fais un diagramme via un *ERD*. En tant que Data Analyst, tu seras amené à relire et comprendre ces schémas de bases de donées. 


### 3.2 Créer une BDD relationnelle

Une fois que tu as modélisé la base, c'est assez simple de la créer, et ça peut être utile (si tu te lances dans l'entrepreneuriat par exemple).

Le premier chapitre du cours OpenClassrooms [Implémentez vos bases de données relationnelles avec SQL](https://openclassrooms.com/fr/courses/6971126-implementez-vos-bases-de-donnees-relationnelles-avec-sql) t'indique comment faire. Si ça t'intéresse, va jusqu'au quiz *Créez une base de données avec MySQL*. 

Et voici une sélection des commandes les plus utiles en SQL :

- Créer une table :
```sql
CREATE TABLE `doctors` (
`id` INTEGER PRIMARY KEY AUTOINCREMENT, `name` TEXT,
`age` INTEGER,
`specialty` TEXT
);
```

- Créer une entrée dans une table :
```sql
INSERT INTO doctors (name, age, specialty) VALUES ('Dr. Dolladille', 45, 'Dentist');
```

- Lire des éléments (avec ou sans critère de sélection) :
```sql
SELECT * FROM doctors;
SELECT * FROM doctors WHERE age = 45;
```

- Mettre à jour une entrée :
```sql
UPDATE doctors SET age = 40, name = 'John Smith' WHERE id = 3;
```

- Supprimer une entrée :
```sql
DELETE FROM doctors WHERE id= 3;
```

- Lire les éléments d'une table selon un critère d'une table liée :
```sql
SELECT * FROM inhabitants
JOIN cities ON cities.id = inhabitants.city_id
WHERE cities.name = 'Paris';
```


## 4. Points importants à retenir
Les bases de données relationnelles sont la base de la majorité des applications. Pour concevoir une BDD relationnelle, SQL est le langage de prédilection.

Avant de coder une BDD, il faut se poser pour établir toutes les tables, les relations entre elles et leurs attributs. 

Il faut également se demander s'il s'agit d'une base de données opérationnelle ou alors d'un datawarehouse car la modélisation ne sera pas la même. 

Le Data Analyst doit savoir travailler avec les tous les types de bases de données (même si quand le datawarehouse est déjà mis en place, il travaillera principalement sur le système d'info décisionnel). 

## 5. Pour aller plus loin
- Pour approfondir la modélisation de bases de données classique, cf. le cours [Modélisez et implémentez une base de données relationnelle avec UML](https://openclassrooms.com/fr/courses/4055451-modelisez-et-implementez-une-base-de-donnees-relationnelle-avec-uml)
