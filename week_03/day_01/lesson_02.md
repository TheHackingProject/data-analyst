# Réaliser des tableaux de bord

## 1. Introduction
Une fois que les KPI sont identifiés, il est important de suivre leur évolution via un tableau de bord 🎯

📌 *Utilité pour le projet* : 5/5<br/>
📊 *Utilité pour être Data Analyst* : 5/5<br/>
💡 *Pourquoi cette ressource ?* : Te faire découvrir la méthodologie et les outils pour réaliser des tableaux de bord efficaces.

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

### 3.3. Les outils pour créer des dashboards visuels

Il existe de nombreux outils permettant de créer des visualisations de données. Mais quels sont les outils BI les plus utilisés ? On t'en donne ici 4 mais tu pourras encore en trouver bien d'autres.

1. **Tableau est l’outil BI de référence sur le marché**. Grâce à sa simplicité d’utilisation et à sa capacité à produire des visualisations interactives, ce logiciel compte une très large base de clients. Il se démarque grâce à de nombreuses fonctionnalités et tableaux de bords préconçus qui permettent de mettre en forme très facilement la donnée issue de logiciels CRM comme Salesforce. L'éditeur propose deux applications de bureau gratuites pour Windows et MacOS : [Tableau Public](https://www.tableau.com/fr-fr/community/public) et [Tableau Reader](https://www.tableau.com/fr-fr/products/reader). Le premier permet à la fois ouvrir et créer des analyses qui sont stockées sur un profil public. Le second offre d'ouvrir et d'interagir avec les fichiers de visualisation de données créés dans Tableau Desktop, l'application payante.

2. **Power BI, désormais le principal concurrent de Tableau, est une suite d’outils analytiques, développée par Microsoft**. Power BI est disponible gratuitement en version limitée et permet de suivre toute votre démarche de data analyse, de la préparation de vos données aux bilans d’analyse, en passant par la réalisation de tableaux de bord interactifs. PowerBI propose, comme Tableau, [un service de gallerie](https://community.powerbi.com/t5/Data-Stories-Gallery/bd-p/DataStoriesGallery) sur lequel on peut trouver de l'inspiration.

3. **Qlikview était le concurrent principal de Tableau avant de connaître une perte de vitesse**. Il témoigne d’un grand nombre de fonctionnalités (data visualisation, business intelligence, analyse et reporting) qui rendent sa configuration très personnalisable. Cependant, la courbe d’apprentissage qui y est liée est non négligeable : pour maîtriser Qlikview, un certain temps est nécessaire !

4. Google Data Studio est un outil de la suite Google Analytics qui transforme vos données provenant de vos comptes Google (Ads, Analytics, Drive, Sheets…) et autres sources (Facebook, YouTube, Twitter, Search console, MySQL...) en rapports à la fois personnalisables et esthétiques, simples à lire et à partager. Même si cet outil est encore récent et qu’il ne permet pas de faire des représentations aussi poussées que Tableau, c’est une solution totalement gratuite, à la fois personnalisable et collaborative, mettant à jour les données en temps réel. 

### 3.4. Zoom sur l'outil Tableau

En effet, dernièrement, la connaissance de Tableau semble être demandée dans la majorité des offres d'emploi de Data Analysts en France. Donc nous te conseillons de t'approprier ce logiciel. C'est le l'outil que tu vas devoir utiliser dans ton projet aujourd'hui. 

Pour cela, tu peux télécharger une version gratuite du logiciel [ici](https://www.tableau.com/fr-fr/products/desktop/download).

Si tu veux un tutoriel en français, tu peux suivre le chapitre 2 du [cours OpenClassrooms](https://openclassrooms.com/fr/courses/4525361-realisez-un-dashboard-avec-tableau/5741176-selectionnez-votre-outil-de-dashboard).

Et si tu es ok avec le fait de te former en anglais, je t'invite à suivre les tutoriels créées par l'entreprise Tableau :
- un [tutoriel bac-à-sable](https://help.tableau.com/current/guides/get-started-tutorial/en-us/get-started-tutorial-home.htm), 
- un tutoriel vidéo en deux parties : [partie 1](https://www.tableau.com/learn/webinars/intro-tableau-desktop-part1-superstore#video) et [partie 2](https://www.tableau.com/learn/webinars/intro-tableau-desktop-part2-superstore). 
Ils permettent d'entrer tout de suite dans la pratique. Et en plus, tu travailleras sur le même jeu de données dans ton projet. Tu n'es pas obligé de faire les tutoriels en entier. Dès que tu te sens à l'aise, tu peux les arrêter et poursuivre le projet en toute autonomie.


## 4. Points importants à retenir
Le "dashboard" ou tableau de bord a pour fonction de permettre la visualisation, le suivi et l'exploitation facile de données pertinentes sous forme de chiffres, ratios et de graphiques. Ces indicateurs (appelés aussi KPI) sont reliés à des objectifs dans le but de prendre des décisions.

Mais il n'est pas question de produire des outils pour rien. Si vous devez construire un tableau de bord, faites en sorte qu'il soit réellement utilisé par ses destinataires, que ce soit vous ou vos collaborateurs ! 

## 5. Pour aller plus loin
- Les livres blancs produits par Tableau à consulter [ici](https://www.tableau.com/fr-fr/learn/whitepapers)
