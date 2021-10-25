# Analysons la qualité de l'air 💨💨

## 1. Introduction
Après ta mission chez l'opérateur de télécoms, tu as voulu changer d'univers et rejoindre le monde des ONGs. Tu as trouvé un poste chez [OpenAQ](https://openaq.org/#/), une organisation à but non lucratif qui permet aux communautés du monde entier de purifier leur air en harmonisant, en partageant et en utilisant des données ouvertes sur la qualité de l'air.

Ils te préviennent tout de suite que l'enjeu principal n'est pas forcément de collecter les données mais surtout de réussir à les harmoniser. C'est en mettant l'ensemble des données collectées au même format qu'on peut ensuite réaliser des comparaisons intéressantes.

## 2. Le projet

OpenAQ souhaiterait mettre en ligne sur son site un fichier qui permet de comparer des mesures de l'air récentes, relevées sur un jour donné, partout dans le monde. Pour cela, on te demande de nettoyer les données dont on dispose pour l'instant. 

Tu as reçu un mail de ton manager qui te dit : "Télécharge [le jeu de données](https://public.opendatasoft.com/explore/dataset/openaq/information/?disjunctive.city&disjunctive.location&disjunctive.measurements_parameter) disponible sur la plateforme Opendatasoft. Et renvoie-moi d'ici la fin de la journée un fichier csv qui ne comporte aucune erreur, ni information non exploitable. Merci et bon courage."

Comme le message est un peu lapidaire, on va te donner quelques informations supplémentaires. Regarde sur l'onglet *Informations* du jeu de données, deux *disclaimers* sont énoncés : 
- Some records contain encoding issues on specific characters; those issues are present in the raw API data and were not corrected.
- Some dates are set in the future: those issues also come from the original data and were not corrected.

Cela te donne une idée de ce qu'il va falloir nettoyer en premier lieu !

Si tu souhaites plus de précision dans les consignes, voici les étapes qu'on te conseille de suivre pour arriver à tes fins : 
- Supprimer les données qui ne concernent pas le jour du 06-08-2021
- Supprimer les données qui sont illisibles et pour lesquelles on ne comprend pas la ville concernée. 
- Pour chaque polluant, vérifier qu'on n'a qu'une seule mesure utilisée. Autrement, supprimer les données qui correspondent à la mesure minoritaire ou moins cohérente.
- Regarder s'il y a des valeurs aberrantes ou des problèmes par rapport à notre objectif final (pouvoir comparer des mesures sur un maximum de pays) et noter ces aspects dans un fichier texte.

## 3. Rendu attendu
- Le fichier csv qui ne comporte aucune erreur ni information non exploitable. 
- Un fichier txt qui précise les limitres du fichier final
