# Modéliser un data warehouse

## 1. Introduction
Tu as normalement bien compris la différence entre base de données et système de BI. Pour rappel, les entrepôts de données (ou data warehouses) sont un type spécial de base de données, spécifiquement construit dans le but d'exécuter des analyses. 

Tu as vu dans le projet 1 comment on modélise une base de données classique. Dans cette ressource et le projet 2, focus sur les data warehouses 👉

📌 *Utilité pour le projet* : 5/5 pour le projet 2<br/>
📊 *Utilité pour être Data Analyst* : 3/5<br/>
💡 *Pourquoi cette ressource ?* : Cette ressource permet de comprendre le type de données auxquelles tu seras confronté dans les entreprises qui ont déjà un peu réfléchi à organiser un système d'info décisionnel. En tant que Data Analyst, tu pourras être amené à modéliser des entrepôts de données et tu devras dans tous les cas comprendre les choix de modélisation donc c'est une compétence très importante.

## 2. Historique et contexte
**Le concept de data warehousing remonte à la fin des années 1980** lorsque les chercheurs d'IBM Barry Devlin et Paul Murphy ont développé le « business data warehouse ». Essentiellement, le concept d'entreposage de données visait à fournir un modèle architectural pour le flux de données allant des systèmes opérationnels aux environnements d'aide à la décision.

Le concept a tenté de répondre aux différents problèmes associés à ce flux, principalement les coûts élevés qui y sont associés. 

En 1990, la société Red Brick Systems, fondée par Ralph Kimball, lance Red Brick Warehouse, le premier système de gestion de base de données spécialement conçu pour l'entreposage de données. En 1994, Bill Inmon définit le data warehouse comme "une collection de données orientées sujet, intégrées, non volatiles et historisées, organisées pour le support d’un processus d’aide à la décision".

Depuis, le marché de datawarehouse se veut en forte croissance : estimé à 21 milliards $ en 2020, il atteindra 34 milliards $ en 2025 selon les prévisions de *Datamation*.

## 3. La ressource

### 3.1. Comment construire un data warehouse ?

Une fois le besoin de recourir à un datawarehouse identifié et confirmé, le plus dur reste à faire : créer l'entrepôt de données. Voici les principales étapes pour y parvenir : 
- **Identifier le besoin auprès des utilisateurs**. L'implication du métier, des utilisateurs, est essentielle, puisque ce sont eux qui transforment les données en informations.
- **Modéliser les données**. Cf. chapitre suivant
- **Choisir l'architecture technique**. À l'instar de nombreuses autres infrastructures informatiques, le datawarehouse a pris le virage du cloud. Le datawarehouse en cloud a l'avantage d'être plus flexible, avec notamment un investissement initial et un processus de déploiement plus rapide qu'avec une architecture traditionnelle.
- **Implanter et déployer**. 


### 3.2. Modéliser les données

**On ne modélise pas un système décisionnel de la même manière qu'un système d'information opérationnel**.

Si l'on revient à la définition du data warehouse, on se rappelle de plusieurs éléments :
- **Les données sont orientées sujet**. Cela veut dire qu'elles sont structurées par thèmes (sujets majeurs de l'entreprise) et non suivant les processus fonctionnels.
- Par ailleurs, les données, issues de différentes applications de production, peuvent exister sous différentes formes. Pour le data warehouse, il faut les intégrer afin de les homogénéiser et de leur donner un sens unique, compréhensible par tous les utilisateurs. **Les données doivent posséder un codage et une description unique**.
- Enfin, les données d'un data warehouse sont **non-volatiles et historisées**. Dans un DW, il est nécessaire de conserver l’historique de la donnée. Le DW stocke donc l’historique des valeurs que la donnée aura prises au cours du temps. Un référentiel de temps est alors associé à la donnée afin d’être capable d’identifier une valeur particulière dans le temps.

Tout cela étant dit, nous allons te présenter les notions essentielles à la modélisation de système décisionnel : 
- **les faits sont ce sur quoi va porter l'analyse**. Ils mesurent l ’activité. Les faits sont toujours numériques. On aura des tables de faits sur les ventes (chiffre d'affaires net, quantités et montants commandés, quantités facturées, quantités retournées, volumes des ventes, etc.) par exemple ou sur les stocks (nombre d'exemplaires d'un produit en stock, niveau de remplissage du stock, taux de roulement d'une zone, etc.), ou peut-être sur les ressources humaines (performances des employés, nombre de demandes de congés, nombre de démissions, taux de roulement des employés, etc.)
- **les dimensions sont ce qu'on utilisera pour faire nos analyses**. Elles sont les critères selon lesquels on souhaite évaluer, quantifier les faits. Il peut y avoir une dimension client, une dimension produit, une dimension géographie (pour faire des analyses par secteur géographique), une dimension temps etc. Chaque table de dimension peut avoir et a en général **plusieurs attributs**.

Enfin, il y a  trois modélisations possibles pour organiser les données stockées dans un Data Warehouse : 
- **la modélisation en étoile**. Le modèle en étoile centre une table des faits et la relie à chaque table de dimension. 
- **la modélisation en flocon**. Le modèle en flocon reprend le modèle en étoile en décomposant les dimensions. 
- **la modélisation en constellation**. Le modèle en constellation rassemble plusieurs tables des faits qui utilisent les mêmes dimensions. 

Pour synthétiser tout cela, regarde [cette vidéo](https://www.youtube.com/watch?v=7vPIo1QI0Ek). Dans le projet 2, tu vas devoir t'essayer à ce type de modélisation donc essaye bien de retenir les concepts clés 📝

Tu trouveras [ici](https://stph.scenari-community.org/dwh/int/co/intUC032modObj.html) quelques lignes intéressantes sur les objectifs du modèle dimensionnel, ainsi qu'un exemple de modèle en étoile.


## 4. Points importants à retenir

La conception des modèles de données dans un DW est une étape importante qui nécessite une approche différente de celle utilisée lors de la conception de systèmes opérationnels. 

Si vous êtes confronté un jour à la lourde tâche de créer un data warehouse pour une entreprise, prenez du temps en amont pour comprendre l'ensemble des concepts liés à la conception de data warehouse. 


## 5. Pour aller plus loin
- Tu as envie de savoir comment ça se passe concrètement dans la réalité ? Lis [cet article](https://grim.developpez.com/cours/businessintelligence/concepts/conception-datawarehouse/) qui explique bien les interactions entre flocon, étoile et constellation.
- Tu peux aussi regarder des témoignages concrets de mise en place de data warehouse : [ici](https://fr.slideshare.net/hamzus/document-1295639592) le travail de Abderrahmane Filali pour la société SONELGAZ, opérateur énergétique en Algérie 
