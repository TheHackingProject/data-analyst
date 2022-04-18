# Modéliser et créer une base de données

## 1. Introduction

Avant de créer une base de données, il est important de la modéliser (cad la représenter sous forme de schéma).

📌 *Utilité pour le projet* : 5/5<br/>
📊 *Utilité pour être Data Analyst* : 2/5<br/>
💡 *Pourquoi cette ressource ?* : Pour que tu saches lire les schémas de base de données sans aucun problème.

## 2. Historique et contexte
Peter Chen a développé les modèles **entité-association** pour la conception de bases de données dans les années 1970. Alors qu'il travaillait comme professeur assistant au MIT, il a publié en 1976 un article précurseur intitulé « The Entity-Relationship Model: Toward a Unified View of Data » (Le modèle entité-association : vers une vision unifiée des données).

A la même époque à peu près, la méthode d'analyse et de conception de systèmes **Merise** a été élaborée par un collectif français en 1979. Elle a fourni un cadre méthodologique et un langage commun et rigoureux à toute une génération d'informaticiens français.

Par la suite, le monde a changé et un autre standard s’est imposé, tout en gardant certains principes de la méthodologie Merise. Au milieu des années 90, les *Three Amigos* (Grady Booch, Ivar Jacobson and James Rumbaug) se sont associés pour apporter plus de clarté aux programmeurs en créant de nouvelles normes. Les efforts de ces penseurs ont abouti à la création en 1996 d'**UML**, un langage de modélisation commun.

Finalement, ces 3 standards se ressemblent et peuvent être retrouvés aujourd'hui dans les projets informatiques. L'essentiel reste que les parties prenantes du projet se comprennent ! 

## 3. La ressource

### 3.1 Modéliser une BDD

- Pour approfondir la modélisation de bases de données classique, cf. le cours [Modélisez et implémentez une base de données relationnelle avec UML](https://openclassrooms.com/fr/courses/4055451-modelisez-et-implementez-une-base-de-donnees-relationnelle-avec-uml)


### 3.2 Créer une BDD relationnelle

Une fois que tu as modélisé la base, c'est assez simple de la créer. C'est le travail généralement du développeur mais on t'explique ça ici car ça peut être utile (si tu te lances dans l'entrepreneuriat par exemple).

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


## 5. Pour aller plus loin

