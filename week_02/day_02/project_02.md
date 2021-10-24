# Analysons la qualité de l'air 💨💨

## 1. Introduction
Après ta mission chez l'opérateur de télécoms, tu as voulu changer d'univers et rejoindre le monde des ONGs. Tu as trouvé un poste chez [OpenAQ](https://openaq.org/#/), une organisation à but non lucratif qui permet aux communautés du monde entier de purifier leur air en harmonisant, en partageant et en utilisant des données ouvertes sur la qualité de l'air.

Ils te préviennent tout de suite que l'enjeu principal n'est pas forcément de collecter les données mais surtout de réussir à les harmoniser. C'est en mettant l'ensemble des données collectées au même format qu'on peut ensuite réaliser des comparaisons intéressantes.

## 2. Le projet

OpenAQ souhaiterait mettre en ligne sur son site un fichier qui permet de comparer des mesures de l'air récentes partout dans le monde. Pour cela, on te demande de nettoyer les données dont on dispose pour l'instant. 

Tu as reçu un mail qui te dit : "Télécharge [le jeu de données](https://public.opendatasoft.com/explore/dataset/openaq/information/?disjunctive.city&disjunctive.location&disjunctive.measurements_parameter) disponible sur la plateforme Opendatasoft. Et renvoie-moi d'ici la fin de la journée un fichier csv qui ne comporte aucune erreur, ni information non exploitable. Merci et bon courage."

Regarde sur l'onglet *Informations* du jeu de données, deux *disclaimers* sont énoncés : 
"- Some records contain encoding issues on specific characters; those issues are present in the raw API data and were not corrected.
- Some dates are set in the future: those issues also come from the original data and were not corrected."

Cela nous donne une idée de ce qu'il va falloir nettoyer en premier lieu !

## 3. Rendu attendu
 Un récapitulatif de ce que nous attendons du projet.
