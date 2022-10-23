# Modéliser un système de BI

## 1. Introduction
Pour concevoir un bon entrepôt de données, il faut bien comprendre le business concerné. On pourrait faire appel au Data Analyst pour réaliser la modélisation de la base ou pour vérifier que rien n'a été oublié. Avant que ça soit ton tour, profite de ce projet pour t'exercer et devenir un as de la modélisation de systèmes d'info décisionnels 🦁

## 2. Le projet
### 2.1. Un système d'info décisionnel pour votre université 🎓🎓

Maintenant que vous savez cruncher les classements mondiaux des universités, vous avez pu transmettre un reporting sur l'évolution des performances de votre Université. Depuis, les équipes veulent améliorer cette performance. Et pour cela, le recteur de l'Université de Strasbourg vous a demandé de mettre en place un système qui lui permettra de prendre des décisions éclairées. 

En fait, il cherche à étudier les facteurs influant sur la réussite des candidats aux examens. Pour cela, on vous a chargé de construire un datawarehouse.

Il souhaite pouvoir répondre aux questions suivantes :
- Quel est le nombre de réussites aux examens par cours, pour l’année 2020 ?
- Quel est le nombre de réussites aux examens d’un cours obligatoire, pour l’année 2020 ?
- Quel est le nombre de réussites aux examens par genre (féminin, masculin), entre 2019 et 2020 ?
- Combien d’apprenants ayant un âge supérieur à 23 ans ont réussi leurs examens de « BI » ?
- Quel est le nombre de réussites aux examens pendant le semestre d’hiver 2020 ?

Pour cela, vous disposez des données suivantes :
Pour chaque examen passé, on connaît l’âge et le genre de l’apprenant, le nom du cours (les cours peuvent être regroupés en cours obligatoire et cours à option), la date de l’examen, la note obtenue et si l’examen est réussi ou non.

Pour l'instant, il vous demande de réfléchir à la conception du système. Vos missions sont les suivantes : 
- Donner la table principale de l’entrepôt ainsi que les tables dimensions relatives.
- Tracer le schéma en étoile dimensionnel.

### 2.2. Un système décisionnel pour étudier vos ventes 💰💰

Un ami à vous possède une entreprise qui revend du matériel informatique. Il vous demande de l'aider dans la gestion de ses ventes car il n'arrive pas vraiment à piloter son entreprise pour l'instant. 

La seule chose dont il dispose est d'un fichier Access qui contient sa base de données. 

Pour aider votre ami, vous allez utiliser le logiciel PowerBI Desktop(à télécharger [ici](https://powerbi.microsoft.com/fr-fr/downloads/)). Vous avez choisi PowerBI car il possède une vue dédié à la modélisation : il est donc le logiciel le plus pratique pour modéliser des données.

Vous importez votre fichier [sales.db](https://drive.google.com/file/d/13AZq7xX1JDkCsFjqUVqGTYJQmLkmAykc/view?usp=sharing), vous chargez toutes les tables. 

___

😩😩 Que faire si j'ai un Mac et que je ne peux pas télécharger Power BI Desktop ?

PowerBI Desktop est un logiciel de data très répandu sur le marché donc je te conseille de trouver un PC dans ton entourage (à un moment ou un autre, pas obligé que ce soit aujourd'hui) et de te familiariser à son interfance.

En attendant, si tu n'as vraiment pas de PC et que tu ne veux pas t'ennuyer avec des tentatives de virtualisation, tu peux réaliser le projet avec un ERD classique.
___

Pour en savoir plus sur le fonctionnement de PowerBI, vous pouvez regarder [cette vidéo](https://www.youtube.com/watch?v=PwyuzmL0jLU) ou [la doc de Microsoft](https://docs.microsoft.com/fr-fr/power-bi/fundamentals/desktop-getting-started), en particulier un tutoriel spécifique à la [conception de modèle de données](https://docs.microsoft.com/fr-fr/learn/modules/design-model-power-bi/).

Vos missions sont les suivantes : 
- Déterminer la table fait et les tables dimensions
- Créer un modèle relationnel en Etoile
- Créer un modèle relationnel en Flocon
- Ajouter deux nouvelles mesures : Total_Sales, Total_Costs
- Afficher les totaux des ventes par client et par date
- Visualiser la moyenne des ventes par catégorie de produit

## 3. Rendu attendu
- Un fichier .pdf contenant les schémas de l'exercice 1. 
- Un fichier .pbix contenant le schéma et les ajouts effectués sur vos tables de données pour l'exercice 2. 

