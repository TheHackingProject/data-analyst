# ETL et Data Warehouse
Quelques mots anglais qui paraissent barbares mais qui constituent la base de l'informatique décisionnel.

## 1. Introduction
Le Data warehouse, ou entrepôt de données, est une base de données dédiée au stockage des données pour l'analyse décisionnelle. Il est alimenté en données depuis les bases de production grâce aux outils d'ETL (Extract Transform Load). Cette ressource, à la frontière de la culture générale, va te permettre de mieux comprendre les enjeux actuels de la data 👻👻.

## 2.Historique et contexte
Les premiers logiciels **Extract-Transform-Load** ont été développés au milieu des années 1970. A cette époque, les entreprises commençaient à utiliser plusieurs sources de données et à gérer différentes bases pour stocker différentes sortes de données business. Très tôt, le besoin s’est fait sentir d’agréger ces données. Au tournant des années 1980 – 1990, un type de plateforme s’est imposé comme solution de référence pour recevoir toutes ces données transformées et faire office de référentiel data : le Data Warehouse.

Un **Data Warehouse** (ou entrepôt de données) est une base de données relationnelle pensée et conçue pour les requêtes et les analyses de données, la prise de décision et les activités de type Business Intelligence, davantage que pour le traitement de transactions. Les Data Warehouses sont utilisées depuis près de 30 ans. Depuis peu toutefois, les Data Lakes gagnent en popularité à tel point que certains pensent qu’ils vont remplacer les Warehouses. 

## 3. La ressource

### 3.1. Les 3 étapes de l'ETL

Comme son nom l'indique, l'ETL se décompose en trois phases : l'extraction, la transformation et le chargement.

- Extract

Pour vous représenter le fonctionnement d'un ETL, prenez l'exemple d'une entreprise vendant des biens à la fois en ligne et dans ses magasins en propre et ayant besoin d'analyser simultanément toutes les tendances de vente. Les données recueillies sur les clients proviennent donc de sources hétérogènes et ne seront, par conséquent, peut-être pas au même format. Le logiciel ETL va dans un premier temps collecter les données pertinentes auprès des différentes sources. Les données extraites sont ensuite stockées dans un data lake ou datawarehouse.

- Transform

La transformation constitue l'étape essentielle du processus ETL. En effet, après l'extraction, lors de laquelle les données brutes sont agrégées et stockées, celles-ci sont nettoyées et converties au format des rapports de l'entreprise. Le nettoyage facilite la mise en conformité avec les normes internes de l'entreprise. Ces opérations, sans lesquelles les rapports seraient inexploitables, sont basées sur des règles prédéfinies : la standardisation (qui statue entre autres sur le format et le mode de stockage), la déduplication (soit le suivi et la suppression des doublons), la vérification pour surveiller les anomalies et le tri ou regroupement des données.

- Load

Le processus ETL s'achève avec le chargement, complet ou incrémental, des données extraites et transformées dans le datawarehouse. Les équipes de Business Intelligence (BI) lancent ensuite des requêtes sur ces données, qui sont ensuite présentées aux utilisateurs finaux ou aux personnes chargées de prendre des décisions commerciales, ou utilisées comme entrées pour des algorithmes de Machine Learning.

![gougou](https://static.axysweb.com/uploads/2018/11/ETL-infographie-axysweb-1024x404.png)

### 3.2. Data Warehouse 

L’une des principales particularités d’une Data Warehouse est que les informations y sont classées par sujets (clients, produits…). De fait, ce qui définit réellement une Data Warehouse est le type de données qu’elle contient et les personnes qui l’utilisent.

Les Data Warehouses présentent de nombreux avantages. Pour les responsables informatiques, elles permettent notamment de séparer les processus analytiques des processus d’exploitation pour améliorer les performances dans ces deux domaines.


## 4. Points importants à retenir
- Au-delà des outils qu'il regroupe, l'ETL désigne aussi un processus fondamental dans l'analyse de données. Tu peux consulter [cette page de cours](https://openclassrooms.com/fr/courses/7168871-apprenez-les-bases-du-langage-python/7296776-extrayez-et-transformez-des-donnees-avec-l-extraction-web) pour comprendre ce que veut dire plus généralement le processus ETL.

- Il faut bien comprendre ce qu'est un **système « opérationnel » ou « de gestion »**, également appelé système OLTP (*on-line transaction processing*). Ces systèmes sont dédiés aux métiers de l'entreprise pour les assister dans leurs tâches de gestion quotidiennes. La tendance est à l'utilisation de P.G.I. (progiciels de gestion intégrée) qui regroupent tous les logiciels de gestion de l'entreprise – finances, ressources humaines, logistique, ventes, etc. – en un unique progiciel paramétrable aux règles de l'entreprise. Qui est à différencier d'un **système « décisionnel »**, également appelés OLAP (*on-line analytical processing*). Ces systèmes sont dédiés au management de l'entreprise pour l'aider au pilotage de l'activité. Ils offrent au décideur une vision transversale de l'entreprise. La tendance pour réaliser un système décisionnel est à la mise en place d'un entrepôt de données, ou data warehouse.

Dans un système OLTP, les données ne sont conservées que sur une courte période ; elles sont détaillées, personnelles, identifiées. A l'inverse, dans un système OLAP, les données sont historisées et peuvent être agrégées et anonymes.


## 5. Pour aller plus loin
Si l'univers du Big Data t'intéresse, tu peux lire ces 2 articles de la société Talend, le leader des ETL open source : 
- [Guide du processus ETL](https://www.talend.com/fr/resources/guide-etl/)
- [Différences entre lacs de données et entrepôts de données](https://www.talend.com/fr/resources/data-lake-vs-data-warehouse/)
