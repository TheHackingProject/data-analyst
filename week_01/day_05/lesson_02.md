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

Pour synthétiser, le Big Data c'est une famille d'outils qui répondent non pas à 3 mais à 5Vs à la fois : 
- **Volume** -> des ensembles de données très volumineux 
- **Vitesse** ou **Vélocité** -> la vitesse à laquelle les données sont générées et à laquelle elles se déplacent
- **Variété** -> en fait, 80% des données dans le monde ne sont plus structurées et ne peuvent donc pas être facilement mises dans des tables ou des bases de données relationnelles - pense à des photos, des séquences vidéos ou des mises à jour de réseaux sociaux ⌚️📱
- **Véracité** -> les données sont devenues incertaines : il faut gérer la fiabilité de données intrinsèquement imprécises.
- **Valeur** -> finalement, tous ces volumes de données variées en mouvement rapide et de véracité différente doivent être transformés en valeur ! C'est là l'enjeu majeur du Big Data ⚖️⚖️

___


### 3.2. Les technos du Big Data

Trois grandes évolutions techniques ont permis la création et la croissance du Big Data :

- L’évolution du hardware de stockage capable de stocker de plus en plus de données, passant de serveurs physiques internes à l’entreprise à des serveurs dit “cloud” qui ont souvent une capacité de stockage bien supérieure.
- Le second point est une remise en cause du modèle matériel existant, celui où il fallait acheter le plus gros serveur possible. Aujourd’hui, la nouvelle évolution consiste à mettre en série des petits serveurs remplaçables et de créer un système distribué résistant aux pannes. Ce paradigme a été popularisé par Google au début des années 2000 et est à l’origine de la première version open source du premier framework Big Data sorti il y a 10 ans : Hadoop.
- La troisième révolution s’est amorcée en 2009 et est l’explosion des outils d’analyse, d’extraction et de traitement des données de manière non structurée que cela soit du NoSQL ou de nouveaux frameworks lié à l’écosystème de Hadoop.

Les bases de données classiques ne permettant plus de gérer de tels volumes, les grands acteurs du web (Facebook, Google, Yahoo, Linkedin, Twitter) ont créé des Framework Big Data permettant de gérer et traiter des grandes quantités de données à travers, par exemple, des lacs de données. Ces données sont ensuite “splittées” ou séparées pour être traitées parallèlement afin d’alléger les processus de calcul (dans l’ancien modèle, les traitements étaient fait les uns après les autres, dans un stack), puis réassemblées pour donner le résultat final. C’est cette technologie qui permet des vitesses de traitement aussi rapides sur de gros volumes de données. Au départ développée par Google, elle est maintenant sous le drapeau Apache et s’appelle Map Reduce.





#### 3.2.1 Modèle d'architecture







#### 3.2.1 MapReduce - algorithmes distribués

Au départ, il y a eu **MapReduce**, une méthode et une technologie de traitement massivement parallèle issues des laboratoires Google Corp  avec gestion de la tolérance aux pannes et système de gestion de fichiers spécifiques (Google File System). On parle là de traitement sur des milliers de machines réparties en grappes (clusters). 

#### 3.2.2 Hadoop

#### 3.2.3 Spark 



#### 3.2.4 Le cloud computing

#### 3.2.5 Les bases de données NoSQL




## 4. Points importants à retenir
Au-delà des buzz words, l'analyse de données prend différentes formes et peut se réaliser à différents niveaux. On peut distinguer deux types d'analyses : 
- l'analyse de données au travers de logiciels de *Business Intelligence* qui permet de faire parler les données, le plus souvent déjà collectées et stockées dans l’entreprise.
- l’analytique Big Data qui nécessite l’intervention de spécialistes et la mise en œuvre d’une architecture informatique et d’outils complexes. 


## 5. Pour aller plus loin


peut-être mettre une blague ex : "si tu me crois pas qu'Hadoop est indispensable, cf https://www.decideo.fr/Les-6-competences-les-plus-recherchees-en-Big-Data_a10051.html"
