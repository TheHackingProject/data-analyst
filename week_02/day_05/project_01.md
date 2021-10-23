# Incollable sur l'éducation dans le monde

## 1. Introduction
Suite à ton stage à l'Université de Strasbourg, tu es recruté par la Banque Mondiale. Ils doivent sortir pour janvier prochain un gros rapport sur l'état de l'éducation dans le monde. Et à vrai dire, à part mettre toutes les données disponibles dans un fichier csv, pas grand chose n'a été fait 😨

## 2. Le projet

### 2.1. Etude de la qualité des données
Lors de ton premier point de prise de poste, on te prévient qu'on ne sait pas vraiment l'étendue de la tâche car personne ne s'est encore vraiment plongé dans le fameux fichier à 887 000 lignes 💩💩 En fait, l’organisme “EdStats All Indicator Query” de la Banque mondiale répertorie quasiment 4 000 indicateurs internationaux décrivant l’accès à l’éducation, l’obtention de diplômes et des informations relatives aux professeurs, aux dépenses liées à l’éducation... Les données sont disponibles sur [le site de la Banque Mondiale](https://datacatalog.worldbank.org/dataset/education-statistics).

Là où on a besoin de toi dans un premier temps, c'est d'évaluer la pertinence et l'exhaustivité de ces données (dans le temps, mais aussi géographiquement). On te confie que les fichiers sont trop complexes pour être évalués directement par un humain. Tous ceux avant toi s'y sont cassés les dents. Pour s'en sortir d'après ce qu'on dit, il faut ruser et faire un premier nettoyage de données. Ton premier objectif doit être de supprimer les lignes qui possèdent trop de valeurs manquantes.

A ce propos, la directrice du département Etudes te demande de lui envoyer un mail récapitulatif quand tu auras fait tes premières analyses et que tu seras en mesure de décrire ce que va pouvoir étudier le rapport. Elle aimerait que tu lui décrives les données dont on dispose et ce qu'on va pouvoir en tirer. Comme elle n'a pas beaucoup de temps, elle te demande que le mail fasse environ une vingtaine de lignes.

### 2.2. Début de l'analyse
Une fois que tu as réussi à estimer ce que sera l'analyse, tu te lances ! 

Les boucles entre nettoyage, visualisation et analyse peuvent commencer. Pour réussir à avancer, tes collègues te conseillent de réduire l'immense fichier à un fichier qui contient les données les plus utiles. Autrement dit, ils te préconisent de faire un grand nettoyage de données 🧽🧽 A la fin de ce nettoyage, tu auras un fichier beaucoup plus lisible qu'ils aimeraient bien obtenir. Ils te demandent d'ailleurs de leur envoyer ton fichier csv final. Cela leur permettra de regarder à leur tour les données intéressantes sur un support plus agréable.

Par ailleurs, en parallèle de ce nettoyage, tu vas devoir dégager des axes d'analyse qui te semblent intéressants. 
De nouveau, la directrice des Etudes te demande de lui envoyer un mail récapitulatif. Cette fois, elle aimerait que tu lui proposes 5 tendances qu'on retrouve dans le jeu de données. Ces 5 tendances pourraient constituer les 5 axes du rapport à publier en janvier. Ce qu'elle appelle tendance, c'est un parti pris sur une évolution constatée dans les données. Ex : la féminisation de l'éducation dans le monde (les femmes ont de plus en plus tendance à aller à l'école dans le monde). 

Rappel : l'objectif du rapport est de faire un état des lieux de la situation de l'éducation dans le monde et comment celle-ci devrait évoluer. Elle souhaiterait que tu illustres chaque tendance choisie par plusieurs chiffres évocateurs 🤓 et au moins, un graphique par tendance choisie.


## 3. Rendu attendu
- Un fichier .ipynb qui contient l'ensemble de tes analyses.
- Un fichier .doc ou.txt qui contient les deux mails récapitulatifs envoyés à ta directrice.
- Le fichier csv final que tu as envoyé à tes collègues.

PS1 : ne te fie pas à la taille de l'énoncé et ouvre plutôt d'abord les fichiers csv pour estimer le temps que va te prendre le projet ☠️

PS2 : si tu te motives à faire un fichier Jupyter nickel, tu pourras présenter ce notebook en disant "voilà c'est un exemple d'analyse que j'ai réalisée en toute autonomie. J'ai essayé d'aller à la source des données de l'éducation dans le monde pour me faire mon propre avis sur la question". Cela fait à la fois très débrouillard et très curieux, deux qualités qui sont très très recherchées en entreprise 😃


## 4. Auto-évaluation

Voilà tu as fini ton premier projet de Data Analyse de bout en bout, bravo 💥💥💥

Comme le projet n'est pas validant, on t'a préparé une grille d'auto-évaluation pour que tu puisses te situer par rapport à ce qui était attendu : 
- Est-ce qu'il y a fichier Jupyter qui alterne texte et code ? Et explique la démarche d'analyse qui a été réalisée ?
- Est-ce qu'il y a un fichier qui donne les deux mails envoyés à la directrice ? 
- Est-ce qu'il y a un fichier CSV qui compte moins de 800 000 lignes ?
- Est-ce que la personne a réussi à supprimer les lignes qui ne possèdent que des valeurs manquantes (ex : remplacer les guillemets vides par NaN puis supprimer les lignes avec NA) ?
- Est-ce que dans le premier mail adressé à la directrice, on apprend qu'on va pouvoir faire des études à différents échelons : au niveau mondial, au niveau des continents ou zones géographiques, au niveau de chaque pays ?
- Est-ce que dans le premier mail adressé à la directrice, on apprend qu'en réalité il n'y a pas 4 000 indicateurs mais quelques centaines ? Chaque indicateur étant divisé en sous-indicateurs, on peut en fait dire q'il y a moins d'un millier de thématiques qui est traité.
- Est-ce que dans le premier mail à la directrice, on a des exemples de sujets dont l'évolution peut être décrite à l'échelle mondiale ? 
- Est-ce que dans le premier mail à la directrice, on a des exemples de sujets dont l'évolution peut être décrite à l'échelle continentale/régionale ? 
- Est-ce que dans le premier mail à la directrice, on a des exemples de sujets dont l'évolution peut être décrite à l'échelle des pays ?
- Est-ce que dans le premier mail à la directrice, l'échelle de temps est évoquée ? C'est-à-dire qu'en fonction des indicateurs et des zones concernées, le nombre d'années concernées est très variable. 
- Est-ce que dans le premier mail à la directrice, on apprend que la base de données n'est pas très récente, cad que les données ne vont jamais au-delà de 2015 (ou alors cas très rares, il s'agit de prévisions) ?
- Est-ce que dans le deuxième mail à la directrice, on a 5 vraies tendances sur les données, cad 5 renseignements sur l'état de l'éducation dans le monde ? 
- Est-ce que ces 5 tendances sont étayées par suffisamment de chiffres, de façon à ce que les tendances ne semblent pas questionnables ?
- Est-ce que le fichier csv reçu peut permettre à des futurs collègues Data Analyst de réaliser leurs propres analyses sur le même sujet, mais en économisant plusieurs étapes de nettoyage ?



