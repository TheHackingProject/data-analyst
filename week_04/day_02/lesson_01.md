# Data Architect et Data Engineer

## 1. Introduction
On a déjà vu rapidement lors de la première semaine quel était le rôle du Data Engineer et à quel moment il intervenait par rapport au Data Analyst. Mais comme ces rôles sont très importants, nous allons revoir en détail ces métiers qui gèrent la collecte et le stockage des données.

## 2. Historique et contexte
Il est difficile de dater avec précision l’apparition des ingénieurs de la donnée. C’est dans les années 1980 que le terme  *information engineering* est inventé pour décrire la conception des bases de données et pour inclure l’ingénierie logicielle à l’analyse de données.

Mais avec l’essor d’Internet dans les années 1990 et 2000, les administrateurs de bases de données, développeurs SQL et autres professionnels de l’informatique liés à ce domaine n’étaient pas encore considérés comme des "Data Engineers".

Ce terme a été popularisé en 2011 par des entreprises data-driven comme Facebook et AirBnB. Les ingénieurs logiciels de ces entreprises assises sur des mines d’or de données avaient besoin de créer des outils pour exploiter ces informations.

**Le rôle du Data Engineer** consistait à l’époque à utiliser des outils ETL traditionnels. Il **a toutefois évolué pour développer ses propres outils afin de prendre en charge les volumes de données toujours plus importants**.

Désormais, suite à l’envol du Big Data, le Data Engineering est une catégorie d’ingénierie logicielle focalisée sur les données à travers l’infrastructure, le Data Warehousing, le forage et la modélisation de données ou encore la gestion des métadonnées.

## 3. La ressource

### 3.1. *Data Architect* ou architecte data

Le Data Architect a pour mission d’**optimiser la collecte et le stockage de données** ou de données massives (Big Data) numériques internes ou externes à l’entreprise. Après avoir évalué les besoins, il fait le choix des solutions techniques les plus adaptées afin de construire une architecture de gestion des données. Il pilote la mise en place et l’évolution permanente des outils de collecte et de gestion des données en tenant compte des usages et dans une recherche d’optimisation des coûts et de la qualité. 

Dans cette perspective, **il effectue une veille technologique afin de maîtriser les dernières technologies relatives aux données et au Big Data**. Il a également la charge de s’assurer que les solutions mises en place respectent la réglementation relative à la collecte et à l’exploitation des données (RGPD). Rattaché à la direction des systèmes d’information de l’entreprise, il travaille en étroite collaboration avec les data engineer, qui développent les solutions de gestion des données, et les data analyst et scientist, qui analysent les données brutes collectées.

Les Data Architects sont assez proches d’un autre métier de la data : le Data Engineer. Ce dernier construit et maintient l’architecture informatique liées aux données, soit tous les outils et les fonctionnalités conçus et mis en place par le Data Architect ! **Le Data Architect intervient avant le Data Engineer dans la construction de systèmes d’information liés à la donnée**. Une fois les outils conçus et prêts à être utilisés par les métiers, le Data Engineer prend la relève.

Le métier paraît complexe, non ? En effet, Data Architect n’est pas un emploi de début carrière et nécessite une expérience professionnelle préalable de quelques années (entre 5 et 10 ans), par exemple en tant que Data Engineer, architecte logiciel ou expert en base de données.

A savoir enfin : ce rôle devient de plus en plus clé dans un contexte d’architecture Cloud, ouverte, de temps réel et de contraintes de cyber sécurité et réglementaires 😎😎

___

🤔🤔 Quelles compétences faut-il avoir pour être architecte data ? 🤔🤔

Voici une liste non exhaustive qui t'aidera à y voir plus clair : 
- Maîtrise de l’environnement Hadoop/Spark/Yarn (que ce soit en local ou sur cloud) 
- Maîtrise des systèmes d’exploitation (Unix, Windows, etc.) 
- Maîtrise de langages de programmation (C++, Java, Python, R, Scala, etc.) 
- Maîtrise en base de données (SQL/NoSQL) et gestion de base de données 
- Maîtrise d’un outil de gestion de flux (Kafka, Flink, etc.)  
- Bonne compréhension et connaissance des interfaces réseaux et de l’infrastructure matérielle  
- Connaissance de la réglementation concernant les données personnelles et des principes de cybersécurité  
- Connaissance des solutions de manipulation des données ETL/ELT  
- Bonne compréhension de la stratégie d’entreprise et des besoins business

___

### 3.2. *Data Engineer* ou ingénieur des données

Dans le détail, les responsabilités qui sont confiées au Data Engineer peuvent fortement varier d’une organisation à l’autre. 

Souvent, il doit **développer des pipelines de données pour assembler les données en provenance de multiples systèmes**. Il doit aussi intégrer, consolider, nettoyer et structurer les données pour qu’elles puissent être utilisées dans des applications analytiques individuelles. C’est lui qui se charge de **mettre en place et de maintenir l’infrastructure de données** sur laquelle sont basés les systèmes informatiques et les applications de l’entreprise. Par *data engineering*, on entend qu’ils sont responsables du développement, de la construction, de la maintenance et du test des architectures, telles que les bases de données et les systèmes de traitement.

L’ingénieur des données officie généralement au sein d’une équipe analytique. Son rôle est alors de fournir des données prêtes à l’usage aux Data Scientists, afin qu’ils puissent effectuer des requêtes à des fins d’analyse prédictive, de Machine Learning ou de Data Mining. En effet, pour analyser et exploiter les données, les Data Scientists ont besoin de données de haute qualité. Le rôle des ingénieurs est de collecter et de préparer les données pour qu’elles puissent être utilisées.

Quels sont les compétences du Data Engineer ? 🤠

- **Connaissance approfondie de SQL et autres langages de base de donnée** : le Data Engineer doit maîtriser les outils de gestion des bases de données (BDD) et avoir une bonne connaissance en SGBDR (SQL, DB2…). Une maîtrise d’autres technologies de requêtage telles que Cassandra ou Bigtable, sont intéressantes en fonction des technologies utilisées par l’entreprise, d’autant plus que les grandes entreprises ne se contentent souvent pas d’une seule technologie de requêtage.

- **Stockage de données et outils ETL** : la maîtrise des outils de stockage de données (Hadoop) et des ETL (Talend, Nifi…) du marché est essentielle ;

- **Analyses basées sur Hadoop (Hbase, Hive, etc.)** : une bonne compréhension de l’analyse de donnée basée sur Apache Hadoop est une compétence de plus en plus courante dans le métier de Data Engineer, les connaissances de Hbase ou Hive étant souvent considérées comme un must-have sur les postes de Data Engineer middle & Senior. On en demandera moins aux Data Engineers juniors.

- **Maîtrise du Code** : la connaissance d’une ou plusieurs langues de programmation est un vrai plus et devient même un prérequis. On exigera une familiarité, sinon une expertise dans un des langages suivants : Python, C / C ++, Java, Scala, Perl, ou dans d’autres langues similaires.

- **Machine Learning, Deep Learning et Intelligence Artificielle** : bien que ce soit principalement le domaine de compétences du data scientist, un certain niveau de compréhension sur ces domaines représente évidemment un atout afin de pouvoir travailler en collaboration avec les Data Scientists. Pour cette raison, une certaine connaissance de l’analyse statistique et de la modélisation des données peuvent s’avérer utiles, tout comme des connaissances dans le domaine de l’apprentissage automatique. L’ensemble de ces compétences « bonus » servent aussi à se démarquer, car être capable de « mettre les deux chapeaux » est inestimable pour une entreprise.

- **Divers systèmes d’exploitation** : UNIX, Linux et Solaris.

## 4. Points importants à retenir
Dans un projet data, on considère souvent que la valeur réside dans l’algorithme permettant de transformer automatiquement et rapidement des données massives en une information non triviale : recommandation de produits, traduction, reconnaissance faciale…, de fait, le data scientist – chargé du développement de cet algorithme – semble être l’acteur essentiel du projet.

C’est partiellement faux, pour une raison très simple : **la valeur ajoutée réside, en majeure partie, dans les données elles-mêmes**. Pour faire simple, le data scientist ne pourra jamais faire mieux que ce que les données lui permettent de faire. C’est pourquoi **les profils Data Architect et Data Engineer sont essentiels : c’est eux qui créent, entretiennent et améliorent les systèmes d’information permettant aux autres membres de l’équipe data de faire leur travail**. Sans eux, les data scientist passeront probablement plus de temps à administrer les données qu’à les analyser.

## 5. Pour aller plus loin
Pour mieux comprendre l'ensemble des métiers existants dans la data, tu peux attendres les autres jours de la semaine. Mais tu peux aussi consulter ces docs très complètes :
- [Le glossaire des principaux métiers de la data](https://syntec-conseil.fr/wp-content/uploads/2020/09/Syntec-Conseil_Glossaire-des-principaux-m%C3%A9tiers-de-la-Data.pdf)
- [Les métiers de la data, par l'APEC](https://corporate.apec.fr/files/live/sites/corporate/files/Nos%20%C3%A9tudes/pdf/Les-metiers-de-la-data.pdf)
... et toujours bien sûr consulter les offres d'emploi 🙃
