# Le Big Data
A quoi correspond techniquement cette révolution qu'on appelle communément "Big Data" et quelles sont ses conséquences sur l'analyse de données ?

## 1. Introduction
Tu viens de voir les deux familles d'outils indispensables à la Data Analyse : les langages de programmation et les bases de données. Il te reste à voir encore deux familles d'outils : les outils d'analyse (que tu verras lors de la troisième semaine de la formation) et les outils Big Data, qu'on va voir dans cette ressource. Les outils Big Data sont apparus récemment et sont souvent gérés par des développeurs vue leur complexité. Mais il est important pour toi de comprendre leur utilité et leur fonctionnement.

## 2. Historique et contexte
On peut dater l’acte de naissance du big data en 2001 avec l’invention de la règle des 3V (Volume, Vitesse et Variété). A l’époque, l’expression traduisait une rupture dans le volume des données à traiter. Jusqu’à la fin des années 90, les quantités de données restaient limitées. Puis, on a assisté à une explosion du volume de données avec l’essor de l’e-commerce, des réseaux sociaux, des terminaux mobiles et, plus récemment, de l’internet des objets (IoT). Face à cette avalanche de data, les modèles techniques existants ont montré leurs limites. La base de données parfaite n’existait plus. En fonction du souhait de privilégier la volumétrie, la vitesse ou les capacités de requêtage, on choisira une solution plutôt qu’une autre ou bien une combinaison d’outils.

Pour leurs propres besoins, les GAFAM ont dû créer des outils pour stocker et traiter à la volée des données à la fois nombreuses et versatiles, leur structuration changeant avec le temps. Facebook est ainsi à l’origine de Cassandra avant de se tourner vers HBase (NoSQL), Google de BigTable et GFS (ancêtre d’HDFS) et plus récemment de TensorFlow (machine learning). Les géants du web ont ensuite versé ces projets en open source, externalisant en quelque sorte leur R&D. Car à leurs yeux, l’or ce sont les données elles-mêmes, pas les technologies. 
 
Finalement, après avoir été longtemps un buzzword, "Big Data" a repris son sens initial : il fait référence à l'ensemble des technologies comme Hadoop, Spark, Kafka ou les bases de données NoSQL ... que tu vas découvrir aujourd'hui.

## 3. La ressource

L'univers du Big Data est complexe et pourrait faire l'objet de plusieurs semaines de formation. Mais dans ton cas de futur Data Analyst, une journée suffira car tu as surtout besoin d'avoir les bases pour savoir ensuite naviguer dans un projet Big Data. En fait, ce n'est pas toi qui devras créer les infrastructures Big Data, c'est le rôle du Data Engineer ou Data Architect. On va donc te livrer ici les notions les plus importantes.

https://matheo.uliege.be/bitstream/2268.2/2562/4/M%C3%A9moire%20Camille%20Marenne.pdf

https://inventiv-it.fr/big-data-devez-apprendre/

https://www.atys-concept.com/blog-de-la-performance/articles-performance-industrielle/differences-entre-data-analytics-data-science-big-data/

https://www.decideo.fr/Les-6-competences-les-plus-recherchees-en-Big-Data_a10051.html


### 3.1. Big data is not only big !

On pourrait penser que le Big Data (mégadonnées en français) se résume à des gros volumes de données. Sans parler de Big Data, il est aujourd’hui possible de stocker et d’exploiter de très gros volumes de données avec une grande variété de sources dans de grands entrepôts de données (les *Data Warehouses*). En effet, les technologies actuelles permettent de traiter des gros volumes de données selon les méthodes analytiques de Business Intelligence sans avoir recours au Big Data.

Si le Big Data concerne effectivement les gros volumes de données, une de ses spécificités est de s’intéresser aussi bien aux données structurées qu’aux données non structurées. Ce sont les données non structurées que les outils habituels d’analytique ne savent pas traiter. Une autre spécificité est le stockage des données, qui ne sont plus stockées dans des *Data Warehouses* mais dans des *Data Lakes*. Plus que les volumes, ce qui fait le Big Data est donc la nature des données, la manière dont on les stocke et les techniques d’analyse pratiquées avec des savoir-faire et des technologies propres.

En fait, au tout début, on a parlé des 3V : volume (grandes quantités), variété (différents types de données) et vélocité (rapidité de traitement). Mais ce que l’acronyme des 3V ne mettait pas en perspective, c’était cette innovation centrale qui veut que les données n’ont pas besoin d’être systématiquement « transformées » pour être analysées. Apparaissait donc une nouvelle approche, très différente de  celle que l’on connaissait à ce moment-là autour du data-mining et des data warehouses. La *data warehouse* classique était conçue pour un objectif donné. La donnée y était structurée et convertie à des formats précis, la donnée initiale étant forcément détruite dans le process. On parlait alors de process ETL : « extract, transform and load ». L’approche ETL est donc limitée à des analyses spécifiques pour des données spécifiques. 

⚠️⚠️ Ne croyez pas pour autant que les big data rendent les *data warehouses* obsolètes. Les systèmes de big data vous amènent à travailler avec des données non structurées, mais le type de résultats de requêtes que vous obtenez est loin de la sophistication des *data warehouses*. La *data warehouse* est conçue pour une analyse en profondeur de la donnée, et cela est rendu possible précisément parce que la donnée a été transformée et prévue dans un format spécifique.

Le big data vous permet d’analyser beaucoup plus de données de beaucoup plus de sources, mais avec une résolution moins fine. Pour schématiser, on peut dire que le big data est un monde impressionniste qui aura toujours besoin à ses côtés de l’hyper-réalisme des *data warehouses* 🎨 C’est pour cela que nous sommes condamnés à vivre à la fois avec les *data warehouses* traditionnelles  et ce nouveau style de traitement que sont les big data. Le big data ne consiste donc surtout pas à désapprendre ce que l’on a appris en se formant au *data warehouse*. Le data scientist n’a pas forcément vocation à prendre la place de l’ingénieur en informatique décisionnelle. Il faudra au contraire que l’entreprise se pose la question de comment faire en sorte que les deux s’enrichissent mutuellement. Et c'est aussi ces deux aspects que nous allons t'apprendre dans cette formation.

Pour synthétiser, le Big Data c'est non pas 3 mais 5Vs à la fois : 
- **Volume** -> des ensembles de données très volumineux 
- **Vitesse** ou **Vélocité** -> la vitesse à laquelle les données sont générées et à laquelle elles se déplacent
- **Variété** -> en fait, 80% des données dans le monde ne sont plus structurées et ne peuvent donc pas être facilement mises dans des tables ou des bases de données relationnelles - pense à des photos, des séquences vidéos ou des mises à jour de réseaux sociaux ⌚️📱
- **Véracité** -> les données sont devenues incertaines : il faut gérer la fiabilité de données intrinsèquement imprécises.
- **Valeur** -> finalement, tous ces volumes de données variées en mouvement rapide et de véracité différente doivent être transformés en valeur ! C'est là l'enjeu majeur du Big Data ⚖️⚖️



### 3.2. Différences entre Big Data et Business Intelligence ?


## 4. Points importants à retenir
Le processus d'analyse de données (ou *Data Analysis*) peut être décomposé en plusieurs phases. La première étape est la collecte de données. Les données sont en provenance d’une ou plusieurs sources. 

Avant de collecter les données, il est primordial de se fixer des objectifs précis pour ensuite faire le bon choix dans les sources de données à utiliser, ainsi que dans les méthodes à employer.


## 5. Pour aller plus loin
Un [article Medium](https://medium.com/@rachidj/collecter-les-donn%C3%A9es-rapidement-et-efficacement-df7dd78b1ac0) d'un data scientist sur la collecte de données. Tu verras comment on peut s'amuser quand on commence à maîtriser les techniques vues aujourd'hui.
Et tu peux regarder [cette vidéo](https://www.youtube.com/watch?v=HYNZixyYrW4) si ça t'intéresse de savoir comment scraper un profil Instagram 👹👹👹.
