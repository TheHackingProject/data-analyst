# Comprendre qui fait quoi : dev ou data ?

## 1. Introduction
Pendant 3 jours, on a laissé le suspense en mode "ba ouais Data Analyst, c'est évident comme job, tout le monde connaît". Mais en fait non, si on n'a pas tranché la question directement, c'est qu'on n'a pas la réponse 😐😐

Maintenant que tu fais partie de ce monde (tu maîtrises déjà Python et SQL), on peut te dire la vérité : personne n'est d'accord sur la définition du métier de **Data Analyst**. 

En gros, c'est un métier récent qui prend différentes facettes (mais vraiment beaucoup de facettes différentes, crois-moi) selon l'entreprise concernée. C'est pourquoi, pendant cette formation Data, on va te présenter le maximum de concepts et d'outils pour que tu puisses ensuite travailler la data dans des environnements très divers. Et que tu deviennes un super couteau-suisse comme on dit 🔪🔎🔦🔬🔨 

Enfin, malgré tout ce flou, on va essayer dans cette ressource de t'expliquer qui fait quoi, et quelles sont les frontières entre développement et data. 

## 2. Historique et contexte
La data et tous les métiers qu'elle englobe ont fait leur apparition dans le vocabulaire courant il n'y a qu'une dizaine d'années. Pourtant, ces métiers ne datent pas d'hier. Remontons un peu l'histoire pour mieux comprendre cela 📜

En 1962, dans *The future of Data Analysis*, John W. Tukey, pourtant un statisticien de renom — on lui doit notamment le terme de « bit » ou encore les diagrammes « boîte à moustache » —, dit préférer le terme de « data analysis » à celui de statistique. Pour lui cette façon de tirer d’un grand nombre de données des tendances relevait plus d’une science empirique que des mathématiques pures, d’où cette différenciation qu’il va être le premier à suggérer.

![texte](https://slideplayer.com/slide/14842537/90/images/3/In+Tukey%E2%80%99s+%281962%29+work+done+for+the+Army+Research+Office+titled%2C+The+Future+of+Data+Analysis%2C+John+Tukey+foreshadowed+the+emergence+of+Data+Science..jpg)

Ensuite, en 1970, comme vu hier, Edgar F. Codd inventait les premières bases de données relationnelles.
A la fin des années 1970 et dans les années 1980, l’informatisation des entreprises se concentrait sous l’angle de la production : saisies et calculs pour la comptabilité, la paie, les stocks, les factures… Des systèmes non conçus pour lancer des requêtes d’analyse.

C’est en 1989 qu’Howard Dresner (futur analyste de la société Gartner) reprend le terme de **Business intelligence** inventé par Luhn et en définit le cadre moderne : des concepts et méthodes pour améliorer la prise de décision grâce à des systèmes d’analyse de données factuelles. Dotée d’une structure et d’un vocabulaire commun, et portée par l’avènement des ordinateurs, l’informatique décisionnelle se normalise enfin.

A l’orée du XXIe siècle, la business intelligence est devenue rigoureuse et a conquis sa place dans le process de prise de décision. C'est son entrée dans l’ère du tout digital qui va la faire basculer dans une autre dimension. Depuis une vingtaine d'années et les débuts du Big Data, de nombreux acteurs de la technologie s'attachent à rajeunir la BI en la rebaptisant Data Discovery (Qliktech), Data Exploration (SAS), Analytics (Tableau, IBM, Oracle), Data Stories (Jolicharts), etc. Les terminologies et les acteurs sont nombreux. Ce qu'il faut retenir c'est qu'**on parle désormais de data pour désigner un ensemble très vaste de technologies qui permettent de traiter les données à très grande échelle**. 

## 3. La ressource
Voyons maintenant les différentes tâches existantes pour faire fonctionner les bases de données, le sujet qui nous intéresse en ce moment. Plutôt que de métiers, on parlera de tâches car comme on le disait dans l'introduction, les frontières entre les différents métiers de la data sont assez floues. Même si, pour que tu comprennes, on te précisera qui, de manière générale, est en charge de réaliser la tâche.

### 3.1. Créer et administrer la base de données
Avant de stocker ses données dans une base, il faut concevoir cette base (voir quel modèle utiliser, se projeter en intégrant tous les éléments), la créer (choisir le logiciel le plus adapté et rendre fonctionnelle la base) et l'administrer (décider des droits d'accès). 

Il s'agit avant tout d'un travail de développeur informatique. C'est pourquoi nous n'avons pas étudié ces aspects-là lors de la journée d'hier. 

> Etre développeur base de données (ou *Data Engineer*) c'est être un spécialiste informatique qui conçoit et déploie une ou plusieurs bases de données. Cette personne est  garante de la cohérence et de l'accessibilité permanente des informations. Elle gère les projets de développement liés au système d'information de l'entreprise qui requièrent le déploiement des bases de données. Elle doit surveiller les performances de la base de données afin de vérifier si la base gère correctement les paramètres. Dans les entreprises plus traditionnelles (industries manufacturières, grands groupes), tu entendras parler "d'Administrateur Base de Données" ou "DB Administrator".

Depuis l'arrivée du Big Data, ces profils sont extrêmement recherchés car certains ont les compétences pour concevoir des bases de données NoSQL. Tu vas voir dans l'autre ressource ce que c'est.

### 3.2. Requêter et faire évoluer la base de données
Une fois que la base de données est créée, un autre profil intervient : l'analyste.

> Le métier de *Data Analyst* consiste à traiter les différentes données issues des clients, des produits ou des performances de l’entreprise afin de dégager des indicateurs utiles aux décideurs. 

Tu vois, la définition est assez vague. C'est pourquoi tu devras savoir faire plein de choses, maîtriser plein d'outils et surtout, être très adaptable.

## 4. Points importants à retenir
L'analyse des données est devenue très complexe depuis une dizaine d'années. C'est pourquoi de nouveaux métiers sont apparus, avec des frontières encore en évolution. 

En théorie : 
Pour créer des bases de données, il faut être dev informatique. 
Pour analyser des bases de données, il faut avoir un esprit analytique, orienté business. 

En pratique : 
Ce sont parfois les mêmes personnes qui réalisent ces deux tâches. En tout cas, ces deux types de profils travaillent régulièrement ensemble et parlent, en partie, les mêmes langages. C'est pourquoi il est important que chacun des deux ait une bonne vision de ce que fait l'autre. D'où l'intérêt de la journée d'aujourd'hui pour vous moussaillons qui avez plutôt opté pour la partie analytique vs le dev pur : vous allez plongé dans l'univers du développement de bases de données 🙈🙈

## 5. Pour aller plus loin
Les 2 autres ressources de la journée vont te permettre d'en savoir plus sur les tâches quotidiennes des *Data Engineers*.

Et pour comprendre mieux tout ce qu'on a dit dans cette ressource, je t'invite, plusieurs fois par semaine, à faire de la veille sur les offres d'emploi autour de la data. En plus des fameux Linkedin, Indeed, Apec, tu peux consulter [Welcome to the jungle](https://www.welcometothejungle.com/fr) : la plupart des entreprises de la Tech postent leurs annonces sur ce site. Tu peux également aller faire un tour sur les plateformes de free-lance comme [Malt](https://www.malt.fr/) et voir les expériences des experts de la data. Ces recherches t'aideront à voir tant la diversité de missions que les constantes qu'on retrouve dans les métiers de la data.
