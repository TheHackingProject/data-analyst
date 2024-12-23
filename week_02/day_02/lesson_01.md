# Le nettoyage des données

## 1. Introduction
C'est l’étape la plus importante avant d’analyser des données. Attention, cette étape peut être très fastidieuse, elle constitue souvent un vraie casse-tête pour les Data Analysts 🤬

📌 *Utilité pour le projet* : 5/5<br/>
📊 *Utilité pour être Data Analyst* : 5/5<br/>
💡 *Pourquoi cette ressource ?* : Ici, on théorise le nettoyage des données. Tu vas surtout apprendre en pratiquant donc go sur le projet dès que possible !

## 2. Historique et contexte
Les volumes de données dont nous disposons ne cessent d’augmenter, de même que les risques d’erreur. Ces données qui présentent des problèmes d’erreur et d’incohérence sont généralement appelées « données sales », et leur impact global n’est pas négligeable. On estime que 3 % seulement des données satisfont aux normes de qualité de base et que les données sales coûtent plus de 3 milliards $USD par an aux entreprises américaines.
Par conséquent, il faut compter sur le nettoyage des données (aussi appelé *data cleaning*) pour pouvoir réaliser des analyses cohérentes. 

## 3. La ressource

### 3.1. Données manquantes
La plus importante tâche du Data Cleaning consiste à traiter les données manquantes. Pour bien comprendre comment gérer les données manquantes, je t'invite à lire cet [article de blog](https://moncoachdata.com/blog/nettoyage-de-donnees-python/).

### 3.2. Valeurs aberrantes
Une valeur aberrante ou *outlier* correspond à une valeur éloignée de la distribution de la variable. Cela peut être dû à une erreur de typographie ou à une erreur de mesure mais cela peut aussi être une valeur extrême. On parle couramment de valeur extrême, pour désigner une valeur non erronée qui s’éloigne néanmoins fortement du reste des valeurs de la variable. 

Une façon assez simple de détecter ces valeurs est de réaliser un box plot (ou boîte à moustaches) pour chacune des variables. Un box plot est un graphique sous forme de rectangle où sont décrites les statistiques de la variables (les quartiles : Q1, médiane, Q3). Les bornes du graphique délimitent les valeurs selon la distribution de la variable. Au-delà de ces extrémités, ces valeurs sont considérées comme des valeurs aberrantes.

Dans le cadre d’un projet de Machine Learning, on fera souvent le choix de supprimer une valeur aberrante. En effet, pour obtenir une meilleure qualité de prédiction il est nécessaire de traiter ces données car un modèle pourra être très sensible aux données extrêmes, ce qui va biaiser les prédictions.

### 3.3. Mauvais format
La valeur de la donnée peut se retrouver avec un mauvais **formatage**. Un exemple simple est la gestion des `float`. En fonction de la source de données, les décimales peuvent être séparées par des virgule `,` ou bien par des points `.`. Lors du premier cas, l'extraction en CSV peut poser problème car le CSV délimite ses données par une virgule.
2 solutions s'offrent alors à toi :
- gérer le problème à la source (10% du temps) : contacter le client qui provisionne les données (Database)
- gérer le problème lors du traitement (90% du temps): trouver des solutions ingénieuses afin de reformater les données.

Un autre exemple de mauvais formatage est l'utilisation d'un Y/N ou d'un O/N (varchar) à la place d'un True/False (Booléen). Dans ce cas-ci, une simple recherche dans ta mémoire (ou sur une documentation appropriée) te donnera la solution.

Un dernier exemple qui t'arrivera **forcément** et qui peut dans certains cas être difficile à relever est l'utilisation d'espace dans les données textuelles. Quoi de plus rageant que de ne pas réussir à trouver le texte `"CoeurSurFéfé"` lorsque la donnée originale est en réalité `" CoeurSurFéfé "`. Plusieurs options s'offrent encore une fois à toi :
- "rogner" les données textuelles (trim in English)
- utiliser les [RegEx](https://www.w3schools.com/python/python_regex.asp).


## 4. Points importants à retenir
- Le nettoyage des données est une étape cruciale pour la réussite de tout projet data. Il y a 3 étapes dans le nettoyage des données : la gestion des données manquantes, la gestion des valeurs aberrantes, et la gestion du mauvais format.

- Dans la plupart des cas, on est obligés de faire des allers-retours entre la phase de nettoyage et la phase de description (analyse). En phase d'analyse, on trouve souvent de nouvelles erreurs, et il faut revenir au nettoyage. 

- Chaque nettoyage de données est unique : il n'y a pas de règle à proprement parler. L'objectif est toujours de repérer les sources d'erreurs qui pourraient nuire à l'analyse et de trouver le meilleur moyen pour les corriger.

## 5. Pour aller plus loin
La ressource du jour est courte car il s'agit surtout de notions que tu apprendras en pratiquant. Profites-en pour faire le [chapitre du cours d'OC](https://openclassrooms.com/fr/courses/4525266-decrivez-et-nettoyez-votre-jeu-de-donnees/4928106-reperez-les-differents-types-derreurs) sur le nettoyage des jeux de données. Tu peux aller jusqu'au quiz final.
