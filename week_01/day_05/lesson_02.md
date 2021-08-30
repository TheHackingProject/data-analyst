# Le Big Data
A quoi correspond techniquement cette révolution qu'on appelle communément "Big Data" et quelles sont ses conséquences sur l'analyse de données ?

## 1. Introduction
Tu viens de voir les deux familles d'outils indispensables à la Data Analyse : les langages de programmation et les bases de données 👏👏 Il te reste à voir encore deux familles d'outils : les outils d'analyse (que tu verras lors de la troisième semaine de la formation) et les outils Big Data, qu'on va voir dans cette ressource. Les outils Big Data sont apparus récemment et sont souvent gérés par des devs vue leur complexité. Mais il est important pour toi de comprendre leur utilité et leur fonctionnement.

## 2. Historique et contexte
On peut dater l’acte de naissance du big data en 2001 avec l’invention de la règle des 3V (Volume, Vitesse et Variété). A l’époque, l’expression traduisait une rupture dans le volume des données à traiter. Jusqu’à la fin des années 90, les quantités de données restaient limitées. Puis, on a assisté à une explosion du volume de données avec l’essor de l’e-commerce, des réseaux sociaux, des terminaux mobiles et, plus récemment, de l’internet des objets (IoT). Face à cette avalanche de data, les modèles techniques existants ont montré leurs limites. La base de données parfaite n’existait plus. En fonction du souhait de privilégier la volumétrie, la vitesse ou les capacités de requêtage, on choisira une solution plutôt qu’une autre ou bien une combinaison d’outils.

Pour leurs propres besoins, les GAFAM ont dû créer des outils pour stocker et traiter à la volée des données à la fois nombreuses et versatiles, leur structuration changeant avec le temps. Facebook est ainsi à l’origine de Cassandra avant de se tourner vers HBase (NoSQL), Google de BigTable et GFS (ancêtre d’HDFS) et plus récemment de TensorFlow (machine learning). Les géants du web ont ensuite versé ces projets en open source, externalisant en quelque sorte leur R&D. Car à leurs yeux, l’or ce sont les données elles-mêmes, pas les technologies. 
 
Finalement, après avoir été longtemps un buzzword, "Big Data" a repris son sens premier : il fait référence à l'ensemble des technologies comme Hadoop, Spark, Kafka ... que tu vas découvrir aujourd'hui.

## 3. La ressource

L'univers du Big Data est complexe et pourrait faire l'objet de plusieurs semaines de formation. Mais dans ton cas de futur Data Analyst, une journée suffira car tu as surtout besoin d'avoir les bases pour pouvoir ensuite naviguer dans un projet Big Data. En fait, ce n'est pas toi qui devras créer les infrastructures Big Data, c'est le rôle du *Data Engineer* ou *Data Architect*. On va donc te livrer ici les notions les plus importantes pour comprendre le Big Data.

https://matheo.uliege.be/bitstream/2268.2/2562/4/M%C3%A9moire%20Camille%20Marenne.pdf

https://inventiv-it.fr/big-data-devez-apprendre/

https://www.atys-concept.com/blog-de-la-performance/articles-performance-industrielle/differences-entre-data-analytics-data-science-big-data/

https://www.decideo.fr/Les-6-competences-les-plus-recherchees-en-Big-Data_a10051.html


### 3.1. Big data is not only big !

On pourrait penser que le Big Data (mégadonnées en français) se résume à des gros volumes de données. Mais sans parler de Big Data, il est aujourd’hui possible de stocker et d’exploiter de très gros volumes de données avec une grande variété de sources dans de grands entrepôts de données (les *Data Warehouses*). En effet, les technologies actuelles permettent de traiter des gros volumes de données selon les méthodes analytiques de Business Intelligence sans avoir recours au Big Data (cf. la ressource précédente).

Si le Big Data concerne effectivement des gros volumes de données, une de ses spécificités est de s’intéresser aussi bien aux données structurées qu’aux données non structurées. Ce sont les données non structurées que les outils habituels d’analytique ne savent pas traiter. Une autre spécificité est le stockage des données, qui ne sont plus stockées dans des *Data Warehouses* mais dans des *Data Lakes*. Finalement, plus que les volumes, ce qui fait le Big Data est donc la nature des données, la manière dont on les stocke et les techniques d’analyse pratiquées avec des savoir-faire et des technologies propres.

En fait, au tout début, on a parlé des 3V : volume (grandes quantités), variété (différents types de données) et vélocité (rapidité de traitement). Mais ce que l’acronyme des 3V ne mettait pas en perspective, c’était cette innovation centrale qui veut que **les données n’ont pas besoin d’être systématiquement « transformées » pour être analysées**. Apparaissait donc une nouvelle approche, très différente de l'approche ETL où La donnée est structurée et convertie à des formats précis. 

⚠️⚠️ Ne croyez pas pour autant que les big data rendent les *data warehouses* obsolètes. Les systèmes de big data vous amènent à travailler avec des données non structurées, mais le type de résultats de requêtes que vous obtenez est loin de la sophistication des *data warehouses*. La *data warehouse* est conçue pour une analyse en profondeur de la donnée, et cela est rendu possible précisément parce que la donnée a été transformée et prévue dans un format spécifique.

Le big data permet d’analyser beaucoup plus de données de beaucoup plus de sources, mais avec une résolution moins fine. Pour schématiser, on peut dire que le big data est un monde impressionniste qui aura toujours besoin à ses côtés de l’hyper-réalisme des *data warehouses* 🎨 C’est pour cela que nous sommes condamnés à vivre à la fois avec les *data warehouses* traditionnelles  et ce nouveau style de traitement que sont les big data. Le big data ne consiste donc surtout pas à désapprendre ce que l’on a appris en se formant au *data warehouse*. Le data scientist n’a pas forcément vocation à prendre la place de l’ingénieur en informatique décisionnelle. Il faudra au contraire que l’entreprise se pose la question de comment faire en sorte que les deux s’enrichissent mutuellement. Et c'est aussi ces deux aspects que nous allons t'apprendre dans cette formation.

___

💡💡 AIDE MNÉMOTECHNIQUE 💡💡

Pour synthétiser, le Big Data c'est non pas 3 mais 5Vs à la fois : 
- **Volume** -> des ensembles de données très volumineux 
- **Vitesse** ou **Vélocité** -> la vitesse à laquelle les données sont générées et à laquelle elles se déplacent
- **Variété** -> en fait, 80% des données dans le monde ne sont plus structurées et ne peuvent donc pas être facilement mises dans des tables ou des bases de données relationnelles - pense à des photos, des séquences vidéos ou des mises à jour de réseaux sociaux ⌚️📱
- **Véracité** -> les données sont devenues incertaines : il faut gérer la fiabilité de données intrinsèquement imprécises.
- **Valeur** -> finalement, tous ces volumes de données variées en mouvement rapide et de véracité différente doivent être transformés en valeur ! C'est là l'enjeu majeur du Big Data ⚖️⚖️

___


### 3.2. Les technos du Big Data

#### 3.2.1 Hadoop


#### 3.2.2 MapReduce

#### 3.2.3 Spark 

Google est à l’origine des deux percées technologiques qui ont rendu les big data possibles :

Le premier était Hadoop, qui consiste en deux services clés :

    un système de stockage de données, utilisant HDFS (Hadoop Distributed File System)
    un système de process de données en parallèle, utilisant une technique appelée Map Reduce.

Hadoop fonctionne sur un ensemble de serveurs en architecture shared-nothing. On peut ajouter ou enlever des serveurs à volonté dans un cluster Hadoop. Le système détecte et règle les problème sur chaque serveur. Hadoop, en d’autres termes, « s’auto-guérit ». Il peut donc continuer à délivrer des données et fonctionner à grande échelle en effectuant des tâches exigeant de hautes performances, malgré des changements ou des échecs.

Sa véritable valeur ajoutée est cependant encore ailleurs : elle provient de adds-on et de compléments personnalisables de sa technologie. Hadoop offre ainsi des projets supplémentaires qui ajoutent des fonctionnalités à la plateforme :

    Hadoop Common: il s’agit des outils de base nécessaires aux autres projets Hadoop
    Chukwa: un système de récupération de données pour gérer les systèmes distribués de grande taille.
    HBase: une base de données distribuée, scalable qui supporte le stockage de données structurées pour de grandes tables.
    HDFS: un système distribué qui procure des accès haut débit aux données d’application
    Hive: une infrastructure de data warehouse qui délivre de la data summarization et un système de requêtes ad hoc.
    MapReduce: un framework logiciel pour les process distribués de sets de données importants
    Pig: un langage et un framework permettant l’exécution de process parallèles.
    ZooKeeper: un service de coordination haute performance pour les applications distribuées.

L’implémentation  d’une plateforme Hadoop comprend forcément quelques un de ces sous-projets.

Par exemple, de nombreuses organisations choisissent d’utiliser HDFS comme système primaire de gestion de fichiers distribués et HBase comme base de données qui peut stocker des milliards de colonnes de données. Et le recours à MapReduce (ou Spark) va s’imposer ensuite presque de soi puisqu’il apporte la vitesse et l’agilité à la plateforme Hadoop.

Avec MapReduce, les développeurs peuvent créer des programmes qui traitent des volumes massifs de données non structurées en parallèle à travers un cluster de processeurs distribués sur des ordinateurs indépendants. Le framework MapReduce est scindé en deux espaces fonctionnels :

    Map, une fonction qui répartit le travail à différents noeuds dans les grappes d’ordinateurs.
    Reduce, une fonction qui rassemble le travail et résume les résultats dans une valeur simple.

Un des avantages primaires de Map Reduce est qu’il est « fault-tolerant » ou tolérant aux pannes. Comment fait-il ? Il « monitore » chaque noeud (node) du cluster régulièrement. Celui-ci est supposé renvoyer périodiquement un travail complet avec des mises à jour des « status ». Si un noeud reste silencieux plus que nécessaire, un master node le signale et réassigne le travail à d’autres noeuds du cluster.

Construit à l’origine pour indéxer le moteur de recherche Nutch, Hadoop est maintenant utilisé dans tous les grands secteurs d’activité pour quantité de tâches big data.

En d’autres termes, grâce au système d’informatique distribuée HDFS et YARN (Yet Another Resource Negotiator), le logiciel permet à l’utilisateur de traiter des volumes de données gigantesques répartis à travers des milliers d’ordinateurs, exactement comme s’ils étaient une seule et même énorme machine.

Comment adapter cela à votre cas ? L’histoire de ces sauts technologiques s’impose forcément à votre organisation et à vous-même. L’informatique distribuée ne vous est pas suffisamment familière ? Il est urgent de mieux la comprendre et de vous y former, vous ou vos équipes. 

Quant aux outils, l’histoire d’Hadoop montre à quel point sa logique s’impose à l’univers Big Data. Son univers ne doit donc pas vous rester étranger. Songez-y. Mais l’histoire n’est pas finie. 

En 2009, des cherchers de l’Université de Californie à Berkeley ont développé Apache Spark , une alternative à MapReduce. Spark procède à ses calculs en parallèle en utilisant du stokage in-memory, il est jusqu’à 100 fois plus rapide que MapReduce. Spark peut être utilisé seul ou à l’intérieur d’Hadoop.

Même avec Hadoop, il faut quand même un moyen de stocker et d’accéder aux données. C’est typiquement ce à quoi servent des NoSQL database telles que Mongo DB, CouchDG ou Cassandra, spécialisées dans le traitement des données non-structurées ou semi-structurées et distribuées à travers de multiples machines.

A la différence de ce qui se passe dans les data warehouses, où des quantités massives de données sont envoyées vers un format unifié et sont stockées dans un data store unique, ces outils ne changent pas la nature ni la localisation de la donnée d’origine – les emails restent des emails, les données de capteurs restent des données de capteurs- et peuvent être stockés virtuellement n’importe où.

Reste un problème : disposer de quantités massives de données dans des bases NoSQL installées dans des clusters de machines n’est pas très utile tant que vous n’en faites rien.
C’est là qu’interviennent les analytics de big data.

Des outils tels que  Tableau, Splunk, et Jasper BI permettent de parser ces data pour identifier des patterns, extraire des significations et révéler de nouvelles perspectives. Ce que vous en ferez ensuite dépendra de vos besoins.

Là encore, les compétences dans ces analytics sont particulièrement demandées. Cela fait partie des compétences à acquérir. Noter également que la maîtrise des bases NoSQL semble importante, voire indispensable. Connaître et maîtriser le NoSQL semble donc à ce jour indispensable à l’univers big data. Quoique…dans cet article, vous verrez que SQL revient en force dans l’univers big data. 


## 4. Points importants à retenir
Au-delà des buzz words, l'analyse de données prend différentes formes et peut se réaliser à différents niveaux. On peut distinguer deux types d'analyses : 
- l'analyse de données au travers de logiciels de *Business Intelligence* qui permet de faire parler les données, le plus souvent déjà collectées et stockées dans l’entreprise.
- l’analytique Big Data qui nécessite l’intervention de spécialistes et la mise en œuvre d’une architecture informatique et d’outils complexes. 


## 5. Pour aller plus loin


peut-être mettre une blague ex : "si tu me crois pas qu'Hadoop est indispensable, cf https://www.decideo.fr/Les-6-competences-les-plus-recherchees-en-Big-Data_a10051.html"
