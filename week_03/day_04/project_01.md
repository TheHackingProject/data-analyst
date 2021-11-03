# Crée la stack data de ton entreprise 

## 1. Introduction
Pour beaucoup d’entreprises, l’étape de création d’une infrastructure qui va permettre de faire de la data est cruciale.

Car on peut se le dire : suivre ses KPIs clés sur un Google Sheets rempli à la main, c’est bien mais c’est pas vraiment ce qu’on appelle faire des traitements data. Pour cela, pas besoin de spécialiste data. Et  pas de possibilité d’obtenir des analyses croisées et très précises. 

On peut dire qu’une entreprise commence à devenir data-driven lors qu’elle franchit au moins une de ses 2 étapes : recruter un spécialiste de la data ou mettre en place un data warehouse.
Souvent, ces 2 étapes sont concomitantes. Et c’est ce qui se passe dans le cas de ce projet !

## 2. Le projet

### 2.1. Contexte de l'entreprise Squadeasy

Tu viens d’être recruté par l’entreprise [Squadeasy](https://www.squadeasy.com/) en tant que première personne de l’équipe Data. C’est le CEO qui a géré ton recrutement : il t’a expliqué que la boîte étant en pleine croissance, ils ont besoin de quelqu’un pour structurer leur data. Mais il a aussi tout de suite précisé qu’il n’y a pour l’instant aucune compétence data chez les salariés de l’entreprise. C'est d'ailleurs une experte freelance qui t'a fait passer un entretien technique pour vérifier tes compétences.

Maintenant que tu as été recruté, les dirigeants te font entièrement confiance sur les outils à mettre en place et les process à créer, même s'ils savent que tu es encore junior dans la data et que tu devras probablement te faire accompagner à certaines étapes (par des freelances par exemple). Ce qui les intéresse en premier lieu c’est que tu sois capable de leur fournir rapidement des informations intéressantes sur leurs clients (Quel type d'organisation est le plus intéressé ? Y-a-t-il des régions à cibler en particulier ? Quel poste dans l'entreprise répond le plus favorablement à la prospection ? etc.) et sur les comportements de leurs utilisateurs (Quelles features sont le plus appréciées ? Quelles thématiques ont le plus de succès ? Qu'est-ce qui crée de l'engagement chez les utilisateurs ? etc.). 

Voici les informations qu’il te donne lors de ton premier jour : le business de Squadeasy c’est de vendre des challenges connectés à des clients B2B. Un challenge connecté c’est une succession d’étapes à réaliser via une application mobile. Pour les participants, le but est de récolter le plus de points car les points récoltés par toute l’équipe seront transformés en dons reversés à des associations partenaires. On peut obtenir des points en cumulant le plus de pas (via un podomètre qui est connecté à l’appli), en répondant à des quizzs et en réalisant des défis. 
Les challenges peuvent être inter-entreprises (plusieurs entreprises s’affrontent) ou bien intra-entreprise (seuls les salariés de l’entreprise participent au jeu dans ce cas).
Aujourd’hui, l’entreprise emploie 20 salariés à temps plein.

Il y a déjà plusieurs sources de données dans l'entreprise (dans l'ordre d'importance) : 
- les données de la base de données de production (Firestore) qui fait tourner l'application au quotidien. Cette base de données enregistre les actions que réalisent les utilisateurs (ex : faire des pas, valider un quizz, changer d'étape)
- les données de Google Analytics qui collectent des données sur 2 choses : le site vitrine et sur l'application. Ce sont ici plutôt des données comportementales (nombre de pages vues, nombre de connexions etc.)
- les données de Hubspot, qui est l'outil CRM de l'entreprise. Il centralise l'ensemble des informations sur les actions commerciales réalisées par l'équipe Sales.
- le reporting de closing clients réalisé sur un Google Sheets et mis à jour par les cofondateurs chaque semaine
- les données collectés par l'ensemble des outils utilisés par les équipes (Mailchimp, Instragam, Facebook, Linkedin, Google Ads etc.).
- les données présents sur le Drive de l'entreprise et accessibles à tous.

### 2.2. Ta mission

Face à toutes ses sources de données, tu es un peu perdu lors de tes premiers jours. Comme un bon élève, tu cherches à réaliser des premières analyses. L'équipe technique t'a envoyé des extracts de la base de données de production mais comme cette base est du NoSQL, tu as beaucoup de mal à tirer des informations utiles de ces extracts. Par ailleurs, leur historique est limité à 30 jours sur cette base de données de production. 

Côté clients, tu as réçu le fameux Google Sheets qui est mis à jour régulièrement par les cofondateurs mais celui-ci doit être complété à la main pour chaque contrat déjà signé. Pour l'instant, tu ne peux pas faire d'analyse poussée car les données n'avaient pas été récoltées dans ce but-là. Tu dois toi-même créer un fichier parallèle et ajouter à la main, pour chaque client, le secteur de l'entreprise, le poste de la personne qui a signé le deal, sa région d'implantation etc. Tu commences mais tu sens que cela va te prendre un temps fou et que ça ne sera même pas réutilisable car non automatisé.

Tu te rappelles alors de tes cours de Data Analyse quand tu apprenais que les entreprises devaient créer un système de BI, parallèle au système de production. Et le mot data warehouse te revient immédiatement en tête 💡 Lors de la cinquième semaine de ton contrat, tu écris alors un mail aux 2 cofondateurs pour leur demander s'ils pourraient débloquer un budget pour que tu mettes en place un datawarehouse pour les besoins data de l'entreprise.

Ils te répondent que tout est envisageable mais que d'abord, tu dois leur expliquer clairement ton besoin au travers d'un cahier des charges. Comment tu vas t'y prendre, quelles seront les étapes du projet, combien de temps cela va durer et quelles ressources humaines et techniques vont être mobilisée. Et surtout quel sera le ROI de ton projet. Autrement dit, estimer le coût vs le bénéfice. 

Tu apprends entre temps que le CTO de l'entreprise est pour l'instant contre ton projet. Selon lui, la base de données actuelle est largement suffisante, pas la peine de créer autre chose. Tu devras donc le convaincre également du besoin de mettre en place un datawarehouse.

## 3. Rendu attendu
- Un cahier des charges qui précise ton besoin data actuel. Concernant le format (présentation PPT, template long, document word), tu es libre de choisir ce que tu penses le plus adéquat pour détailler tes arguments. 

PS : par rapport au temps dont tu disposes (une journée) et à la non maturité technique de tes interlocuteurs, nous te recommandons de faire une présentation PPT très visuelle et claire. En une quinzaine de slides et 15 minutes de présentation, tu devrais être capable de réussir à les convaincre du bien fondé de ton projet. Pour cela surtout, montre leur que tu as bien étudié le projet (en cherchant sur Internet toutes les infos disponibles), que tu as benchmarké des outils. Que tu as identifié les phases du projet. Et que tu peux estimer le coût total (en incluant par exemple des besoins de freelance).
