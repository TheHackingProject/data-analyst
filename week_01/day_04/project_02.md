# Jouer avec une base NoSQL
Ca c'est vraiment la classe 🔮🔮

## 1. Introduction
Dans ce projet, tu vas utiliser MongoDB 🎉🎉 Développé en 2007, MongoDB est depuis devenu un des SGBD les plus utilisés. Selon le classement *DB-Engines Ranking*, MongoDB se classe en cinquième position des serveurs de données les plus populaires au niveau mondial. Première technologie NoSQL de ce palmarès, l'infrastructure open source de MongoDB se hisse juste derrière les principaux systèmes phares de base relationnelle : Oracle Database, MySQL, SQL Server et PostgreSQL - avec lequel elle est au coude-à-coude.

![ranking](https://lh3.googleusercontent.com/hK6ISsEifSkk4fUl7V5lVvc87Bpce-q45uzX68S6fNwoW9__ysAflqBHFFZ5UcCP3K-uNlaqx9nL_0DsYFetgqcMhVAui7M0oDlkBRRgEs52EqtkTfATf1ZdetFYtKZbCYQVg8yO)

## 2. Le projet
### 2.1. Créer un cluster sur MongoDB Atlas
Un cluster est un groupe de deux ou plusieurs serveurs indépendants fonctionnant comme un système unique.
Et MongoDB Atlas est une version cloud entièrement gérée de la base de données. Cela va nous aider car autrement, les tâches nécessaires, telles que l’installation de la base de données, son réglage pour maintenir des performances optimales sur de longues périodes et sa sécurisation, ont tendance à demander beaucoup d’efforts spécialisés ... 

Avec MongoDB Atlas, tu vas pouvoir créer un cluster MongoDB auprès de tout fournisseur de cloud majeur de votre choix et commencer à utiliser ce cluster en quelques minutes.

- Tout d'abord, tu dois te créer un compte sur [MongoDB Atlas](https://account.mongodb.com/account/register).
- Ensuite, tu te connectes, tu crée un cluster et tu lui donnes un nom. Choisis la version Free.
- Puis, tu crées un utilisateur de base de données.
- Tu ajoutes les adresses IP qui peuvent se connecter à ta base de données. Choisis que le serveur est accessible partout.
- Tu connectes le cluster à MongoDB Compass.


### 2.2. Télécharger MongoDB Compass
- Télécharge l'outil graphique [MongoDB Compass](https://www.mongodb.com/try/download/compass), tu l'ouvres et tu le connectes à ton cluster en collant l'url de connexion obtenu précédemment (en changeant 'password' par le mot-clé qui avait été saisi lors de la création de l'utilisateur.
- Crée une base de données 'demo' et une collection 'publis'.
- Télécharge les données disponibles [ici](http://b3d.bdpedia.fr/files/dblp/json.zip). Il s'agit d'un extrait de la base de données DBLP (*Digital Bibliography & Library Project*), un catalogue de bibliographies en informatique disponible en ligne.
- Dézippe le fichier et importe le à ta base de données.

### 2.3. Requêter la base de données
Ca y est tu as maintenant une base de données disponible sur MongoDB. A toi de faire les requêtes suivantes : 
- Vérifier le nombre de documents importés.
- Prévisualiser les 20 premiers documents.
- Lister tous les livres (type 'Book').
- Lister les publications depuis 2011.
- Lister toutes les publications de 2011 et 2013.
- Lister toutes les publications de 2011 ou 2013.
- Lister les publications ayant 3 auteurs.
- Lister les livres publiés depuis 2014.
- Lister les publications de l'auteur "Toru Ishida".
- Lister tous les éditeurs (type 'publisher') distincts.
- Listes tous les auteurs distincts.
- Trier les publications de 'Toru Ishida' par titre de livre et par page de début.
- Compter le nombre de ses publications.
- Compter le nombre de publications depuis 2011 et par type.
- Compter le nombre de publications par auteur et trier le résultat par ordre croissant.

Aide [ici](https://openclassrooms.com/fr/courses/4462426-maitrisez-les-bases-de-donnees-nosql/4474606-interrogez-vos-donnees-avec-mongodb).

## 3. Rendu attendu
Un fichier texte qui donne l'ensemble des requêtes pour obtenir les réponses.
