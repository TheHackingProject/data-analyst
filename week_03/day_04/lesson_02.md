# Les livrables à produire

## 1. Introduction
Le Data Analyst participe à l'amélioration de la stack data de son entreprise, bien souvent en réalisant des études spécifiques. Nous verrons ici quels livrables tu devras être en mesure de produire pour documenter les process data de ton entreprise 📂📂

## 2. Définitions
**Documenter ses données, c’est donner les informations nécessaires pour les trouver, les lire, les comprendre et les réutiliser** : sources, modalités de production, de collecte et de traitement, logiciel utilisé, format du fichier, unités de mesure, attribution de mots-clés thématiques descriptifs, localisation géographique, date d’acquisition, identifiant … Ces informations sont aussi appelées métadonnées, ce qui signifie « données décrivant des données ».

Chaque fois qu’un aspect est important, tu dois le documenter. Si toute ton équipe décide de partir vivre au Brésil 😎, tu dois espérer qu’ils t'ont légué une documentation claire et complète sur les procédures de sécurité et de sauvegarde : tu pourras ainsi poursuivre les activités sans difficultés et sans perdre de temps. En l’absence d’une documentation complète et détaillée, la connaissance des systèmes et solutions est limitée à leurs propriétaires.

## 3. La ressource

### 3.1. Modéliser la base de données
Pour documenter la data d'une entreprise, il est courant qu'on te demande de modéliser la base de données. Celle-ci est déjà opérationnelle mais personne n'a encore réalisé de schéma pour expliquer comment elle fonctionne. Rappelle-toi, on avait vu cela lors du jeudi de la première semaine. 

On ne va pas trop se relancer là-dedans mais sache que : 
- une base de donnés relationnelles se modélise grâce à un diagramme Entité-Relation (cf. le [tutoriel de Grafikart](https://grafikart.fr/tutoriels/modeliser-base-de-donnee-75) si tu veux en savoir plus)
- les bases de données NoSQL étant très récentes, aujourd'hui il n'existe pas réellement de méthodes permettant de les modéliser. Une solution pour modéliser une base de données document est d'écrire du JSON. 

### 3.2. Cartographier les données
Une représentation visuelle de l'architecture de la donnée, de la collecte à son exploitation, est très utile. Elle permet d’identifier les intégrations existantes ou manquantes et de définir une stratégie globale. En effet, les sources sont multiples et il est probable que vous soyez confrontés à des silos. Par exemple, une start up peut se retrouver avec de la donnée concernant ses utilisateurs dans Google Analytics, Hubspot, Wootric pour le NPS et JIRA. Avant de regrouper, **une vue d’ensemble est nécessaire**.

Ce matin, si tu as bien lu le super article que je t'ai conseillé, tu as dû voir passer un exemple déjà de cartographie des données. Je te le remets ici au cas où 😴

![djay](https://www.followtribes.io/wp-content/uploads/2021/03/image-1.png)

En fait, cartographier l’organisation des données d’une entreprise consiste à faire deux choses :
- **Recenser tous les lieux de stockage** des données clients : bases, outils, applications … Il s’agit de répondre à la question : « Où y a-t-il de la donnée ? »
- **Recenser tous les flux entre ces lieux de stockage**. Les flux – qui peuvent être entrants ou sortants – permettent à la donnée de circuler d’un système à l’autre. La question est donc : « Comment circule la donnée entre les systèmes ? ».

Le travail de cartographie peut sembler relativement simple à première vue, mais dans la pratique les silos de données ne sont pas toujours aussi apparents qu’on pourrait le penser. Ils peuvent se trouver dans des endroits non évidents comme : dans des smartphones, sur des fiches papiers, voire dans la tête de vos collaborateurs.

Enfin, il n'y a pas de modèle de cartographie type, l'important étant de reproduire visuellement la réalité. Voici un dernier exemple de cartographie d'un SI qui semble bien complexe : 

![ami](https://www.custup.com/wp-content/webp-express/webp-images/uploads/2019/01/cartographie-donnees.png.webp)


### 3.3. Faire un audit
Un audit de la qualité des données permet de n'exploiter que les données qui ont du sens. Or, sélectionner les données à exploiter peut être un choix cornélien face à une telle profusion !

Sur les sites e-commerce par exemple, on comptabilise chaque jour des milliers de pages vues. Ce n'est pas pertinent de tout stocker pour chercher ensuite à tout exploiter. 

Pour faire un audit des données de façon intelligente, une solution est de reprendre les 5V que l'on a étudiés avec le Big Data : 
- **Le volume**. Quelle masse de données est concernée ?
- **La véracité** de la donnée. Par exemple, des transactions d’achat doivent être corrigées à cause de régularisations ou des retours de produits.
- **La vitesse** à laquelle la donnée circule. Ce qui pose encore une fois la question de la véracité : plus la donnée circule vite, plus elle risque d'être erronnée.
- **La variété** de la donnée parce qu’elle provient de systèmes totalement hétérogènes et il faut être capable d'aller la capter partout. C'est un vrai défi.
- **La valeur** : c’est tout l’enjeu de la donnée ! Elle doit remplir les objectifs de l'entreprise et être créatrice de valeur pour la marque et pour les clients.

Finalement, la question à laquelle doit répondre un audit est : quelles données je peux et je souhaite exploiter ? Pour quels coûts/bénéfices ? 

### 3.4. Faire un benchmark
Enfin, comme on l'a vu ce matin, l'analyse des données d'une entreprise se fait souvent à travers un empilement d'outils. Pour faire les bons choix d'outils, une méthode est imparable : **le benchmark**. Ce mot est souvent employé à tort et à travers mais il désigne en réalité "étude comparative". 

Il consiste à mesurer les performances d'une entreprise par rapport à celles de ses concurrents. Cette approche méthodologique incontournable permet de mieux atteindre vos objectifs.

Par exemple, si tu dois trouver un outil de visualisation pour ton entreprise, on te demandera probablement (ou tu pourras réaliser par toi-même) cette fameuse étude comparative. Ce travail consistera à étudier les opportunités de souscrire à un nouveau logiciel, à présenter les différents logiciels et enfin à faire des recommandations sur la solution qui paraît la mieux adaptée aux besoins de l'entreprise.

## 4. Points importants à retenir
En tant que Data Analyst, tu seras souvent amené à réfléchir sur comment améliorer la performance data de l'entreprise. Contrairement à ce qu'on pourrait penser, ce n'est pas une tâche méditative 🙏 Au contraire, il s'agit plutôt de produire des livrables sur la base desquels les décisions pourront ensuite être prises. C'est vraiment ta production (schéma, mapping, audit, benchmark etc.) qui permettra aux décideurs d'y voir plus clair sur les datas et d'éventuellement accepter des changements dans la stratégie.

## 5. Pour aller plus loin
On reprendra ces concepts la semaine prochaine, quand on étudiera l'intérêt du Data Management. 

