# Data et BI : de quoi parle-t-on au juste ?

## 1. Introduction
Pendant 2 jours, on a laissé le suspense en mode "ba ouais Data Analyst, c'est évident comme job, tout le monde connaît". Mais en fait non, si on n'a pas tranché la question directement sur ce que l'intitulé de poste signifie, c'est qu'on n'a pas la réponse 😐😐

Maintenant que tu fais partie de ce monde, on peut te dire la vérité : personne n'est d'accord sur la définition du métier de **Data Analyst**. 

En gros, la Data est univers récent qui est en train de se construire. Il y a encore beaucoup de flou et surtout beaucoup de personnes qui ne savent pas vraiment de quoi elles parlent quand elles doivent s'aventurer dans l'univers data (recruteurs, chefs d'entreprise, chefs de projet etc.).

Malgré ce flou général, on va éclaircir tout cela aujourd'hui en te précisant tous les termes importants.

📌 *Utilité pour le projet* : uniquement pour le projet bonus<br/>
📊 *Utilité pour être Data Analyst* : 4/5<br/>
💡 *Pourquoi cette ressource ?* : C'est grâce à la maîtrise parfaite de ces concepts que tu passeras d'un simple exécutant Data (à qui on ne confiera pas la gestion du projet ni de tâche stratégique) à une personne que l'on consulte quand il s'agit de prendre des décisions importantes. Ce qu'il faut retenir ici c'est que si les mondes de l'informatique et de la data se sont construits en même temps à la fin des années 80, ils n'ont aujourd'hui plus rien à voir. Nous te conseillons de bien comprendre les différences entre les deux univers car tu seras amené à travailler avec tous les types de profils. 

## 2. Historique et contexte
La data et tous les métiers qu'elle englobe ont fait leur apparition dans le vocabulaire courant il n'y a qu'une dizaine d'années. Pourtant, ces métiers ne datent pas d'hier. Remontons un peu l'histoire pour mieux comprendre cela 📜

En 1962, dans *The future of Data Analysis*, John W. Tukey, pourtant un statisticien de renom — on lui doit notamment le terme de « bit » ou encore les diagrammes « boîte à moustache » —, dit préférer le terme de « data analysis » à celui de statistique. Pour lui cette **façon de tirer d’un grand nombre de données des tendances** relève plus d’une science empirique que des mathématiques pures, d’où cette différenciation qu’il est le premier à suggérer.

![texte](https://slideplayer.com/slide/14842537/90/images/3/In+Tukey%E2%80%99s+%281962%29+work+done+for+the+Army+Research+Office+titled%2C+The+Future+of+Data+Analysis%2C+John+Tukey+foreshadowed+the+emergence+of+Data+Science..jpg)

Quelques années plus tard, en 1970, comme vu hier, Edgar F. Codd inventait les premières bases de données relationnelles.
A la fin des années 1970 et dans les années 1980, l’informatisation des entreprises se concentrait sous **l’angle de la production** : saisies et calculs pour la comptabilité, la paie, les stocks, les factures… Des systèmes non conçus pour lancer des requêtes d’analyse.

C’est en 1989 qu’Howard Dresner (futur analyste de la société Gartner) reprend le terme de **Business intelligence** inventé par Luhn et en définit le cadre moderne : des concepts et méthodes pour améliorer la prise de décision grâce à des systèmes d’analyse de données factuelles. Dotée d’une structure et d’un vocabulaire commun, et portée par l’avènement des ordinateurs, l’informatique décisionnelle se normalise enfin.

A l’orée du XXIe siècle, la business intelligence est devenue rigoureuse et a conquis sa place dans le process de prise de décision. C'est son entrée dans l’ère du tout digital qui va la faire basculer dans une autre dimension. Depuis une vingtaine d'années et les débuts du Big Data, de nombreux acteurs de la technologie s'attachent à rajeunir la BI en la rebaptisant Data Discovery (Qliktech), Data Exploration (SAS), Analytics (Tableau, IBM, Oracle), Data Stories (Jolicharts), etc. Les terminologies et les acteurs sont nombreux. Ce qu'il faut retenir c'est qu'**on parle désormais de data pour désigner un ensemble très vaste de technologies qui permettent de traiter les données à très grande échelle**. 

## 3. La ressource

### 3.1. C'est quoi une "data" ?

**Une data c’est tout simplement une donnée stockée numériquement**. Plus précisément, c'est une information dématérialisée capable de circuler à travers un réseau de télécommunication ou informatique. Ce peut être une donnée que vous avez déposée inconsciemment en navigant sur Internet (ex : les cookies, les logs). Ce peut être une donnée que vous avez créée consciemment (ex : rédaction d'un mail). Ce peut être une donnée qui a été produite par une autre machine (ex : systèmes de mesure, IoT).

On comprend alors qu'il y a différents types de données. Lorsqu'une entreprise parle de "nos données", cela mériterait d'être précisé car on ne sait pas s'il s'agit des données personnelles des utilisateurs, des données commerciales et financières, des données liées aux opérations de l'entreprise, des données marketing etc.

Finalement, le mot "data" est très galvaudé. Il n'a plus vraiment de sens lorsqu'il n'est pas précisé par les personnes qui l'utilisent. 
D'ailleurs, tu verras qu'une grande part de ton rôle en tant qu'expert data sera d'aider les non-initiés à employer les bons termes. Tu seras donc amené à faire beaucoup de pédagogie.


### 3.2. Différencier informatique et informatique décisionnelle

**L’informatique décisionnelle est une branche de l’informatique** de plus en plus adoptée par les entreprises. Connue également sous l’appellation *Business Intelligence* (et souvent BI) en anglais, elle désigne l’ensemble des méthodes et outils informatiques utilisés généralement pour piloter une organisation. Le meilleur exemple de solution d’informatique décisionnelle est le tableau de bord. L’informatique décisionnelle utilise les données brutes de l’organisation comme matière première. A l’aide d’outils décisionnels (logiciels ou applications), on se connecte à des sources de données qui peuvent être très diverses : Excel, base de données SQL, ERP, etc…

En anglais la distinction est plus facile à comprendre car **on parle de *Computer Science* et de *Data science***. Finalement, en français, on pourrait traduire cela par l'informatique d'un côté et la science des données de l'autre. L'informatique concerne principalement le développement et l'ingénierie logicielle. Et par ailleurs, la science des données est un domaine interdisciplinaire qui a pour objectif d'extraire des connaissances et des idées de vastes jeux de données.

C'est important de faire la disctinction car les métiers ne sont pas les mêmes. Même si les développeurs et les experts de la donnée sont tous des profils techniques, ils ne vont pas forcément se comprendre. Par ex, un dev doit monter en compétences sur la data s'il veut comprendre comment cela marche. Idem pour un expert data : il doit se former au développement logiciel s'il veut être à l'aise dans cet univers.


### 3.3. Différencier système opérationnel et système décisionnel

Les systèmes « opérationnels » ou « de gestion », également appelés systèmes OLTP (on-line transaction processing), sont dédiés aux métiers de l'entreprise pour les assister dans leurs tâches de gestion quotidiennes et donc directement opérationnels.

Les systèmes « décisionnels », également appelés OLAP (on-line analytical processing), sont dédiés au management de l'entreprise pour l'aider au pilotage de l'activité. Ils offrent au décideur une vision transversale de l'entreprise.

**Dans un système OLTP, les données ne sont conservées que sur une courte période** ; elles sont détaillées, personnelles, identifiées (une facture appartient à une personne précise) et représentent généralement en volume quelques centaines de mégaoctets, voir quelques gigaoctets. 

En revanche, **dans un système OLAP, les données sont historisées et peuvent être agrégées**.


### 3.4. Une équipe data, ça sert à quoi ?

L’équipe Data permet de faciliter le développement d’une entreprise, quelle qu’elle soit. 

Elle aura plusieurs types de missions : 
- Assurer et permettre la fiabilité des données
- Doter les salariés d'outils efficaces pour analyser leurs données
- Anticiper les nouvelles tendances
- Détecter certaines problématiques possibles. 

Finalement, elle a un double rôle (dont la répartition va dépendre de chaque entreprise) : 
- un rôle de prestataire de services, pour lequel l'équipe data doit répondre aux besoins des équipes qui la sollicitent
- un rôle de conseiller stratégique, pour lequel l'équipe data peut influencer le business grâce à ses recommandations.

En fonction des organisations, c'est une équipe qui pourra fonctionner de manière autonome et centralisée ou bien de manière décentralisée (en dispatchant des expers Data dans les équipes qui en ont besoin).


## 4. Points importants à retenir

Autour de la data, on trouve beaucoup de confusions et de termes galvaudés. C'est bon signe car cela témoigne de l'intérêt grandissant du grand public et des médias pour ces thématiques. 

Mais cela impose aux experts data d'être très pédagogues et rigoureux dans leurs échanges. Rectifier les mauvaises interprétations et trouver des moyens de vulgariser est un exercice difficile mais indispensable à tout bon Data Analyst.


## 5. Pour aller plus loin
- [un article](https://www.saagie.com/fr/blog/comment-lequipe-data-sintegre-t-elle-au-sein-dune-organisation-existante/) sur "Comment bien intégrer son équipe data"
- des témoignages de start-ups qui décrivent le fonctionnement de leur équipe data : [Agicap](https://career.agicap.com/article/data/) et [Jobteaser](https://www.emil.school/articles/decryptage-de-lorganisation-de-lequipe-data-chez-jobteaser)
- [un article](https://www.upwarddata.fr/blog/creer-sa-strategie-data/) qui donne des conseils pour bien cadrer sa stratégie data
- toute source que vous pouvez trouver et qui vous permettra d'en savoir un peu plus sur le très vaste univers de la data ...
