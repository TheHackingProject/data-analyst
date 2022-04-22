# Data Warehouse et ETL : les piliers de la BI
Quelques mots anglais qui paraissent barbares mais qui constituent la base de l'informatique décisionnel. Si tu décides de faire de la data (par opposition au développement logiciel), ce sont ces outils que tu utiliseras.

## 1. Introduction
Le *Data warehouse*, ou entrepôt de données, est une base de données dédiée au stockage des données pour l'analyse décisionnelle. Il est alimenté en données depuis les bases de production grâce aux outils d'ETL (Extract Transform Load). Cette ressource, à la frontière de la culture générale, va te permettre de mieux comprendre les enjeux actuels de la data 👻👻

📌 *Utilité pour le projet* : 3/5 pour le projet 2<br/>
📊 *Utilité pour être Data Analyst* : 4/5<br/>
💡 *Pourquoi cette ressource ?* : Pour comprendre le type de base de données que tu vas manipuler quand tu feras de la *Business Intelligence*.

## 2. Historique et contexte
Les premiers logiciels **Extract-Transform-Load** ont été développés au milieu des années 1970. A cette époque, les entreprises commençaient à utiliser plusieurs sources de données et à gérer différentes bases pour stocker différentes sortes de données business. Très tôt, le besoin s’est fait sentir d’agréger ces données. Au tournant des années 1980 – 1990, un type de plateforme s’est imposé comme solution de référence pour recevoir toutes ces données transformées et faire office de référentiel data : le Data Warehouse.

Un **Data Warehouse** (ou entrepôt de données) est une base de données relationnelle pensée et conçue pour les requêtes et les analyses de données, la prise de décision et les activités de type Business Intelligence, davantage que pour le traitement de transactions. Les Data Warehouses sont utilisés depuis près de 30 ans. 

## 3. La ressource

### 3.1. Les 3 étapes de l'ETL

Comme son nom l'indique, l'ETL se décompose en trois phases : l'extraction, la transformation et le chargement.

- Extract

Pour vous représenter le fonctionnement d'un ETL, prenez l'exemple d'une entreprise vendant des biens à la fois en ligne et dans ses magasins en propre et ayant besoin d'analyser simultanément toutes les tendances de vente. Les données recueillies sur les clients proviennent donc de sources hétérogènes et ne seront, par conséquent, peut-être pas au même format. Le logiciel ETL va dans un premier temps collecter les données pertinentes auprès des différentes sources. Les données extraites sont ensuite stockées dans un data lake ou datawarehouse.

- Transform

La transformation constitue l'étape essentielle du processus ETL. En effet, après l'extraction, les données sont nettoyées et converties au format des rapports de l'entreprise. Le nettoyage facilite la mise en conformité avec les normes internes de l'entreprise. Ces opérations, sans lesquelles les rapports seraient inexploitables, sont basées sur des règles prédéfinies : la standardisation (qui statue entre autres sur le format et le mode de stockage), la déduplication (soit le suivi et la suppression des doublons), la vérification pour surveiller les anomalies et le tri ou regroupement des données.

- Load

Le processus ETL s'achève avec le chargement, complet ou incrémental, des données extraites et transformées dans le datawarehouse. Les équipes de Business Intelligence (BI) lancent ensuite des requêtes sur ces données, qui sont ensuite présentées aux utilisateurs finaux ou aux personnes chargées de prendre des décisions commerciales, ou utilisées comme entrées pour des algorithmes de Machine Learning.

![gougou](https://static.axysweb.com/uploads/2018/11/ETL-infographie-axysweb-1024x404.png)

### 3.2. Data Warehouse 

L’une des principales particularités d’un Data Warehouse est que les informations y sont classées par sujets (clients, produits…).

Les Data Warehouses présentent de nombreux avantages. Pour les responsables informatiques, ils permettent notamment de séparer les processus analytiques des processus d’exploitation pour améliorer les performances dans ces deux domaines.

Ils sont très utiles pour permettre aux entreprises d’accéder rapidement et facilement aux données en provenance de multiples sources de manière centralisée. De manière générale, un Data Warehouse permet de réduire le temps nécessaire pour l’analyse de données et la production de rapports et de faciliter ces tâches.


### 3.3. Quelles différences entre le Data Warehouse et la base de données opérationnelle ?

Il faut bien comprendre ce qu'on a commencé à voir mercredi. 

D'une part, une entreprise possède un **système « opérationnel » ou « de gestion »**, également appelé système OLTP (*on-line transaction processing*). Ces systèmes sont dédiés aux métiers de l'entreprise pour les assister dans leurs tâches de gestion quotidiennes. Les bases de données sont ici conçues de manière à ce que les données qu'elles contiennent soient accessibles et manipulables. Mais par ailleurs, l'entreprise a besoin d'un meilleur endroit pour conserver les données en provenance de diverses sources : un endroit qui  permet de maintenir un référentiel unique et d'exécuter des analyses sur toutes les sources de données et flux simultanément.

C'est pourquoi, dès qu'elles commencent à s'intéresser sérieusement à leurs données, les entreprises se dotent d'un **système « décisionnel »**, également appelés OLAP (*on-line analytical processing*). Ces systèmes sont dédiés au management de l'entreprise pour l'aider au pilotage de l'activité. Ils offrent au décideur une vision transversale de l'entreprise. La tendance pour réaliser un système décisionnel est à la mise en place d'un entrepôt de données, ou data warehouse.

Mais tu dois te demander : concrètement, quelles sont les différences entre les systèmes OLTP et systèmes OLAP ?

Voici quelques réponses qui vont t'éclairer : en raison de la structure des fichiers OLAP, il est beaucoup plus facile d'effectuer des requêtes et des analyses sur les données qu'ils contiennent, et n'importe qui peut interroger l'entrepôt de données avec un logiciel d'entrepôt de données ou une connaissance du SQL.

En revanche, alors qu'on s'attend à ce que les bases de données aient un temps de disponibilité de 99,99 %, les entrepôts de données n'ont généralement pas besoin d'avoir ce genre de temps de disponibilité. Les entrepôts de données ne sont pas constamment lus et écrits comme les bases de données le sont. La plupart des entrepôts de données se rafraîchissent avec les données des bases de données, souvent toutes les 24 heures environ.


## 4. Points importants à retenir
- Au-delà des logiciels, l'ETL désigne par extension un processus fondamental dans l'analyse de données. Finalement, tu entendras souvent cet acronyme de la part des experts data car il permet de nommer le processus qui sert à récolter des données à un endroit, à les manipuler un peu et à les sauvegarder dans un autre endroit.  

- En tant que Data Analyst, ton rôle est théoriquement d'utiliser les données déjà enregistrées (Loaded) dans l'entrepôt de données pour créer des tableaux de bord et faire des analyses. Donc normalement, ce n'est pas toi qui gères le fonctionnement du data warehouse. Néanmoins, dans la pratique, il existe un flou aujourd'hui entre Data Engineer et Data Analyst dans certaines entreprises. En fait, si l'entreprise n'a pas de Data Engineer à sa disposition, ce sera au Data Analyst d'aller aussi farfouiller (Extract), remettre en forme (Transform) et mettre à disposition (Load) les données du Data Warehouse. On en revient toujours à la fameuse compétence "couteau-suisse" que doit avoir le Data Analyst 😅


## 5. Pour aller plus loin
Si un jour tu te demandes s'il est temps pour ton entreprise de mettre en place un datawarehouse, voici plusieurs articles qui te seront utiles : 
- [Est-il temps de mettre en place un Datawarehouse dans votre entreprise ?](https://www.cartelis.com/blog/datawarehouse-mise-en-place/)
- [Comment créer son premier Data Warehouse ? Le guide complet pour les analystes débutants](https://www.cartelis.com/blog/creer-datawarehouse/)

