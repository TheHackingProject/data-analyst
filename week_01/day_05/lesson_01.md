# Modéliser un data warehouse

## 1. Introduction
Tu as normalement bien compris la différence entre base de données et système de BI. Pour rappel, les entrepôts de données (ou data warehouses) sont un type spécial de base de données, spécifiquement construit dans le but d'exécuter des analyses. 

Alors que la plupart des bases de données sont des fichiers d'application OLTP (*Online Transactional Processing*), la plupart des entrepôts de données sont des fichiers OLAP (*Online Application Processing*). En raison de la structure des fichiers OLAP, il est beaucoup plus facile d'effectuer des requêtes et des analyses sur les données qu'ils contiennent, et n'importe qui peut interroger l'entrepôt de données avec un logiciel d'entrepôt de données ou une connaissance du SQL.

En revanche, alors qu'on s'attend à ce que les bases de données aient un temps de disponibilité de 99,99 %, les entrepôts de données n'ont généralement pas besoin d'avoir ce genre de temps de disponibilité. Les entrepôts de données ne sont pas constamment lus et écrits comme les bases de données le sont. La plupart des entrepôts de données se rafraîchissent avec les données des bases de données, souvent toutes les 24 heures environ.

On va maintenant voir comment on modélise ces deux types de systèmes. Dans cette ressource, focus sur les data warehouses 👉

## 2. Historique et contexte
**Le concept de data warehousing remonte à la fin des années 1980** lorsque les chercheurs d'IBM Barry Devlin et Paul Murphy ont développé le « business data warehouse ». Essentiellement, le concept d'entreposage de données visait à fournir un modèle architectural pour le flux de données allant des systèmes opérationnels aux environnements d'aide à la décision.

Le concept a tenté de répondre aux différents problèmes associés à ce flux, principalement les coûts élevés qui y sont associés. En l'absence d'une architecture d'entreposage de données, une énorme quantité de redondance était nécessaire pour prendre en charge plusieurs environnements d'aide à la décision. Le processus de collecte, de nettoyage et d'intégration des données provenant de diverses sources, généralement des systèmes opérationnels existants à long terme (souvent appelés systèmes hérités), était en partie répliqué pour chaque environnement.

En 1990, la société Red Brick Systems, fondée par Ralph Kimball, lance Red Brick Warehouse, le premier système de gestion de base de données spécialement conçu pour l'entreposage de données. En 1994, Bill Inmon définit le data warehouse comme "une collection de données orientées sujet, intégrées, non volatiles et historisées, organisées pour le support d’un processus d ’aide à la décision".

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




 Pour comprendre la modélisation d'un système décisionnel, regarde [cette vidéo](https://www.youtube.com/watch?v=7vPIo1QI0Ek). Dans un des deux projets du jour, tu vas devoir t'essayer à ce type de modélisation donc pense à bien prendre des notes pour retenir les concepts clés 📝

Tu trouveras [ici](https://stph.scenari-community.org/dwh/int/co/intUC032modObj.html) quelques lignes intéressantes sur les objectifs du modèle dimensionnel, ainsi qu'un exemple de modèle en étoile.




## 4. Points importants à retenir
 

## 5. Pour aller plus loin
- 
