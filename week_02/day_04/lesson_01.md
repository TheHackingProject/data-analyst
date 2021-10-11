# La visualisation des données ou *dataviz*

## 1. Introduction

Notre cerveau est incapable de traiter les gros volumes de données générées ou traitées dans l’entreprise 🤯 Ainsi, la visualisation des données a été créée pour rapidement explorer et analyser les données. Elle est destinée à tous ceux dans l'entreprise qui souhaitent utiliser et tirer des enseignements à partir des données indépendamment de leur niveau de compétence analytique : utilisateurs métiers, décideurs, analystes, statisticiens et data scientists. 

Le volume de données continuera à croître alors que le temps et les ressources nécessaires pour les interpréter diminueront. La visualisation des données sera alors l’un des rares outils capable de nous aider à emporter ce défi.

## 2. Historique et contexte

Tout pourrait porter à croire que la Data visualisation est récente mais il n’en est rien, bien au contraire. Prenons l’exemple d’un très vaste volume d’informations que la population a dû assimiler : la Bible. Pour faciliter l’assimilation des informations très éclatées qui s’y trouvent, un support visuel assez singulier a été produit au Moyen-Age. Il s’agit de [l’Arbre de Jessé](https://fr.wikipedia.org/wiki/Arbre_de_Jess%C3%A9) qui est une représentation de la généalogie présumée de Jésus de Nazareth et qui synthétise l’ensemble des informations relatives à ses ascendants - informations très clairsemées au fil de l’ouvrage. On estime que cette aide visuelle constitue le premier exemple significatif de Data visualisation.

**Le concept d’utilisation d’images pour comprendre des données remonte donc à des siècles en arrière mais il s’est affiné au fil du temps** et s’est sophistiqué. Avant le 17ème siècle, la visualisation des données existait principalement dans le domaine de la cartographie, affichant surtout des repères terrestres, des villes, des routes et des ressources. 

Le 18ème siècle a vu l’apparition de la cartographie thématique. Des tentatives de cartographie thématique des données géologiques, économiques et médicales ont été effectuées vers la fin du siècle. L’un des exemples les plus cités de graphiques statistiques a eu lieu lorsque Charles Minard a cartographié [l’invasion de la Russie par Napoléon](https://fr.wikipedia.org/wiki/Charles_Joseph_Minard#/media/Fichier:Minard.png). La carte représente la taille de l’armée ainsi que la trajectoire du retrait de Napoléon de Moscou.

**Mais c’est surtout l’informatique et les nouvelles technologies qui ont vraiment révolutionné la Data visualisation**. Ainsi, les ordinateurs ont permis de traiter de grandes quantités de données à des vitesses optimales. Aujourd’hui, la datavisualisation est devenue un mélange scientifique et artistique, appuyé par les nouvelles technologies qui ont permis de rendre cette méthode interactive et beaucoup plus efficiente 👌

## 3. La ressource

### 3.1. Dataviz avec Python

En utilisant Python, il est possible de manipuler, de transformer et de créer des visualisations de données. De nombreux Data Analysts et Scientists se tournent vers cette solution.

Au cours des dernières années, de nombreuses nouvelles librairies de visualisation de données ont vu le jour sur Python. **Matplotlib est devenu la principale librairie de visualisation de données**, bien qu'elle soit assez complexe d'utilisation. On peut citer d'autres librairies populaires : 
- **Seaborn** exploite la puissance de matplotlib pour créer de belles visualisations en quelques lignes de code. La principale différence réside dans les styles et les palettes de couleurs offerts par Seaborn, qui sont conçus pour être plus esthétiques et modernes.
- **Plotly** permet la création de graphiques interactifs, mais propose aussi des visualisations difficiles à trouver dans la plupart des bibliothèques, comme les courbes de niveau, les dendrogrammes, les graphiques en 3D…

Pour maîtriser ses librairies, il s'agit avant tout de pratiquer 🤙

Voici quelques ressources qui peuvent t'aider à commencer dans la visualisation avec Python : 
- [un article](https://moncoachdata.com/blog/visualisation-de-donnees-avec-python/) qui compare les différentes librairies Python
- [une vidéo](https://www.youtube.com/watch?v=JSnb7HU8Ahs) qui te montre comment utiliser Matplotlib.


### 3.2. Les outils de dataviz

Les outils BI sont à la data, ce que le no-code est au développement web. Ce sont des softwares déjà développés qui permettent de glisser et déposer, par un système de drag and drop, un dataset pour visualiser la donnée directement. On dit de ces outils qu’ils sont plus accessibles aux personnes qui n’ont pas ou peu été initiées à la data. Ils sont souvent destinés aux entreprises qui cherchent des résultats rapides et simples à manier. 

Il existe de nombreux outils permettant de créer des visualisations de données. Mais quels sont les outils BI les plus utilisés ?

1. **Tableau est l’outil BI de référence sur le marché**. Grâce à sa simplicité d’utilisation et à sa capacité à produire des visualisations interactives, ce logiciel compte une très large base de clients. Il se démarque grâce à de nombreuses fonctionnalités et tableaux de bords préconçus qui permettent de mettre en forme très facilement la donnée issue de logiciels CRM comme Salesforces. 

L'éditeur propose deux applications de bureau gratuites pour Windows et MacOS : [Tableau Public](https://www.tableau.com/fr-fr/community/public) et [Tableau Reader](https://www.tableau.com/fr-fr/products/reader). Le premier permet à la fois ouvrir et créer des analyses qui sont stockées sur un profil public. Le second offre d'ouvrir et d'interagir avec les fichiers de visualisation de données créés dans Tableau Desktop, l'application payante.

2. **Power BI, désormais le principal concurrent de Tableau, est une suite d’outils analytiques, développée par Microsoft**. Power BI est disponible gratuitement en version limitée et permet de suivre toute votre démarche de data analyse, de la préparation de vos données aux bilans d’analyse, en passant par la réalisation de tableaux de bord interactifs. PowerBI propose, comme Tableau, [un service de gallerie](https://community.powerbi.com/t5/Data-Stories-Gallery/bd-p/DataStoriesGallery) sur lequel on peut trouver de l'inspiration.

3. **Qlikview était le concurrent principal de Tableau avant de connaître une perte de vitesse**. Il témoigne d’un grand nombre de fonctionnalités (data visualisation, business intelligence, analyse et reporting) qui rendent sa configuration très personnalisable. Cependant, la courbe d’apprentissage qui y est liée est non négligeable : pour maîtriser Qlikview, un certain temps est nécessaire !

4. Google Data Studio est un outil de la suite Google Analytics qui transforme vos données provenant de vos comptes Google (Ads, Analytics, Drive, Sheets…) et autres sources (Facebook, YouTube, Twitter, Search console, MySQL...) en rapports à la fois personnalisables et esthétiques, simples à lire et à partager. Même si cet outil est encore récent et qu’il ne permet pas de faire des représentations aussi poussées que Tableau, c’est une solution totalement gratuite, à la fois personnalisable et collaborative, mettant à jour les données en temps réel. 

## 4. Points importants à retenir
La visualisation de données est très utilisée dans tous les secteurs d’activité. Par conséquent, **maîtriser un outil de dataviz est une compétence précieuse et convoitée**. On peut obtenir des résultats similaires en travaillant avec des librairies de dataviz et des outils BI, mais ces deux solutions reposent sur des techniques différentes.

## 5. Pour aller plus loin
Faire de la veille sur les outils de dataviz et pratiquer sans relâche !
