# Concepts avancés en statistiques

## 1. Introduction
L'analyste de données apporte avant tout une lecture statistique aux problèmes auxquels est confrontée l'entreprise. Pour cela, il va devoir parfois utiliser des concepts statistiques avancés. On peut lui demander par exemple : de réaliser une analyse multi-variée pour comprendre la corrélation entre des variables ou de réaliser un test statistique afin de vérifier une prédiction, ou encore de réaliser une modélisation statistique à l’aide de méthodes d’apprentissage supervisé et non supervisé. En sachant que les sujets statistiques sont trop variés pour être tous couverts ici, nous verrons dans cette ressource les  méthodes les plus courantes 💆‍♀️💆‍♂️

## 2. Historique et contexte
L'avènement de l'informatique dans les années 40 (aux États-Unis), puis en Europe (dans les années 60) permit de traiter un plus grand nombre de données, mais surtout de croiser entre elles des séries de données de types différents. C'est le développement de ce qu'on appelle l'analyse multidimensionnelle : on étudie les relations entre plus de 2 variables à la fois !

Et c’est ici qu’il faudra réveiller votre âme d’explorateur ! En effet, vous partirez à la découverte d'espaces inexplorés, des espaces que le cerveau de l’homme ne peut même pas appréhender, car ce sont des espaces qui possèdent souvent plus de 3 dimensions… 🕵️‍♂️🕵️‍♂️

## 3. La ressource

### 3.1. Manipuler des données dans un espace multidimensionnel

#### 3.1.1. L'Analyse en Composantes Principales (ou ACP) : pour les variables quantitatives continues

L'ACP est une notion qui peut être difficile à comprendre théoriquement mais très utile dans la pratique. On t'a trouvé plusieurs ressources aux niveaux différents pour que tu puisses choisir le niveau de difficulté qui te convient le mieux : 
- cet [article](https://datascientest.com/acp) résume l'intérêt de l'ACP
- ce [cours chapitre 1](https://www.math.univ-toulouse.fr/~baccini/zpedago/asdm.pdf) explique bien l'ACP sans rentrer dans trop de détails mathématiques
- le [cours d'OC](https://openclassrooms.com/fr/courses/4525281-realisez-une-analyse-exploratoire-de-donnees/5280368-comprenez-lenjeu-de-lanalyse-en-composantes-principales) si tu veux avoir les détails mathématiques.

___

👽👽 A quoi ça sert concrètement ? 👽👽

Voici quelques exemples de situations où l’ACP peut être intéressante:
- comparer des équipes de hockey sur la base de 6 statistiques de fin de saison;
- comparer la criminalité entre états sur la base des taux de 7 types de crimes différents;
- compresser des images formées de 1084×1084 pixels;
- identifier le nombre de variantes d’un type de tumeur à partir du degré d’expression de millions de gènes;
- analyser les réponses à un questionnaire sur la personnalité.
___

##### 3.1.2. L'Analyse Factorielle des Correspondances (AFC) et l'Analyse des Correspondances Multiples (ACM) : pour les variables catégorielles

Au chapitre précédent tu as vu que l’analyse en composantes principales (ACP) pouvait permettre de visualiser, de découvrir une structure ou réduire la dimension d’ensembles de plusieurs variables continues. Dans ce chapitre, tu verras comment il est aussi possible de le faire lorsque les variables sont catégorielles, par exemple des variables rapportées dans des tableaux de contingences ou des réponses à des questionnaires à choix multiples.

L’analyse des correspondances est une méthode d’origine française (vous trouverez beaucoup de documentation en français!). Elle permet de représenter graphiquement des **tableaux de fréquences**. On verra deux familles de méthodes:
- analyse des correspondances binaires: pour des tableaux de fréquences croisant deux variables;
- analyse des correspondances multiples: pour des tableaux faisant intervenir trois variables ou plus.

Tu peux retrouver le même cours que précédemment [ici](https://www.math.univ-toulouse.fr/~baccini/zpedago/asdm.pdf) et suivre les chapitres 2 et 3. Enfin, tu peux confirmer ces connaissances avec une vidéo sur l'[AFC en 6 minutes](https://www.youtube.com/watch?v=tEc5cmlQVdI), ainsi qu'une vidéo sur l'[ACM en 6 minutes](https://www.youtube.com/watch?v=bihScz3OXbw).

#### 3.1.2. Partitionner des données



#### 3.1.3. L'analyse discriminante



### 3.2. Estimation et tests statistiques

Regarder sur OpenClassrooms ce qui doit être connu

cours OC : https://openclassrooms.com/fr/courses/4525306-initiez-vous-a-la-statistique-inferentielle/4993371-familiarisez-vous-avec-deux-cas-pratiques


### 3.3. Régression

cf. chapitre 4 : https://certis.enpc.fr/~dalalyan/Download/Poly2.pdf

cf. chapitre 7 du cours Udemy

### 3.4. Tests d'adéquation

A voir si utile

cf. chapitre 5 : https://certis.enpc.fr/~dalalyan/Download/Poly2.pdf


## 4. Points importants à retenir
La ressource en quelques points importants.

https://edutechwiki.unige.ch/fr/Principes_de_base_d%27analyse_statistique

## 5. Pour aller plus loin
https://moncoachdata.com/blog/6-distributions-de-probabilite-data-science/
La journée de data science prévue lors de la quatrième semaine vous permettra également de revoir les méthodes d'apprentissage automatique.
