# Notions de base en statistique

## 1. Introduction
On va reprendre dans cette ressource les notions qu'il faut maîtriser pour réussir ses analyses de données. Tu as déjà dû voir ça plusieurs fois dans ton cursus éducatif mais ça fait toujours du bien de reprendre ces notions qui sont omniprésentes dans notre quotidien ✍️

## 2. Historique et contexte
L'origine du mot "statistique" remonte au latin classique *status* (état) qui, par une série d'évolutions successives, aboutit au français "statistique", attesté pour la première fois en 1771.

Les statistiques (des grandeurs calculées à partir d'observations recueillies) sont nées de l’activité de recueil des données répondant aux besoins d’organisation et de gouvernement des grands empires (armée, impôts, organisation des richesses). Par exemple, les premiers recensements ont eu lieu vers 3000 ans avant notre ère en Sumérie.

Mais on distingue généralement les statistiques (au pluriel) de la statistique. Le second sens n'apparaît que vers 1830. On peut définir la statistique comme domaine d'étude : un ensemble de techniques d'interprétation mathématique appliquées à des phénomènes pour lesquels une étude exhaustive de tous les facteurs est impossible à cause de leur grand nombre ou de leur complexité 📊📊

## 3. La ressource

### 3.1. Vocabulaire de base

### 3.1.1. Quelques rappels

- L’ensemble de personnes ou d’objets équivalents étudié s’appelle la **population**. 
- Chaque objet d’une population s’appelle un **individu** ou une **unité statistique**. 
- Les caractéristiques que l’on mesure s’appellent des **variables**. Les mesures s’appellent des **observations**. La série d’observations recueillies s’appelle **série statistique**. Elle est généralement retranscrite dans un tableau de données.

Il existe différents types de variables : 
- les variables **quantitatives**: elles prennent des valeurs numériques (taille, âge,...). Elles s’expriment par des nombres réels sur lesquels les opérations arithmétiques de base (somme, moyenne) ont un sens. Elles peuvent être **discrètes** (nombre fini ou dénombrable de valeurs) ou **continues** (toutes les valeurs réelles sont susceptibles d’être prises).
- les variables **qualitatives**: elles prennent des valeurs non numériques. Elles peuvent être **nominales** (sexe par ex) ou **ordinales** lorsque l’ensemble des catégories est muni d’un ordre total (très résistant, assez résistant, peu résistant). Les différents niveaux d’une variable qualitative s’appellent des **modalités** (ou catégories).

### 3.1.2. Les différents objectifs de la statistique

On peut scinder la statistique en deux grands domaines :
- la statistique **descriptive** (ou exploratoire) a pour but de structurer et de représenter l'information contenue dans les données.
- la statistique **inférentielle** cherche à induire les caractéristiques d'un groupe général à partir de celles d'un groupe particulier, en fournissant une mesure de la certitude de la prédiction : la probabilité d'erreur.

La statistique descriptive utilise des tableaux (tables de fréquence), des graphiques (box-plots, histogrammes) et des indicateurs (moyenne, corrélation). 
La statistique inférentielle utilise des estimations (approcher des paramètres de la population à partir de l'échantillon), des tests (valider ou infirmer les hypothèses émises sur ces paramètres) et de la modélisation. 

En fait, le rôle des probabilités est nul en statistique descriptive et prépondérant en statistique inférentielle.

___

🔮🔮 QUESTION : les statistiques modernes sont descriptives ou inférentielles ? 🔮🔮

Ca dépend !

D'une part, la statistique descriptive s’est enrichie ces dernières années de nombreuses techniques de visualisation de données multidimensionnelles, connues sous le nom d’analyse des données, ou de *datamining*. Parmi ces méthodes on trouve :
- les méthodes de classification (partitionnement, CAH), visant à réduire la taille de l’échantillon en classant les individus dans des groupes de caractéristiques homogènes.
- les méthodes d’analyse factorielle (ACP, AFCM,...) qui cherchent à réduire le nombre de caractéristiques d’une population en les résumant par un petit nombre de composantes synthétiques.

D'autre part, l'analyse prédictive qui fait partie de la statistique inférentielle, est de plus en plus utilisée. Elle consiste à utiliser des données, des algorithmes statistiques et des techniques de machine learning pour anticiper de probables résultats futurs en fonction des données historiques. L'objectif est d'extrapoler à partir des événements survenus pour mieux prévoir les événements futurs.

___


### 3.2. Les mesures statistiques à connaître

### 3.2.1. L'analyse univariée

Pour revoir les mesures statistiques importantes, je t'invite à faire le [chapitre 2](https://openclassrooms.com/fr/courses/4525266-decrivez-et-nettoyez-votre-jeu-de-donnees/4928081-rencontrez-ulysse-data-analyst-a-openclassrooms) du cours OpenClassrooms *Décrivez et nettoyez votre jeu de données*.

Vous verrez à la suite les mesures de tendance centrale, de dispersion, de forme, de concentration ... et encore d'autres !

### 3.2.2. L'analyse bivariée

Mais jusqu'à présent, tu analysais uniquement une variable. Pour étudier la relation entre deux variables et voir si elles sont liées, il faut faire de l'analyse bivariée. Suis [le chapitre 3](https://openclassrooms.com/fr/courses/4525266-decrivez-et-nettoyez-votre-jeu-de-donnees/4725620-entrez-dans-le-monde-de-l-analyse-bivariee) du cours OpenClassrooms pour voir les méthodes à connaître.

Enfin, tu as peut-être déjà entendu parler de la matrice de corrélation. Elle est utilisée pour évaluer la dépendence entre plusieurs variables en même temps. Le résultat est une table contenant les coefficients de corrélation entre chaque pair de variables. Pour calculer les corrélations sur un ensemble de colonnes, ce n’est pas plus compliqué, il suffit d'appliquer la méthode `.corr` à tout le Dataframe. Et avec une grille de chaleur, cela rendra le résultat plus visible et interprétable. Tu peux check [cette vidéo](https://www.youtube.com/watch?v=UgtjatBt3vY) pour bien comprendre ces concepts 🤗

## 4. Points importants à retenir
Utilisées dans quasiment tous les domaines (biomédical, industriel, bancaire, social…), les statistiques sont devenues depuis ces dernières années accessibles au plus grand nombre d’entre nous. Elles sont aujourd’hui les moyens d’expression privilégiés de toute personne souhaitant faire « parler » une base de données, quel qu’en soit son contenu. Il est important donc de savoir bien les utiliser et d'en connaître leurs limites.

## 5. Pour aller plus loin
- Ce [site](http://www.astro.ulg.ac.be/cours/magain/STAT/Stat_Main_Fr/Chapitre1.html) d'introduction aux statistiques, très axé sur la pratique.
- La chaîne YouTube [StatQuest](https://www.youtube.com/playlist?list=PLblh5JKOoLUK0FLuzwntyYI10UQFUhsY9) et sa partie sur les fondamentaux.
