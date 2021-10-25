# Réaliser des tableaux de bord

## 1. Introduction
Une fois que les KPI sont identifiés, il est important de suivre leur évolution via un tableau de bord 🎯

## 2. Historique et contexte

A partir de la seconde moitié du 19ème siècle, les dirigeants élaborent un système d'information de gestion présentant les données, pour l'essentiel sous forme narrative, au travers d'un « rapport hebdomadaire » ou « journal de marche ». La révolution industrielle entraine la croissance de la taille des entreprises et leur complexité. Le besoin des gestionnaires d'informations statistiques descriptives de la réalité opérationnelle se fait de plus en plus important. 

En fait, **les  tableaux  de  bord apparaissent  lorsque  les  dirigeants  d’entreprise  perdent  le  contact  direct  avec  leurs  affaires**.  La  taille  et  la  dispersion  géographique  éloignent  mécaniquement  les  dirigeants  des  commerçants,  des  producteurs,  du  personnel,  etc.  S’ils  veulent  rester  informés,  ils  doivent  inventer  un  dispositif leur permettant, si ce n’est de voir l’état de leurs affaires, de se le représenter.

En France en 1977, le cartographe Jacques Bertin nous fournit un exemple très détaillé de tableau de bord dans son livre *La graphique et le traitement graphique de l'information*. Tu peux regarder à quoi cela ressemblait [ici](https://perceptible.fr/bertin/).

Mais c'est surtout les chercheurs **Kaplan et Norton qui ont rendu célèbre le tableau de bord dans un article de 1992**, publié dans la Harvard Business Review : « *The Balanced Scorecard : Measures That Drive Performance* ». Le *Balanced Scorecard*  est un tableau de bord stratégique dont l'objectif est de prendre en compte l'ensemble des dimensions concourant à la performance au-delà des simple mesures financières. Les 4 vues du modèle sont : Client, Finance, Processus internes, Apprentissage et développement.

La publication du texte en 1992 a entrainé l'adoption du tableau de bord par plusieurs organisations publiques ou privées pour l'implémentation de leur stratégie.
Comme vu dans la ressource précédente, la redécouverte de tableau de bord et des indicateurs non financiers a été un des phénomènes frappants des années 90 🔥


## 3. La ressource

### 3.1. Concevoir un dashboard

Il y a plusieurs étapes à respecter pour bien concevoir un tableau de bord, et tout ceci avant de se lancer dans la création du tableau :
- **Définir l’objectif du tableau de bord avec votre client**. Un tableau de bord peut servir au pilotage, au reporting ou bien à la communication : il est important de bien préciser dans quel cas vous vous situez.
- **Définir les bons indicateurs avec votre client**. Cf. ressource précédente sur les KPI 🤗
- **Recueillir tous les besoins de votre client**. Si tu cherches à savoir comment cette étape se passe dans la pratique, je t'invite à suivre toutes les vidéos d'échange entre Luc et Thomas dans [ce cours OpenClassrooms](https://openclassrooms.com/fr/courses/4525361-realisez-un-dashboard-avec-tableau/5728791-participez-a-une-reunion-d-analyse-de-besoins). Tu peux aller jusqu'à réaliser le *Quiz : Réalisez les étapes de création d'un dashboard* pour voir si tu as bien assimilé l'essentiel.

### 3.2. Créer son dashboard

C’est l’étape la plus « technique ». 

Une fois les KPI validés, il va falloir **lister les sources de données** dont vous aurez besoin pour les développer. Cette étape est très importante, car, pour chaque source que vous connectez au dashboard, vous risquez de voir augmenter le coût et la complexité de votre infrastructure. C’est pourquoi il vaut toujours mieux se connecter seulement aux sources pertinentes pour les KPI attendus.

De même, vous allez devoir **prévoir l'infrastructure**. En fonction de la complexité des données et de leur volume, il vous faudra estimer des ressources de stockage et de calcul. Avoir la bonne infrastructure en backend améliore considérablement la performance de vos tableaux de bord, d’autant qu’ils seront fréquemment mis à jour. Que la mise à jour se fasse tous les jours ou en temps réel, il faut prévoir l’infrastructure en conséquence pour éviter tout problème de performance à long-terme.

Enfin et suite à ces deux paramètres, vous pourrez **choisir la solution de visualisation adaptée**. Pour répondre aux besoins croissants du marché, de nombreux outils analytiques de visualisation de données existent aujourd’hui. Mais alors que certains se révèlent faciles à utiliser et intuitifs, d’autres sont plus complexes au premier abord et conviennent mieux à des experts de la data ayant des connaissances en développement. Il vous faut donc choisir celui qui sera adapté à vos besoins, de votre secteur d’activité et aux utilisateurs finaux au sein de votre entreprise. La question du budget est aussi à se poser car si de nombreuses offres existent sur le marché, toutes ne sont pas accessibles pour toutes les organisations. 

___

🙃🙃 Et si je choisis l'outil le plus populaire ? 🙃🙃

C'est déconseillé de répondre comme cela car la solution peut ne pas être adaptée aux contraintes de ton entreprise. 

Mais pour ta culture générale, voici les 3 outils les plus connus sur le marché : Tableau, PowerBI et Qlik. Et si tu veux en connaître encore d'autres et constater l'immensité du marché, tu peux consulter ce [top 11](https://superdatacamp.com/data-science/meilleurs-outils-de-visualisation/) des meilleurs outils de data viz en 2021.

___

### 3.3. Zoom sur le logiciel Tableau 

Et dernièrement, la connaissance de Tableau semble être demandée dans la majorité des offres d'emploi de Data Analysts en France. Donc nous te conseillons de t'approprier ce logiciel. Pour cela, tu peux télécharger une version gratuite du logiciel et suivre le chapitre 2 du [cours OpenClassrooms](https://openclassrooms.com/fr/courses/4525361-realisez-un-dashboard-avec-tableau/5741176-selectionnez-votre-outil-de-dashboard).


## 4. Points importants à retenir
Le "dashboard" ou tableau de bord a pour fonction de permettre la visualisation, le suivi et l'exploitation facile de données pertinentes sous forme de chiffres, ratios et de graphiques. Ces indicateurs (appelés aussi KPI) sont reliés à des objectifs dans le but de prendre des décisions.

Mais il n'est pas question de produire des outils pour rien. Si vous devez construire un tableau de borde, faites en sorte qu'il soit réellement utilisé par ses destinataires, que ce soit vous ou vos collaborateurs ! 

## 5. Pour aller plus loin
- Les livres blancs produits par Tableau à consulter [ici](https://www.tableau.com/fr-fr/learn/whitepapers)
