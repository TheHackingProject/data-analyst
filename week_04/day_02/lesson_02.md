# Les infrastructures, le socle du Big Data

## 1. Introduction
Aujourd'hui, on va te donner quelques notions techniques pour que tu aies des bases en architecture de données. Ainsi, tu pourras dialoguer avec des experts de ces sujets 👣👣

## 2. Historique et contexte
De la carte perforée créé par le fondateur d'IBM en 1890 au concept du Cloud computing : **le stockage et la gestion des données ont beaucoup évolué entre la fin des années 1800 et aujourd’hui**. Les énormes machines qui servaient jadis à entreposer les données se sont peu à peu miniaturisées, tout en gagnant en vitesse et en capacité, avant de finalement disparaître grâce à la virtualisation et au Cloud.

Pendant des décennies, lorsqu’un décideur avait besoin de données, il les demandait au service informatique qui devait les extraire par différents moyens. Le résultat de ce processus lent et fastidieux répondait rarement aux attentes et besoins du décideur. Dans ce contexte, **les difficultés pour accéder aux données nécessaires au bon moment limitaient le potentiel de la stratégie de l’entreprise**.

L’accessibilité et l’accroissement des données en temps réel provenant de sources internes et externes ont poussé les décideurs à exiger davantage de données plus rapidement. Le big data a été propulsé dans le monde réel par l’influence grandissante du cloud. 

Et maintenant que le problème du stockage est quasiment résolu avec les architectures Big Data distribuées, il reste la question de l’analyse même de ces données distribuées. Initiée par Google et Yahoo, c’est typiquement ce que permet l’architecture MapReduce en facilitant le développement de moteurs de calcul dans le cadre "Big Data" (framework Hadoop par exemple). 

Finalement, **la conception d'une architecture de données moderne permet de combler les attentes des business strategists et des experts techniques**. Ensemble, ils peuvent déterminer les données nécessaires pour développer l’entreprise, les sources de ces données et leur mode de distribution afin de fournir des informations exploitables aux décideurs.


## 3. La ressource

### 3.1. Définitions : infrastructure et architecture

**L’architecture informatique représente le modèle constructif d’une infrastructure IT**. Il détermine l’organisation du système d’informations et le rôle de chaque élément (facteur humain, matériels, logiciels et progiciels, réseau ou autres).

**L’infrastructure informatique regroupe l’ensemble des équipements matériels (postes de travail, serveurs, routeurs, périphériques…) et logiciels (ERP, CRM, messagerie, réseau…) d’une entreprise**. Elle représente l’agencement entre : les différentes applications, le service de stockage et le réseau d’entreprise. Tous ces éléments, qui sont connectés entre eux, forment l’infrastructure informatique. 

Les infrastructures informatiques sont traditionnelles ou cloud :
- **Une infrastructure IT traditionnelle** est constituée des composants matériels et logiciels habituels : installations, centres de données, serveurs, matériel réseau, ordinateurs de bureau et solutions logicielles d'applications d'entreprise. Généralement, cette configuration d'infrastructure requiert plus de puissance, d'espace physique que les autres types d'infrastructure ; elle est aussi plus coûteuse. Une infrastructure traditionnelle est généralement installée sur site ; elle est dédiée à une utilisation privée, pour l'entreprise uniquement.
- **Une infrastructure IT de cloud computing** est similaire à l'infrastructure traditionnelle. Cependant, les utilisateurs finaux peuvent accéder à l'infrastructure via Internet, avec la possibilité d'utiliser des ressources informatiques sans installation sur site, grâce à la virtualisation. La virtualisation connecte des serveurs physiques gérés par un fournisseur de services à un ou plusieurs emplacements géographiques. Ensuite, elle divise et abstrait des ressources, comme le stockage, pour les rendre accessibles aux utilisateurs presque partout où une connexion Internet peut être établie. 

**Les configurations de l'infrastructure IT varient selon les besoins et les objectifs des entreprises**, mais certains objectifs sont communs à elles toutes. L'infrastructure optimale fournira un stockage métier hautes performances, un réseau à faible latence, la sécurité, un réseau WAN optimisé, la virtualisation et zéro indisponibilité.

Pour comprendre le rôle des composants d'une infrastructure IT, tu peux lire [cette page](https://bluebearsit.com/infrastructure-informatique).

___

👽👽 Et pour la data, ça donne quoi ? 👽👽

**L’architecture de données** est le processus qui permet de standardiser la façon dont les entreprises collectent, stockent, transforment, distribuent et utilisent les données.

**L'infrastructure data** s’appuie sur quatre composantes essentielles qui permettent de collecter, stocker, analyser et enfin, visualiser les données traitées. À travers ces quatre étapes, le système est capable d’assurer la transformation des données stockées par votre entreprise.

___

### 3.2. Les solutions de collecte de données

Les capteurs des appareils électroniques, des véhicules, des bâtiments, des machines, ou ceux présents sur les emballages des produits permettent de collecter des données. Les applications informatiques sont également sources de données. 

La collecte de données est un processus visant à rassembler vos données sur une plateforme unique. Elle se fait soit de manière automatique (via un outil ETL), soit de manière manuelle, ce qui est souvent fastidieux et chronophage.


### 3.3. Les solutions de stockage de données

Le stockage de données est le processus selon lequel les systèmes informatiques archivent, organisent et partagent les octets qui constituent les éléments qu'on utilise au quotidien, des applications aux protocoles réseau, en passant par les documents, les contenus multimédias, les carnets d'adresses et les préférences utilisateur. 

On pourrait comparer le fonctionnement d'un ordinateur à celui d'un cerveau. Tous deux ont des mémoires à court et long terme. Le cerveau gère la mémoire à court terme dans le cortex préfrontal tandis que l'ordinateur utilise la RAM (Random Access Memory).

Le cerveau et la RAM traitent et retiennent les informations qui leur parviennent durant la phase d'éveil, et finissent par être fatigués. Le cerveau convertit les éléments de mémoire de travail en mémoires à long terme durant la phase de sommeil, tout comme l'ordinateur transfère la mémoire active vers des volumes de stockage lorsqu'il est en veille. 

Pour aider les entreprises à faire face au volume sans cesse croissant des données à stocker, il existe plusieurs types de stockage de données : 
- **Le stockage logiciel ou SDS** est un système de stockage qui se base sur des serveurs physiques. Cependant, un logiciel de stockage délivre les fonctionnalités d’hébergement. Ainsi, la couche logicielle fonctionne indépendamment du matériel de stockage physique.
- **Le stockage des données en local ou en réseau**. Une box (serveur de stockage) accueille vos données et applications localement au sein de votre entreprise. Toutes les données à sauvegarder sont collectées sur le réseau puis cryptées et compressées avant d’être stockées sur les disques durs présents dans la box.
- **Le stockage dans le cloud**. Le stockage dans le cloud est l'organisation des données stockées dans un emplacement accessible depuis Internet par toute personne qui dispose d'une autorisation. Vous n'avez pas besoin de vous connecter à un réseau interne (on parlerait alors de serveur de stockage en réseau) et vous n'accédez pas aux données à partir de matériel directement relié à votre ordinateur. Amazon, Microsoft, Google et IBM sont actuellement les principaux fournisseurs de stockage dans le cloud.
- **Le stockage des données en hybride**. Les solutions de stockage hybrides stockent les données actives et fréquemment consultées sur du stockage Flash (une alternative à l'utilisation des disques durs qui peut offrir des performances et une efficacité optimales) tout en conservant les données inactives ou moins importantes sur des supports plus économiques. Cela permet aux entreprises de gérer des données dans un système de stockage unifié tout en trouvant le juste équilibre entre les performances et les coûts.

### 3.4. Les solutions d'analyse de données
L’objectif final de cette procédure est la transformation des données en connaissance utilisable. Pour ce faire, l’utilisation d'un langage programmatif ou de plateformes analytiques est incontournable. IBM, Oracle ou encore Google (et bien d'autres fournisseurs) proposent des outils Big Data pour transformer des données brutes en informations. BigQuery (Google) est conçu par exemple pour permettre à toute personne avec un peu de connaissances de traiter de de vastes ensembles de données. Cloudera, HDInsight (Microsoft) et Amazon Web Services sont aussi sur ce créneau. Et de nombreuses startups proposent également des solutions sur ce champs.

### 3.4. Les solutions de visualisation de données
On a déjà vu les outils de visualisation répandus sur le marché (Tableau, PowerBI, Qlik etc.).

## 4. Points importants à retenir
Un travail sérieux réalisé sur les quatre étapes du traitement de la donnée permettra à votre entreprise d'obtenir l'infrastructure nécessaire à la réalisation de projets Big Data. N'hésitez pas à vous faire aider d'expert en architecture pour faire les bons choix d'infrastructure.

## 5. Pour aller plus loin
- Un article sur [L'infrastructure informatique, vecteur de l'essor de votre entreprise](https://www.appvizer.fr/magazine/services-informatiques/virtualisation/infrastructure-informatique)
- [Comment bien choisir son Data Warehouse](https://www.lemagit.fr/conseil/Bien-choisir-son-Data-Warehouse-nouvelle-generation)

