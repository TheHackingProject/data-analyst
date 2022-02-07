# Concepts avancés en statistiques

## 1. Introduction
L'analyste de données apporte avant tout une lecture statistique aux problèmes auxquels est confrontée l'entreprise. Pour cela, il va devoir parfois utiliser des concepts statistiques avancés. On peut lui demander par exemple : de réaliser une analyse multi-variée pour comprendre la corrélation entre des variables ou de réaliser un test statistique afin de vérifier une prédiction, ou encore de réaliser une modélisation statistique à l’aide de méthodes d’apprentissage supervisé et non supervisé. En sachant que les sujets statistiques sont trop variés pour être tous couverts ici, nous verrons dans cette ressource les  méthodes les plus courantes 💆‍♀️💆‍♂️

📌 *Utilité pour le projet* : 0/5<br/>
📊 *Utilité pour être Data Analyst* : 1/5<br/>
💡 *Pourquoi cette ressource ?* : Simplement pour que tu prennes conscience de l'ampleur du domaine des statistiques. Si tu as envie d'être Data Scientist ou que tu aimes les statistiques, plonge toi sérieusement dans certains de ces concepts avancés. Si non, tu peux clairement passer ton chemin : un Data Analyst n'a pas besoin de connaître tous ces concepts. Ce que je te recommande c'est de lire la ressource aujourd'hui et tu reviendras te former à ces concepts le jour où on te le demandera expressément.


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

#### 3.1.2. L'Analyse Factorielle des Correspondances (AFC) et l'Analyse des Correspondances Multiples (ACM) : pour les variables catégorielles

Au chapitre précédent tu as vu que l’analyse en composantes principales (ACP) pouvait permettre de visualiser, de découvrir une structure ou réduire la dimension d’ensembles de plusieurs variables continues. Dans ce chapitre, tu verras comment il est aussi possible de le faire lorsque les variables sont catégorielles, par exemple des variables rapportées dans des tableaux de contingences ou des réponses à des questionnaires à choix multiples.

L’analyse des correspondances est une méthode d’origine française (vous trouverez beaucoup de documentation en français!). Elle permet de représenter graphiquement des **tableaux de fréquences**. On verra deux familles de méthodes:
- analyse des correspondances binaires: pour des tableaux de fréquences croisant deux variables;
- analyse des correspondances multiples: pour des tableaux faisant intervenir trois variables ou plus.

Tu peux retrouver le même cours que précédemment [ici](https://www.math.univ-toulouse.fr/~baccini/zpedago/asdm.pdf) et suivre les chapitres 2 et 3. Enfin, tu peux confirmer ces connaissances avec une vidéo sur l'[AFC en 6 minutes](https://www.youtube.com/watch?v=tEc5cmlQVdI), ainsi qu'une vidéo sur l'[ACM en 6 minutes](https://www.youtube.com/watch?v=bihScz3OXbw).

#### 3.1.3. Partitionner des données

Pour bien comprendre le partitionnement des données ou *clustering*, vous pouvez réaliser le dernière chapitre du [cours OC](https://openclassrooms.com/fr/courses/4525281-realisez-une-analyse-exploratoire-de-donnees/5254143-recherchez-une-bonne-partition). Et lire [cet article](https://larevueia.fr/clustering-les-3-methodes-a-connaitre/) qui résume les 3 types de méthodes de clustering à connaître.


### 3.2. Estimation et tests statistiques

Tu devrais l'avoir deviné : on n'est plus dans la statistique descriptive mais on est revenus à la statistique inférentielle.
La statistique inférentielle est un monde à elle toute seule. Si tu n'as jamais eu de cours de probabilités, tu dois comprendre les notions importantes d'estimateur, proportion, intervalle de confiance etc. Réalise le cours [Initiez-vous à la statistique inférentielle](https://openclassrooms.com/fr/courses/4525306-initiez-vous-a-la-statistique-inferentielle/4993371-familiarisez-vous-avec-deux-cas-pratiques) pour te mettre à niveau sur toutes ces notions.


### 3.3. Modélisation de données et régression

Idem, les concepts de régression et ANOVA sont complexes. Ils permettent surtout de prédire le futur. Si tu as encore de l'énergie aujourd'hui, tu peux suivre le cours [Réalisez des modélisations de données performantes](https://openclassrooms.com/fr/courses/4525326-realisez-des-modelisations-de-donnees-performantes). Si tu as déjà engrangé trop d'infos, garde le pour un autre jour car ce sont des notions importantes.

Je te mets quand même ici deux cas pratiques de régression linéaires pour que tu voies rapidement de quoi il s'agit : 
- [un article](https://mrmint.fr/regression-lineaire-python-pratique) sur la régression linéaire avec Python
- [une vidéo](https://www.linkedin.com/learning/python-l-analyse-de-donnees/mettre-en-application-la-regression-lineaire) qui présente aussi un cas de régression linéaire.


## 4. Points importants à retenir
La ressource d'aujourd'hui abordait beaucoup de points techniques. Si tu n'es pas fan de maths et de théorie, ce n'était probablement pas la journée la plus fun 🤕🤕 Mais ne t'inquiète pas, dans la pratique, tu pourras reprendre du temps sur chaque notion : tu n'auras pas à maîtriser toutes ces techniques en une fois. Prend ton temps pour digérer tout cela et n'hésite pas à te challenger régulièrement sur l'un de ces points pour que les outils statistiques deviennent tes meilleurs amis 🥰

Allez comme on est sympas, on te donne un résumé des [Principes de base de l'analyse statistique](https://edutechwiki.unige.ch/fr/Principes_de_base_d%27analyse_statistique).

## 5. Pour aller plus loin
- La journée de data science prévue lors de la quatrième semaine te permettra d'approfondir les méthodes d'apprentissage automatique, et certains autres concepts vus aujourd'hui. 
- Dans [ce cours](https://certis.enpc.fr/~dalalyan/Download/Poly2.pdf), tu peux revoir tous les concepts importants à connaître en statistiques. 
- Tu peux t'entraîner en faisant des Katas, tu as même un répertoire intitulé [Data and Statistics in Python](https://www.codewars.com/collections/data-and-statistics-in-python).



