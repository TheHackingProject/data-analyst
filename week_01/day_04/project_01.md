# Concevoir des bases de données

## 1. Introduction
Pour concevoir une bonne base de données, il faut bien comprendre le business concerné. Donc on fera souvent appel au Data Analyst pour réaliser la modélisation de la base ou pour vérifier que rien n'a été oublié. Avant que ça soit ton tour, profite de ce projet pour t'exercer et devenir un as de la modélisation de bases de données 🦁

## 2. Le projet
### 2.1. La startup tech du moment
Ça y est, tu tiens la prochaine licorne française, tu vas conquérir le monde avec une app qui va révolutionner le monde du blogging. Ça va tout déchirer et Mark Zuckerberg va chialer. Avant de faire le code de ton blog, nous allons te demander de concevoir la base de données de ce dernier. 3nsuite, tu vas devoir créer, en SQL les tables qui constitueront ta BDD avec leurs relations et leurs attributs.

Voici, sans plus tarder, l'architecture de ton app de blogging :

- L'application va accueillir plusieurs `user` et ils auront tous un nom.
- Chaque `user` peut créer plusieurs `article` et chaque `article` est forcément créé par un `user`.
- Un `article` peut appartenir à plusieurs `category` et chaque `category` peuvent avoir plusieurs `article`. Chaque `category` a un titre.
- Une catégorie peut appartenir à plusieurs tag ; chaque `tag` a un titre et une couleur.

Utilise SQL pour créer cette base de données, ainsi que les tables correspondantes.

A présent, tu vas créer un élément de chaque table : un `user`, un `article`, une `category` et un `tag`.

### 2.2. Concepts de sites et base de données
Ce premier exercice sur un blog a permis de bien t'échauffer et de réviser la création de base de données en langage SQL. Mais la partie la plus complexe est de concevoir l'architecture complète de la BDD : en te guidant sur le blog, on t'a évité cette étape.

À présent c'est ton tour ! On va te décrire un concept et c'est à toi de concevoir la BDD de A à Z. Liste (à tête reposée) les différentes tables, attributs, et jointures pour les sites ci-dessous. Tu n'auras pas besoin de les créer en SQL, mais juste de les concevoir, dans un fichier .txt par exemple.

#### 2.2.1. MOOCademy
Tu dois créer une plateforme d'apprentissage en ligne. Il y a plein de cours. Chaque cours a un titre et une description. Enfin, chaque cours a plusieurs leçons, qui ont un titre et un body.

#### 2.2.2. The Hacking Pinterest
Tu veux faire de la concurrence à Pinterest, donc tu voudrais créer un site où les utilisateurs peuvent créer des "pins". Chaque pin contient l'URL d'une image sur le net. Les utilisateurs peuvent commenter les pins, mais ne peuvent pas commenter les commentaires.

#### 2.2.3. The Hacking News
Tu veux créer un message board à la Hacker News. Les utilisateurs peuvent poster des liens. Les autres utilisateurs peuvent commenter les liens soumis, ou commenter les commentaires (mais on ne peut pas aller plus loin qu'un commentaire de commentaire). Comment faire en sorte qu'un commentaire sache où dans la hiérarchie il se trouve ? 🤔

#### 2.2.4. The Hacking Class
Tu vas encore faire un site d'éducation en ligne. Dans ce site il y aura des élèves qui peuvent s'inscrire à un seul cours. Un cours pourra avoir plusieurs élèves.

## 3. Rendu attendu
- Un fichier .sql ontenant la BDD de ton appli de blog.
- Un fichier .txt (ou .md) ou diagramme ERD avec la structure de chaque BDD (blog, MOOCacademy, Hackinterest, Hacking News, Hacking Class).
