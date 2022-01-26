# Data et BI : de quoi parle-t-on au juste ?

## 1. Introduction
Pendant 2 jours, on a laissé le suspense en mode "ba ouais Data Analyst, c'est évident comme job, tout le monde connaît". Mais en fait non, si on n'a pas tranché la question directement sur ce que l'intitulé de poste signifie, c'est qu'on n'a pas la réponse 😐😐

Maintenant que tu fais partie de ce monde, on peut te dire la vérité : personne n'est d'accord sur la définition du métier de **Data Analyst**. 

En gros, la Data est univers récent qui est en train de se construire. Il y a encore beaucoup de flou et surtout beaucoup de personnes qui ne savent pas vraiment de quoi elles parlent quand elles doivent s'aventurer dans l'univers data (recruteurs, chefs d'entreprise, chefs de projet etc.).

Malgré ce flou général, on va éclaircir tout cela aujourd'hui en te précisant tous les termes importants.

## 2. Historique et contexte
La data et tous les métiers qu'elle englobe ont fait leur apparition dans le vocabulaire courant il n'y a qu'une dizaine d'années. Pourtant, ces métiers ne datent pas d'hier. Remontons un peu l'histoire pour mieux comprendre cela 📜

En 1962, dans *The future of Data Analysis*, John W. Tukey, pourtant un statisticien de renom — on lui doit notamment le terme de « bit » ou encore les diagrammes « boîte à moustache » —, dit préférer le terme de « data analysis » à celui de statistique. Pour lui cette **façon de tirer d’un grand nombre de données des tendances** relève plus d’une science empirique que des mathématiques pures, d’où cette différenciation qu’il est le premier à suggérer.

![texte](https://slideplayer.com/slide/14842537/90/images/3/In+Tukey%E2%80%99s+%281962%29+work+done+for+the+Army+Research+Office+titled%2C+The+Future+of+Data+Analysis%2C+John+Tukey+foreshadowed+the+emergence+of+Data+Science..jpg)

Quelques années plus tard, en 1970, comme vu hier, Edgar F. Codd inventait les premières bases de données relationnelles.
A la fin des années 1970 et dans les années 1980, l’informatisation des entreprises se concentrait sous **l’angle de la production** : saisies et calculs pour la comptabilité, la paie, les stocks, les factures… Des systèmes non conçus pour lancer des requêtes d’analyse.

C’est en 1989 qu’Howard Dresner (futur analyste de la société Gartner) reprend le terme de **Business intelligence** inventé par Luhn et en définit le cadre moderne : des concepts et méthodes pour améliorer la prise de décision grâce à des systèmes d’analyse de données factuelles. Dotée d’une structure et d’un vocabulaire commun, et portée par l’avènement des ordinateurs, l’informatique décisionnelle se normalise enfin.

A l’orée du XXIe siècle, la business intelligence est devenue rigoureuse et a conquis sa place dans le process de prise de décision. C'est son entrée dans l’ère du tout digital qui va la faire basculer dans une autre dimension. Depuis une vingtaine d'années et les débuts du Big Data, de nombreux acteurs de la technologie s'attachent à rajeunir la BI en la rebaptisant Data Discovery (Qliktech), Data Exploration (SAS), Analytics (Tableau, IBM, Oracle), Data Stories (Jolicharts), etc. Les terminologies et les acteurs sont nombreux. Ce qu'il faut retenir c'est qu'**on parle désormais de data pour désigner un ensemble très vaste de technologies qui permettent de traiter les données à très grande échelle**. 

## 3. La ressource

### 3.1. C'est quoi une "data" ?

Une data c’est tout simplement une donnée stockée numériquement. Plus précisément, c'est une information dématérialisée capable de circuler à travers un réseau de télécommunication ou informatique. Ce peut être une donnée que vous avez déposée inconsciemment en navigant sur Internet (ex : les cookies, les logs). Ce peut être une donnée que vous avez créée consciemment (ex : rédaction d'un mail). Ce peut être une donnée qui a été produite par une autre machine (ex : systèmes de mesure, IoT).

On comprend alors qu'il y a différents types de données. Lorsqu'une entreprise parle de "nos données", cela mériterait d'être précisé car on ne sait pas s'il s'agit des données personnelles des utilisateurs, des données commerciales et financières, des données liées aux opérations de l'entreprise, des données marketing etc.

Finalement, le mot "data" est très galvaudé. Il n'a plus vraiment de sens lorsqu'il n'est pas précisé par les personnes qui l'utilisent.


### 3.2. Différencier informatique et informatique décisionnelle

L’informatique décisionnelle est une branche de l’informatique de plus en plus adoptée par les entreprises. Connue également sous l’appellation *Business Intelligence* (et souvent BI) en anglais, elle désigne l’ensemble des méthodes et outils informatiques utilisés généralement pour piloter une organisation. Le meilleur exemple de solution d’informatique décisionnelle est le tableau de bord. L’informatique décisionnelle utilise les données brutes de l’organisation comme matière première. A l’aide d’outils décisionnels (logiciels ou applications), on se connecte à des sources de données qui peuvent être très diverses : Excel, base de données SQL, ERP, etc…

### 3.3. Différencier modèle transactionnel et modèle multidimensionnel

#### 3.1.3. Différencier Data Analysis et Data Science

#### 3.1.4. C'est quoi le Big Data ?



### 3.2. Une équipe data, ça sert à quoi ?

Créer et administrer la base de données
Avant de stocker ses données dans une base, il faut concevoir cette base (voir quel modèle utiliser, se projeter en intégrant tous les éléments), la créer (choisir le logiciel le plus adapté et rendre fonctionnelle la base) et l'administrer (décider des droits d'accès). 

Il s'agit plutôt d'un travail de développeur informatique.

> Etre développeur base de données (ou *Data Engineer*) c'est être un spécialiste informatique qui conçoit et déploie une ou plusieurs bases de données. Cette personne est  garante de la cohérence et de l'accessibilité permanente des informations. Elle gère les projets de développement liés au système d'information de l'entreprise qui requièrent le déploiement des bases de données. Elle doit surveiller les performances de la base de données afin de vérifier si la base gère correctement les paramètres. 

Dans les entreprises plus traditionnelles (industries manufacturières, grands groupes), tu entendras parler de "Administrateur Base de Données" ou "DB Administrator". 
Depuis l'arrivée du Big Data, ces profils sont extrêmement recherchés car certains ont les compétences pour concevoir des bases de données NoSQL. Tu vas voir dans l'autre ressource ce que c'est.

### 3.2. Requêter et faire évoluer la base de données
Une fois que la base de données est créée, un autre profil intervient : l'analyste.

> Le métier de *Data Analyst* consiste à traiter les différentes données issues des clients, des produits ou des performances de l’entreprise afin de dégager des indicateurs utiles aux décideurs. 

Tu vois, la définition est assez vague. C'est pourquoi tu devras savoir faire plein de choses, maîtriser plein d'outils et surtout, être très adaptable.

## 4. Points importants à retenir
L'analyse des données est devenue très complexe depuis une dizaine d'années. C'est pourquoi de nouveaux métiers sont apparus, avec des frontières encore en évolution. 

En théorie : 
Pour créer des bases de données, il faut être dev informatique. 
Pour analyser des bases de données, il faut avoir un esprit analytique, orienté business et connaître les bases des statistiques. 

En pratique : 
Ce sont parfois les mêmes personnes qui réalisent ces deux tâches. En tout cas, ces deux types de profils travaillent régulièrement ensemble et parlent, en partie, les mêmes langages. C'est pourquoi il est important que chacun des deux ait une bonne vision de ce que fait l'autre. D'où l'intérêt de la journée d'aujourd'hui pour vous moussaillons qui avez plutôt opté pour la partie analytique vs le dev pur : vous allez plongé dans l'univers du développement de bases de données 🙈🙈

## 5. Pour aller plus loin
Les 2 autres ressources de la journée vont te permettre d'en savoir plus sur les tâches quotidiennes des *Data Engineers*.

Et pour comprendre mieux tout ce qu'on a dit dans cette ressource, je t'invite, plusieurs fois par semaine, à faire de la veille sur les offres d'emploi autour de la data. En plus des fameux Linkedin, Indeed, Apec, tu peux consulter [Welcome to the jungle](https://www.welcometothejungle.com/fr) : la plupart des entreprises de la Tech postent leurs annonces sur ce site. Tu peux également aller faire un tour sur les plateformes de free-lance comme [Malt](https://www.malt.fr/) et voir les expériences des experts de la data. Ces recherches t'aideront à voir tant la diversité de missions que les constantes qu'on retrouve dans les métiers de la data.


