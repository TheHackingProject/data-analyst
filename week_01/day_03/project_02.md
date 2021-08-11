# 5 ans après, nouvelle enquête sur les Panama Papers

## 1. Introduction
Toujours comme ce matin pendant le cours OpenClassrooms ([à relire](https://openclassrooms.com/fr/courses/4449026-initiez-vous-a-lalgebre-relationnelle-avec-le-langage-sql/4539106-explorez-les-panama-papers) si tu as un peu oublié), tu es dans la peau journaliste d'investigation du *Fronde* qui doit ré-enquêter sur les Panama Papers. La revue pense qu'il faut re-sensibiliser le public aux découvertes faites en 2016.

A ce propos, le secrétaire de rédaction t'a retoqué hier ton article car selon lui, "il manque de données quantitatives et précises". Il te demande d'aller directement à la source de l'information, de reprendre toutes les données qui ont été rendues publiques à l'époque et de répondre à une longue liste de questions que se posent les lecteurs. Ces réponses pourront faire l'objet d'une infographie interactive, ce qui "plaira beaucoup plus aux lecteurs que ton histoire incompréhensible d'argent planqué".

## 2. Le projet

Voici la liste de questions auxquelles tu dois répondre : 

- Combien la base de données contient-elle de sociétés offshores différentes dont la source est "Panama Papers" ?
- Quel intermédiaire a créé le plus de sociétés offshores ? A-t-on son adresse et son pays ?
- Combien la base contient-elle de bénéficiaires avec un nom unique ? Quel est le bénéficiaire dont le nom revient le plus souvent ? 
- Donner la liste des juridictions avec le nombre d'entreprises offshores enregistrées sur chaque territoire, triée par ordre décroissant.
- Regrouper les sociétés offshores par statut, et trier la liste par ordre décroissant.
- Trouver la liste des bénéficiaires dont le nom contient "BNP" et ajouter, pour chaque bénéficiaire, le nom des sociétés offshores.
- Trouver la liste des sociétés dont la juridiction est "France", "Monaco" ou "Réunion".
- Trouver la liste des sociétés dont le pays de l'adresse et le pays de la juridiction sont différents.
- Trouver la liste des bénéficiaires qui ont des sociétés au même nom et enregistrée à la même date, trier la liste par odre décroissant.
- Donner la liste des intermédiaires qui ont aussi été bénéficiaires, en ajoutant leur nom de bénéficiaire et leur adresse.
- Donner le top 10 des bénéficiaires qui ont le plus d'identités différentes (similar name and address) et le nombre d'identités correspondants.
- Donner le top 10 des bénéficiaires qui ont le plus de parts toujours valides dans des entreprises offshores (dont la date de fin n'est pas encore passée).
- Question bonus : réussir à retrouver dans la base au moins 3 personnalités que tu connais ([indice](https://fr.wikipedia.org/wiki/Liste_des_personnes_cit%C3%A9es_dans_les_Panama_Papers)).

## 3. Rendu attendu
Un fichier .txt (ou .md) contenant les requêtes SQL qui permettent d'obtenir les infos demandées sur notre BDD.

## 4. Aller plus loin
Alors tu as aimé te prendre pour Sherlock Holmes pendant 3 heures ? Ca t'a plu de travailler sur de vraies données ? A l'époque, c'était assez novateur comme type de journalisme : c'est une des affaires qui a aidé les grandes rédactions à se tourner davantage vers la Tech. 
Si cela t'intéresse, voici 2-3 ressources qui t'en diront plus sur comment ça s'est passé dans la vie réelle :
- un journaliste du Monde qui raconte [les 9 mois passés à travailler sur cette base de données](https://www.lejdd.fr/Medias/Presse-ecrite/Comment-nous-avons-travaille-pendant-9-mois-sur-Panama-Papers-779799)
- 
