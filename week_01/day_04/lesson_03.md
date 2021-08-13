# Les bases de données NoSQL

Ou comment faire quand le volume de données devient ingérable et que répondre à de simples requêtes prend des heures.

## 1. Introduction
Les exigences de développement d’applications moderne ont connu une profonde révolution ces 15 dernières années. Pour ce qui est de la gestion de gros volumes de données, les bases de données NoSQL ou non relationnelles semblent devenus indispensables 🗣🗣.

## 2. Historique et contexte
Le terme et le concept NoSQL furent inventés en 1998 par Carl Strozz, afin de désigner sa base de données relationnelle légère et open source. Ce concept a ensuite été adopté et **popularisé par les GAFAM** tels que Google, Facebook ou Amazon confrontés à d’immenses volumes de données. Les bases de données relationnelles étaient devenues trop lentes 🐢🐢.

Plutôt que de mettre à jour leur équipement informatique pour accroître les performances des SGBD, les géants de la technologie ont choisi de distribuer la charge sur de multiples serveurs hôtes. C’est la méthode dite du ”scaling out“. 

En l’an 2000, la base de données graphique Neo4j fut lancée. Ce fut ensuite le tour de la Google Bigtable, en 2004, puis CouchDB en 2005. L’histoire des bases de données NoSQL fut aussi marquée par Amazon Dynamo en 2007.

Puis, en 2008, Facebook rend open source la base de données non-relationnelle qu’elle utilise en interne : **Cassandra**. Cet outil devient la référence des databases NoSQL, et remet le terme NoSQL sous le feu des projecteurs en lui donnant son sens et sa popularité actuelle.

## 3. La ressource
Tu vas découvrir ici les caractéristiques principales des bases de données NoSQL pour que tu saches en parler et que tu ne sois pas désarmé si tu dois en rencontrer.

### 3.1. Définition de NoSQL

NoSQL correspond à « **not only SQL** » et c’est en effet ce que ce modèle de base de données veut être : non pas une contrepartie, mais bien un enrichissement et complément utile des bases de données SQL relationnelles traditionnelles. Pour être précis, les bases de données NoSQL dépassent les limites des systèmes relationnels et exploitent un modèle de base de données alternatif. Cela ne veut toutefois pas dire qu’aucun système SQL n’est utilisé. Il existe de nombreuses variantes combinées au sein desquelles les deux solutions peuvent être utilisées et qui restent toutefois englobées sous l’étiquette NoSQL 👐👐.

Les systèmes NoSQL sont souvent décrits comme des mémoires structurées de stockage de données, ce qui met en évidence leur différence significative avec les bases de données SQL : contrairement à ces dernières, **les bases de données NoSQL n’exploitent pas de schéma de tableau fixe dans lequel les données doivent être définies avant l’enregistrement**. Elles utilisent des méthodes plus flexibles leur permettant d’enregistrer facilement de nouveaux jeux de données et d’assurer leur mise à jour en continu au sein de l’application. Les solutions NoSQL sont également adaptées au traitement de données non structurées ou inconnues, ce qui serait totalement impossible avec une base de données relationnelle.

> Finalement, la définition exacte de la famille du NoSQL reste sujette à débat. Le terme se rattache autant à des caractéristiques techniques qu'à une génération historique de SGBD qui a émergé dans les années 2000. 

### 3.2. Les caractéristiques de NoSQL

- La principale particularité des bases de données NoSQL est qu’elles ne suivent pas le modèle relationnel et ne présentent pas de tableaux sous forme de colonnes fixes. Ces bases de données ne nécessitent pas de normalisation de données ou de mapping relationnel. Il est possible d’interagir sans utiliser de langages de requête complexe.

- Une autre particularité est l’absence ou la flexibilité des schémas. Il n’est pas nécessaire de définir de schéma des données, et les données de différentes structures peuvent donc être regroupées sur un même système.

- Les bases de données non relationnelles se distinguent aussi par une interface simple d’utilisation pour le stockage et la requête de données. Des APIs permettent de manipuler les données avec diverses méthodes de sélection. Les protocoles, basés sur le texte, reposent principalement sur HTTP REST avec JSON. On utilise en général un langage de requête NoSQL.

- La dernière caractéristique d’une base de données NoSQL est d’être distribuée. De multiples bases NoSQL peuvent être exécutées de façon distribuée, offrant des capacités d’auto-scaling et de fail-over. L'approche ACID des BDD relationnelles peut être délaissée au profit de l’élasticité et des performances 🔆🔆.

___

👾👾 ACID vs BASE 👾👾

Pour garantir l'intégrité et la sécurité des données, les bases de données relationnelles reposent sur le mécanisme transactionnel. Une transaction est un ensemble de modifications de la base qui forme un tout indivisible. Il faut effectuer ces modifications entièrement ou pas du tout, sous peine de laisser la base dans un état incohérent. On parle du principe ACID :
- Atomique : tout ou rien, une modification des données doit être réalisée dans son intégralité ou pas du tout.
- Cohérent : les données doivent toujours être cohérentes entre elles, même en cas d'erreur. Dans ce cas là, on effectuera un RollBack.
- Isolée : Pas d'interférences entre les transactions. Utilisation des verrous et des points de synchronisation.
- Durable : Lorsqu'une transaction s'est achevée, avec succès (Commit) ou en erreur (Rollback), les données doivent être dans un état stable et cohérent.

Cependant, avec le développement du Cloud computing et des systèmes distribués, de nouvelles bases de données ont été conçues pour répondre à des contraintes différentes.
Un nouveau concept opposé à ACID est apparu, le concept BASE :
- Basic Availability : le sytème doit toujours être accessible.
- Soft state : l'état de la base de données n'est pas garanti à un instant t.
- Eventually consistent : la cohérence des données à un instant t n'est pas primordiale.

En fait, la plupart des SGBD NoSQL relâchent les contraintes ACID, ou même ne proposent pas de gestion des transactions.

___


### 3.3. Les différents 



## 4. Points importants à retenir
Regarde [cette vidéo](https://youtu.be/0buKQHokLK8) qui synthétise très bien l'utilité des bases de données NoSQL.



## 5. Pour aller plus loin
Tu peux faire le cours OpenClassrooms [Maîtrisez les bases de données NoSQL](https://openclassrooms.com/fr/courses/4462426-maitrisez-les-bases-de-donnees-nosql) qui fait normalement partie de la formation *Data Architect*. Cela te donnera un aperçu de ce métier et t'aidera beaucoup pour réaliser un des projets de cet après-midi.



La raison principale de l'émergence et de l'adoption des SGBD NoSQL serait le développement des centres de données et la nécessité de posséder un paradigme de bases de données adapté à ce modèle d'infrastructure matérielle3. 

L'architecture machine en clusters induit une structure logicielle distribuée fonctionnant avec des agrégats répartis sur différents serveurs permettant des accès et modifications concurrentes mais imposant également de remettre en cause de nombreux fondements de l'architecture SGBD relationnelle traditionnelle, notamment les propriétés ACID.
