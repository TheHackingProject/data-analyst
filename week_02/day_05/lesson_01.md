# Le processus général d'analyse de données

## 1. Introduction
Maintenant que l'on a décomposé les 4 étapes de l'analyse de données, on va les réunir ensemble pour voir dans la pratique comment une analyse de données peut se dérouler.

## 2. Historique et contexte
Les notions requises pour une analyse des données modernes commencent à être maîtrisées **au début du 19ème siècle**. Adolphe Quetelet, astronome et statisticien belge, exploite ce qu'il connaît de la loi gaussienne à l'anthropométrie pour examiner la dispersion autour de la moyenne (la variance) des mesures des tailles d'un groupe d'hommes. Puis, Francis Galton, parce qu'il veut étudier la taille des pères et des fils, s'intéresse à la variation conjointe (la covariance et la corrélation) de deux grandeurs, qui est à l'origine de ce qu'on appelle aujourd'hui la régression.

Marion Richardson et Frederic Kuder en 1933, cherchant à améliorer la qualité des vendeurs de « Procter & Gamble », utilisent ce qu'on appelle maintenant l'algorithme « Reciprocal averaging », bien connu en ACP.

Et plus tard, c'est l'avènement de l'ordinateur, et surtout du micro-ordinateur, qui a rendu possible les calculs complexes, les diagonalisations, les recherches de valeurs propres sur de grands tableaux de données, avec des délais d'obtention de résultats très courts par rapport à ce qui se faisait dans le passé.

## 3. La ressource
Face à un problème d'analyse de données, il est important de ne pas foncer tête baissée et de suivre différents process.

### 3.1. Les étapes d'un projet data 🤝 

Un projet data classique se déroule en 5 étapes : 
- **Formaliser le besoin**. Contrairement à un réflexe fréquent, la première phase d’un projet data n’est pas de choisir l’outil informatique, mais de définir les besoins business auxquels ce projet doit répondre. Voici quelques exemples de besoins : obtenir des données utilisateurs afin d'améliorer le tunnel d'inscription au service ; relancer les utilisateurs "qui veulent abandonner" pour améliorer le CA ; trouver des informations pour mieux cibler mes prospects etc. Ces besoins doivent être formalisés via des exigences fonctionnelles (ce que le produit doit permettre de faire) et non fonctionnelles (dans quelles conditions techniques le produit doit faire cela).
- **Identifier et collecter les données pertinentes**. La deuxième phase consiste à extraire les données qui vont permettre de répondre aux questions. Ces données sont la plupart du temps chiffrées et disponibles, mais souvent dispersées dans plusieurs outils informatiques qui ne communiquent pas toujours entre eux. La démarche typique pour constituer un jeu de données exploitables est d’identifier et de qualifier précisément les données sur lesquelles s’appuyer, à l’aide des divers métiers (finance, contrôle de gestion, commercial, marketing, production, logistique etc.) ; de localiser les données et d’y accéder dans les divers outils sources (ERP, back-office, outils de gestion de production ou de facturation, catalogue produits, fichier achats, base de données clients, informations du CRM, du call center, Web analytics, base de données RH…)… complétées au besoin par des données externes. Enfin, il faut réunir ces données dans un nombre limité de fichiers simples à exploiter.
- **Mobiliser les ressources nécessaires pour analyser les données**. C’est souvent le cœur du problème ! Par exemple, beaucoup de PME s’équipent avec des solutions surdimensionnées par rapport à leurs besoins alors qu’il suffit parfois de disposer d’une version récente d’Excel et d’une personne capable de concevoir des calculs un peu complexes pour mener à bien cette étape ! Il faut partir des questions business pour élaborer une méthode. Quelles données pour calculer quoi ? Quelles réponses en attendre ? Pour cela, il est indispensable de disposer d’une double expertise métier et data, et, au besoin, de se faire accompagner pour l’élaboration de la méthode de calcul. Enfin, il faut être patients ! L’équipe concernée doit dédier du temps à extraire les données, à spécifier les calculs et les résultats attendus, à les interpréter et… à les challenger !
- **Partager les données aux collaborateurs dans des formats adaptés**. Pour chaque profil, il faut penser au bon format de restitution des données et à la nature des informations à transmettre. Le rôle du demandeur est ici de challenger au maximum les résultats qui lui sont présentés : les résultats répondent-ils bien aux questions business posées ? Les réponses sont-elles synthétiques et clairement exprimées ? Les réponses sont-elles opérationnelles, actionnables ? Peut-on prendre des décisions sur la base des résultats présentés ?
- **Evaluer le retour sur investissement**. Souvent négligée, cette dernière étape est probablement la plus importante pour une PME. Il est indispensable pour le dirigeant de mettre en relation ce que le projet data coûte à l’entreprise et ce qu’il va lui rapporter dans le temps. Toute présentation de résultats d’analyse de données doit s’accompagner d’un récapitulatif des ressources engagées (investissements et charges) et des espérances de gains directement liés aux analyses produites par ces ressources.

### 3.2. Comment réaliser l'étape d'analyse des données 🤠

Pour certains problèmes, vous pourrez adopter **l'approche traditionnelle, qui est destinée à vérifier des hypothèses a priori** sur les relations entre variables. Par exemple, "Est-ce qu'il y a une corrélation positive entre l'âge d'une personne et sa prédisposition à un risque".

A l'inverse, dans beaucoup d'autres cas, vous serez amenés à faire ce qu'on appelle **l'analyse exploratoire des données (ou AED)**. Elle permet d'identifier les relations systématiques entre des variables, lorsqu'il n'existe aucune hypothèse a priori (ou des hypothèses incomplètes) quant à la nature de ces relations. C'est la posture qui va être privilégiée dans les projets de data science. 

En fait, **l’analyse exploratoire de données est un cycle itératif qui vous aide à comprendre vos données**. Lorsque vous faites un analyse exploratoire de données, vous :
- Générez des questions sur vos données
- Cherchez des réponses par visualisation, transformation, et/ou modélisation de vos données
- Utilisez ce que vous avez appris des données pour affiner vos questions ou générer de nouvelles questions.

L’analyse exploratoire de données n’est pas un processus formel avec une liste stricte de règles. Plus que tout, c’est une façon de penser. Lors des phases initiales de l’analyse exploratoire de données, vous devez vous sentir libre de creuser toutes les questions qui vous passent par la tête 🧐🧐 Certaines de ces idées vont se développer, d’autres vont être abandonnées. Tout au long de votre exploration, vous allez noter vos idées et vos découvertes qui méritent d’être approfondies ou communiquées aux autres.

> "Mieux vaut une réponse approximative à la bonne question, qui est souvent vague, que la réponse exacte à la mauvaise question, bien qu’elle soit précise.)” — John Tukey

**L’analyse exploratoire de données est, fondamentalement, un processus créatif**. Et comme tout processus créatif, la clé pour se poser de bonnes questions c’est de se poser un grand nombre de questions. Il est difficile de se poser des questions perspicaces au début de votre analyse parce que vous ne savez pas ce qu’il y a dans vos données. Et chaque question que vous allez vous poser va révéler un nouvel aspect de votre jeu de données et augmenter votre chance de découvrir quelque chose. Vous pouvez rapidement creuser dans la partie la plus intéressante de vos données —et développer des questions pertinentes— si vous suivez chaque question avec une nouvelle question basée sur ce que vous avez trouvez.


## 4. Points importants à retenir
L'analyse des données est un processus qui contient plusieurs étapes. Pour autant, c'est un processus itératif. Pensez à revenir souvent aux phases initiales, que ce soit préciser le besoin du client ou nettoyer les données. C'est cela qui rendra vos analyses complètes et intéressantes pour le client.

## 5. Pour aller plus loin
- Un article qui rappelle [les étapes d'un projet de data science](https://www.empirik.fr/2019/07/12/la-data-science-expliquee-a-ma-grand-mere-3-5-cycle-de-vie-dun-projet).
