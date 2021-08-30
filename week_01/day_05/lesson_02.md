# Le Big Data
A quoi correspond techniquement cette révolution qu'on appelle communément "Big Data" et quelles sont ses conséquences sur l'analyse de données ?

## 1. Introduction
Tu viens de voir les deux familles d'outils indispensables à la Data Analyse : les langages de programmation et les bases de données 👏👏 Il te reste à voir encore deux familles d'outils : les outils d'analyse (que tu verras lors de la troisième semaine de la formation) et les outils Big Data, qu'on va voir dans cette ressource. Les outils Big Data sont apparus récemment et sont souvent gérés par des devs vue leur complexité. Mais il est important pour toi de comprendre leur utilité et leur fonctionnement.

## 2. Historique et contexte
On peut dater l’acte de naissance du big data en 2001 avec l’invention de la règle des 3V (Volume, Vitesse et Variété). A l’époque, l’expression traduisait une rupture dans le volume des données à traiter. Jusqu’à la fin des années 90, les quantités de données restaient limitées. Puis, on a assisté à une explosion du volume de données avec l’essor de l’e-commerce, des réseaux sociaux, des terminaux mobiles et, plus récemment, de l’internet des objets (IoT). Face à cette avalanche de data, les modèles techniques existants ont montré leurs limites. La base de données parfaite n’existait plus. En fonction du souhait de privilégier la volumétrie, la vitesse ou les capacités de requêtage, on choisira une solution plutôt qu’une autre ou bien une combinaison d’outils.

Pour leurs propres besoins, les GAFAM ont dû créer des outils pour stocker et traiter à la volée des données à la fois nombreuses et versatiles, leur structuration changeant avec le temps. Facebook est ainsi à l’origine de Cassandra avant de se tourner vers HBase (NoSQL), Google de BigTable et GFS (ancêtre d’HDFS) et plus récemment de TensorFlow (machine learning). Les géants du web ont ensuite versé ces projets en open source, externalisant en quelque sorte leur R&D. Car à leurs yeux, l’or ce sont les données elles-mêmes, pas les technologies. 
 
Finalement, après avoir été longtemps un buzzword, "Big Data" a repris son sens premier : il fait référence à l'ensemble des technologies comme Hadoop, Spark, les bases de données NoSQL ... que tu vas découvrir aujourd'hui.

## 3. La ressource

L'univers du Big Data est complexe et pourrait faire l'objet de plusieurs semaines de formation. Mais dans ton cas de futur Data Analyst, une journée suffira car tu as surtout besoin d'avoir les bases pour pouvoir ensuite naviguer dans un projet Big Data. En fait, ce n'est pas toi qui devras créer les infrastructures Big Data, c'est le rôle du *Data Engineer* ou *Data Architect*. On va donc te livrer ici les notions les plus importantes pour comprendre le Big Data.

### 3.1. Big data is not only big !

On pourrait penser que le Big Data (mégadonnées en français) se résume à des gros volumes de données. Mais sans parler de Big Data, il est aujourd’hui possible de stocker et d’exploiter de très gros volumes de données avec une grande variété de sources dans de grands entrepôts de données (les *Data Warehouses*). En effet, les technologies actuelles permettent de traiter des gros volumes de données selon les méthodes analytiques de Business Intelligence sans avoir recours au Big Data (cf. la ressource précédente).

Si le Big Data concerne effectivement des gros volumes de données, une de ses spécificités est de s’intéresser aussi bien aux données structurées qu’aux données non structurées. Ce sont les données non structurées que les outils habituels d’analytique ne savent pas traiter. Une autre spécificité est le stockage des données, qui ne sont plus stockées dans des *Data Warehouses* mais dans des *Data Lakes*. Finalement, plus que les volumes, ce qui fait le Big Data est donc la nature des données, la manière dont on les stocke et les techniques d’analyse pratiquées avec des savoir-faire et des technologies propres.

En fait, au tout début, on a parlé des 3V : volume (grandes quantités), variété (différents types de données) et vélocité (rapidité de traitement). Mais ce que l’acronyme des 3V ne mettait pas en perspective, c’était cette innovation centrale qui veut que **les données n’ont pas besoin d’être systématiquement « transformées » pour être analysées**. Apparaissait donc une nouvelle approche, très différente de l'approche ETL où La donnée est structurée et convertie à des formats précis. 

⚠️⚠️ Ne croyez pas pour autant que les big data rendent les *data warehouses* obsolètes. Les systèmes de big data vous amènent à travailler avec des données non structurées, mais le type de résultats de requêtes que vous obtenez est loin de la sophistication des *data warehouses*. La *data warehouse* est conçue pour une analyse en profondeur de la donnée, et cela est rendu possible précisément parce que la donnée a été transformée et prévue dans un format spécifique.

Le big data permet d’analyser beaucoup plus de données de beaucoup plus de sources, mais avec une résolution moins fine. Pour schématiser, on peut dire que le big data est un monde impressionniste qui aura toujours besoin à ses côtés de l’hyper-réalisme des *data warehouses* 🎨 C’est pour cela que nous sommes condamnés à vivre à la fois avec les *data warehouses* traditionnelles  et ce nouveau style de traitement que sont les big data. Le big data ne consiste donc surtout pas à désapprendre ce que l’on a appris en se formant au *data warehouse*. Le data scientist n’a pas forcément vocation à prendre la place de l’ingénieur en informatique décisionnelle. Il faudra au contraire que l’entreprise se pose la question de comment faire en sorte que les deux s’enrichissent mutuellement. Et c'est aussi ces deux aspects que nous allons t'apprendre dans cette formation.

___

💡💡 AIDE MNÉMOTECHNIQUE 💡💡

Pour synthétiser, le Big Data c'est une famille d'outils qui répondent non pas à 3 mais à 5Vs à la fois : 
- **Volume** -> des ensembles de données très volumineux 
- **Vitesse** ou **Vélocité** -> la vitesse à laquelle les données sont générées et à laquelle elles se déplacent
- **Variété** -> en fait, 80% des données dans le monde ne sont plus structurées et ne peuvent donc pas être facilement mises dans des tables ou des bases de données relationnelles - pense à des photos, des séquences vidéos ou des mises à jour de réseaux sociaux ⌚️📱
- **Véracité** -> les données sont devenues incertaines : il faut gérer la fiabilité de données intrinsèquement imprécises.
- **Valeur** -> finalement, tous ces volumes de données variées en mouvement rapide et de véracité différente doivent être transformés en valeur ! C'est là l'enjeu majeur du Big Data ⚖️⚖️

___


### 3.2. Les technos du Big Data

Quatre grandes révolutions techniques ont permis la création et la croissance du Big Data :

- **L’évolution du hardware de stockage**, passant de serveurs physiques internes à l’entreprise à **des serveurs dits “cloud”** qui ont souvent une capacité de stockage bien supérieure. Au début des années 2000, sont apparus des hébergeurs web capables d'héberger des applications dans leurs locaux informatiques. 

- **De nouvelles techniques de calcul**. Au départ développée par Google, la technologie MapReduce a permis des vitesses de traitement très rapides sur de gros volumes de données.

- **Un nouveau modèle d'architecture**. Ce paradigme a été popularisé par Google au début des années 2000 et est à l’origine de la première version open source du premier framework Big Data : Hadoop. L’idée n’est plus de centraliser le stockage et le traitement des données sur un serveur, mais de distribuer leur stockage et de paralléliser leur traitement sur plusieurs ordinateurs.

- **Un nouveau type de bases de données : le NoSQL**. 

#### 3.2.1 Le cloud computing

Avant l’arrivée des plateformes informatiques cloud, le stockage et l’utilisation du Big Data étaient effectués sur site. L’introduction des plateformes en cloud computing comme Microsoft Azure, Amazon AWS ou Google BigQuery permet désormais d’effectuer ce processus de management de la donnée à distance.

Ce n’est pas une technologie Big Data pure et dure, mais c’est la méthode de déploiement favorisée pour les technologies Big Data. En effet, celui-ci demande des capacités énormes de stockage et de traitement et le cloud est aujourd’hui le moyen le plus capable de supporter ces volumétries et à moindre coût comparé à une solution classique on-premise.

#### 3.2.2 Le modèle de programmation MapReduce

Développé initialement par Google en 2003 pour analyser ses résultats de recherche, MapReduce a gagné en popularité grâce à sa capacité à diviser et traiter plusieurs téra-octets de données en parallèle et à obtenir ainsi des résultats plus rapides.

Cette technique de programmation simplifie le traitement d’ensembles de données en commençant par réduire les données à des séries de couples « clé/valeur », puis en procédant à des calculs sur les données possédant des clés similaires, afin de tout réduire à une valeur unique. Chaque « gros morceau » de données pouvait ainsi être traité en parallèle sur des centaines voire des milliers de machines peu coûteuses. Cette technique de traitement en parallèle sur des échelles massives a permis à Google de générer des résultats de recherche sur des volumes de données incroyablement plus grands qu’avant, et ce, en allant plus vite.

Le framework MapReduce est scindé en deux espaces fonctionnels :
- Map, une fonction qui répartit le travail à différents noeuds dans les grappes d’ordinateurs.
- Reduce, une fonction qui rassemble le travail et résume les résultats dans une valeur simple.

![djo](https://www.lebigdata.fr/wp-content/uploads/2017/08/mapreduce-fonctionnement.png)

Un des avantages primaires de Map Reduce est qu’il est  tolérant aux pannes. Comment fait-il ? Il « monitore » chaque noeud (node) du cluster régulièrement. Celui-ci est supposé renvoyer périodiquement un travail complet avec des mises à jour des « status ». Si un noeud reste silencieux plus que nécessaire, un master node le signale et réassigne le travail à d’autres noeuds du cluster.





#### 3.2.3. Le framework Hadoop

Juste après, il y a eu "Hadoop", un framework mis au point afin de mieux généraliser l'usage du stockage et traitement massivement parallèle de Map Reduce et de Google File System. 
Hadoop est composé de plusieurs éléments : un système de stockage (HDFS), un système de planification des traitements (YARN) et le framework de traitement (MapReduce).

Hadoop fractionne les fichiers en gros blocs et les distribue à travers les nœuds du cluster. Pour traiter les données, il transfère le code à chaque nœud et chaque nœud traite les données dont il dispose. Cela permet de traiter l'ensemble des données plus rapidement et plus efficacement que dans une architecture plus classique. 

Néanmoins, Hadoop seul ne peut pas venir à bout de toutes les problématiques du Big Data. Sa véritable valeur ajoutée réside dans les technologies qui forment ce qu'on appelle l’écosystème Hadoop. A ce jour, l’écosystème Hadoop est composé d’une centaines de technologies.

[heyo](https://www.data-transitionnumerique.com/wp-content/uploads/2019/09/carte-heuristique-%C3%A9cosyst%C3%A8me-Hadoop.png)



#### 3.2.4. Les bases de données NoSQL

Même avec Hadoop, il faut quand même un moyen de stocker et d’accéder aux données. C’est typiquement ce à quoi servent des NoSQL database telles que Mongo DB, CouchDG ou Cassandra, spécialisées dans le traitement des données non-structurées ou semi-structurées et distribuées à travers de multiples machines.




Pour réussir à exploiter les « Big Data » techniquement, l’idée n’est plus de centraliser le stockage et le traitement des données sur un serveur, mais de distribuer leur stockage et de paralléliser leur traitement sur plusieurs ordinateurs




## 4. Points importants à retenir
Au-delà des buzz words, l'analyse de données prend différentes formes et peut se réaliser à différents niveaux. On peut distinguer deux types d'analyses : 
- l'analyse de données au travers de logiciels de *Business Intelligence* qui permet de faire parler les données, le plus souvent déjà collectées et stockées dans l’entreprise.
- l’analytique Big Data qui nécessite l’intervention de spécialistes et la mise en œuvre d’une architecture informatique et d’outils complexes. 

https://www.atys-concept.com/blog-de-la-performance/articles-performance-industrielle/differences-entre-data-analytics-data-science-big-data/

## 5. Pour aller plus loin


peut-être mettre une blague ex : "si tu me crois pas qu'Hadoop est indispensable, cf https://www.decideo.fr/Les-6-competences-les-plus-recherchees-en-Big-Data_a10051.html"
