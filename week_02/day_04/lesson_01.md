# La visualisation des données ou *dataviz*

## 1. Introduction

Notre cerveau est incapable de traiter les gros volumes de données générées ou traitées dans l’entreprise 🤯 Ainsi, la visualisation des données a été créée pour rapidement explorer et analyser les données. Elle est destinée à tous ceux dans l'entreprise qui souhaitent utiliser et tirer des enseignements à partir des données indépendamment de leur niveau de compétence analytique : utilisateurs métiers, décideurs, analystes, statisticiens et data scientists. 

Le volume de données continuera à croître alors que le temps et les ressources nécessaires pour les interpréter diminueront. La visualisation des données sera alors l’un des rares outils capable de nous aider à emporter ce défi.


📌 *Utilité pour le projet* : 4/5<br/>
📊 *Utilité pour être Data Analyst* : 5/5<br/>
💡 *Pourquoi cette ressource ?* : T'expliquer l'importance de la visualisation.

## 2. Historique et contexte

Tout pourrait porter à croire que la Data visualisation est récente mais il n’en est rien, bien au contraire. Prenons l’exemple d’un très vaste volume d’informations que la population a dû assimiler : la Bible. Pour faciliter l’assimilation des informations très éclatées qui s’y trouvent, un support visuel assez singulier a été produit au Moyen-Age. Il s’agit de [l’Arbre de Jessé](https://fr.wikipedia.org/wiki/Arbre_de_Jess%C3%A9) qui est une représentation de la généalogie présumée de Jésus de Nazareth et qui synthétise l’ensemble des informations relatives à ses ascendants - informations très clairsemées au fil de l’ouvrage. On estime que cette aide visuelle constitue le premier exemple significatif de Data visualisation.

**Le concept d’utilisation d’images pour comprendre des données remonte donc à des siècles en arrière mais il s’est affiné au fil du temps** et s’est sophistiqué. Avant le 17ème siècle, la visualisation des données existait principalement dans le domaine de la cartographie, affichant surtout des repères terrestres, des villes, des routes et des ressources. 

Le 18ème siècle a vu l’apparition de la cartographie thématique. Des tentatives de cartographie thématique des données géologiques, économiques et médicales ont été effectuées vers la fin du siècle. L’un des exemples les plus cités de graphiques statistiques a eu lieu lorsque Charles Minard a cartographié [l’invasion de la Russie par Napoléon](https://fr.wikipedia.org/wiki/Charles_Joseph_Minard#/media/Fichier:Minard.png). La carte représente la taille de l’armée ainsi que la trajectoire du retrait de Napoléon de Moscou.

**Mais c’est surtout l’informatique et les nouvelles technologies qui ont vraiment révolutionné la Data visualisation**. Ainsi, les ordinateurs ont permis de traiter de grandes quantités de données à des vitesses optimales. Aujourd’hui, la datavisualisation est devenue un mélange scientifique et artistique, appuyé par les nouvelles technologies qui ont permis de rendre cette méthode interactive et beaucoup plus efficiente 👌

## 3. La ressource

### 3.1. Réussir ses graphiques

Contrairement à ce qu'on pourrait penser, réussir un graphique n'est pas chose aisée. Il faut prendre son temps pour savoir ce qu'on cherche à représenter et ensuite trouver la meilleure représentation. 

Consultez [cet article](https://tssperformance.com/les-4-etapes-essentielles-pour-reussir-son-graphique/) qui rappelle toutes les étapes essentielles à la réussite d'un graphique. Cela peut paraître évident mais vous verrez en pratiquant qu'on est souvent tentés de griller des étapes pour se rendre finalement compte que le graphe choisi n'est pas le bon ou par ex que les axes doivent être intervertis. 


### 3.2. Dataviz avec Python

En utilisant Python, il est possible de manipuler, de transformer et de créer des visualisations de données. De nombreux Data Analysts et Scientists se tournent vers cette solution.

Au cours des dernières années, de nombreuses nouvelles librairies de visualisation de données ont vu le jour sur Python. **Matplotlib est devenu la principale librairie de visualisation de données**, bien qu'elle soit assez complexe d'utilisation. On peut citer d'autres librairies populaires : 
- **Seaborn** exploite la puissance de matplotlib pour créer de belles visualisations en quelques lignes de code. La principale différence réside dans les styles et les palettes de couleurs offerts par Seaborn, qui sont conçus pour être plus esthétiques et modernes.
- **Plotly** permet la création de graphiques interactifs, mais propose aussi des visualisations difficiles à trouver dans la plupart des bibliothèques, comme les courbes de niveau, les dendrogrammes, les graphiques en 3D…

Voici quelques ressources qui peuvent t'aider à commencer dans la visualisation avec Python : 
- [un article](https://moncoachdata.com/blog/visualisation-de-donnees-avec-python/) qui compare les différentes librairies Python
- [une vidéo](https://www.youtube.com/watch?v=JSnb7HU8Ahs) qui te montre comment utiliser Matplotlib.

Mais pour maîtriser ses librairies, il s'agit avant tout de pratiquer 🤙

Commence le projet du jour et surtout garde à disposition Google ton meilleur ami. Au début, tu vas tâtonner, tenter des trucs. Et ces tentatives vont t'aider à comprendre le fonctionnement global. Pour garder en mémoire les fonctions que tu maîtrises, pense à te créer une *cheat sheet* (aide-mémoire). Si tu es un peu flemmard, beaucoup sont en libre accès sur Internet. Voici une sélection, à toi de garder celles qui te correspondent : 
- [une](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Python_Matplotlib_Cheat_Sheet.pdf) sur Matplotlib
- [une](https://www.datacamp.com/community/blog/seaborn-cheat-sheet-python) sur Seaborn
- [une](https://phychim.ac-versailles.fr/IMG/pdf/tuto_python_matplotlib.pdf) en français sur Matlplotlib.


### 3.3. Les outils de dataviz

Les outils BI sont à la data ce que le no-code est au développement web. Ce sont des softwares déjà développés qui permettent de glisser et déposer, par un système de drag and drop, un dataset pour visualiser la donnée directement. On dit de ces outils qu’ils sont plus accessibles aux personnes qui n’ont pas ou peu été initiées à la data. Ils sont souvent destinés aux entreprises qui cherchent des résultats rapides et simples à manier. 

On peut obtenir des résultats similaires en travaillant avec des librairies de dataviz et des outils BI, mais ces deux solutions reposent sur des techniques différentes. Nous verrons quels sont ces outils et comment les utiliser lors de la semaine prochaine. Cette semaine, on se concentre sur les tâches qu'on peut réaliser avec Python.

## 4. Points importants à retenir
La visualisation de données est très utilisée dans tous les secteurs d’activité. Rappelle-toi que **le cerveau humain préfère dans la plupart des cas regarder un graphe que du texte**. Quand tu travailles sur tes jeux de données, fais plaisir à ton cerveau en lui offrant régulièrement la possibilité de voir une représentation graphique. Et surtout, quand tu présentes tes résultats à d'autres personnes, pense toujours à les agrémenter de nombreux graphes 📊📈📉

## 5. Pour aller plus loin
Pratiquer sans relâche !
