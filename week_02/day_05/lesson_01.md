# Le processus général d'analyse de données

## 1. Introduction
Maintenant que l'on a décomposé les 4 étapes de l'analyse de données, on va les réunir ensemble pour voir dans la pratique comment une analyse de données peut se dérouler.

## 2. Historique et contexte
Les notions requises pour une analyse des données modernes commencent à être maîtrisées **au début du 19ème siècle**. Adolphe Quetelet, astronome et statisticien belge, exploite ce qu'il connaît de la loi gaussienne à l'anthropométrie pour examiner la dispersion autour de la moyenne (la variance) des mesures des tailles d'un groupe d'hommes. Puis, Francis Galton, parce qu'il veut étudier la taille des pères et des fils, s'intéresse à la variation conjointe (la covariance et la corrélation) de deux grandeurs, qui est à l'origine de ce qu'on appelle aujourd'hui la régression.

Marion Richardson et Frederic Kuder en 1933, cherchant à améliorer la qualité des vendeurs de « Procter & Gamble », utilisent ce qu'on appelle maintenant l'algorithme « Reciprocal averaging », bien connu en ACP.

Et plus tard, c'est l'avènement de l'ordinateur, et surtout du micro-ordinateur, qui a rendu possible les calculs complexes, les diagonalisations, les recherches de valeurs propres sur de grands tableaux de données, avec des délais d'obtention de résultats très courts par rapport à ce qui se faisait dans le passé.

## 3. La ressource
On peut distinguer 2 types de postures différentes face à un problème d'analyse de données. 

### 3.1. La posture d'analyste, ou "problem-solver" 🤝 
C'est le cas où on vous soumet un problème précis et votre rôle est de répondre au cahier des charges.

Votre projet data se déroule ici en 5 étapes : 
- **Formaliser le besoin**. Contrairement à un réflexe fréquent, la première phase d’un projet data n’est pas de choisir l’outil informatique, mais de définir les besoins business auxquels ce projet doit répondre. Voici quelques exemples de besoins : obtenir des données utilisateurs afin d'améliorer le tunnel d'inscription au service ; relancer les utilisateurs "qui veulent abandonner" pour améliorer le CA ; trouver des informations pour mieux cibler mes prospects etc. Ces besoins doivent être formalisés via des exigences fonctionnelles (ce que le produit doit permettre de faire) et non fonctionnelles (dans quelles conditions le produit doit faire cela).
- **Identifier et collecter les données pertinentes**. La deuxième phase consiste à extraire les données qui vont permettre de répondre aux questions. Ces données sont la plupart du temps chiffrées et disponibles, mais souvent dispersées dans plusieurs outils informatiques qui ne communiquent pas toujours entre eux. La démarche typique pour constituer un jeu de données exploitables est d’identifier et de qualifier précisément les données sur lesquelles s’appuyer, à l’aide des divers métiers (finance, contrôle de gestion, commercial, marketing, production, logistique…) ; de localiser les données et d’y accéder dans les divers outils sources (ERP, back-office, outils de gestion de production ou de facturation, catalogue produits, fichier achats, base de données clients, informations du CRM, du call center, Web analytics, base de données RH…)… complétées au besoin par des données externes. Enfin, il faut réunir ces données dans un nombre limité de fichiers simples à exploiter.
- **Mobiliser les ressources nécessaires**. C’est souvent le cœur du problème ! Par exemple, beaucoup de PME s’équipent avec des solutions surdimensionnées par rapport à leurs besoins alors qu’il suffit parfois de disposer d’une version récente d’Excel et d’une personne capable de concevoir des calculs un peu complexes pour mener à bien cette étape ! Il faut partir des questions business pour élaborer une méthode. Quelles données pour calculer quoi ? Quelles réponses en attendre ? Pour cela, il est indispensable de disposer d’une double expertise métier et data, et, au besoin, de se faire accompagner pour l’élaboration de la méthode de calcul. Enfin, il faut être patients ! L’équipe concernée doit dédier du temps à extraire les données, à spécifier les calculs et les résultats attendus, à les interpréter et… à les challenger !
- **Partager les données aux collaborateurs dans des formats adaptés**. Pour chaque profil, il faut penser au bon format de restitution des données et à la nature des informations à transmettre. Le rôle du demandeur est ici de challenger au maximum les résultats qui lui sont présentés : les résultats répondent-ils bien aux questions business posées ? Les réponses sont-elles synthétiques et clairement exprimées ? Les réponses sont-elles opérationnelles, actionnables ? Peut-on prendre des décisions sur la base des résultats présentés ?
- **Evaluer le retour sur investissement**. Souvent négligée, cette dernière étape est probablement la plus importante pour une PME. Il est indispensable pour le dirigeant de mettre en relation ce que le projet data coûte à l’entreprise et ce qu’il va lui rapporter dans le temps. Toute présentation de résultats d’analyse de données doit s’accompagner d’un récapitulatif des ressources engagées (investissements et charges) et des espérances de gains directement liés aux analyses produites par ces ressources.

### 3.2. La posture de "chercheur", ou analyse exploratoire des données 🤠
Par opposition à l'approche traditionnelle d'un besoin précis exprimé par un demandeur, destinée à vérifier des hypothèses a priori sur les relations entre variables (par exemple, "Est-ce qu'il y a une corrélation positive entre l'âge d'une personne et sa prédisposition à un risque"), **l'analyse exploratoire des données (AED) permet d'identifier les relations systématiques entre des variables, lorsqu'il n'existe aucune hypothèse a priori (ou des hypothèses incomplètes) quant à la nature de ces relations**. Lors d'une analyse exploratoire typique, le chercheur prend en compte et compare, à l'aide de diverses techniques, de nombreuses variables pour mettre en évidence des structures systématiques. C'est la posture qui va être privilégiée dans les projets de data science.

Votre projet data se déroule ici en 5 étapes : 

https://www.linkedin.com/pulse/les-7-%C3%A9tapes-dun-projet-data-science-j%C3%A9r%C3%A9my-bouzidi/?originalSubdomain=fr

https://thinkr.fr/tutoriels-gratuits-pour-apprendre-r/analyse-exploratoire-de-donnees/

https://www.empirik.fr/2019/07/12/la-data-science-expliquee-a-ma-grand-mere-3-5-cycle-de-vie-dun-projet

https://www.youtube.com/watch?v=KDzUozgLyCI





## 4. Points importants à retenir
La ressource en quelques points importants.

## 5. Pour aller plus loin
Quelques éléments en ligne pour aller plus loin
