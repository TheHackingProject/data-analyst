# Série d'exercices en Python

## 1. Introduction
Pour ton premier jour de développeur Python 😎😎😎, rien de mieux que de te faire la main avec une suite d'exercices. 

## 2. A toi de jouer !
La difficulté des exercices est croissante alors pas d'inquiétude si tu as du mal vers la fin du projet.

### 2.1. Manipulation de chaînes de caractères
a) créer et afficher la variable `bonjour` qui contient une chaîne de caractères "hello world !"
b) afficher le premier caractère de `bonjour`
c) afficher le dernier caractère de `bonjour`
d) afficher les caractères de `bonjour` de la position 1 à la position 3
e) afficher les caractères de `bonjour` de la position 3 jusqu'à la fin
f) vérifier que `bonjour` commence par "hel"
g) vérifier que `bonjour` se termine par "world !"

### 2.2. Manipulation de listes
a) créer et afficher la liste `mylist` qui contient les éléments "am", "stram", "gram", "pic"
b) supprimer le deuxième élément de `mylist`
c) supprimer l'élément "am" de `mylist`
d) inverser les valeurs de `mylist`
e) afficher la taille de `mylist`
f) compter le nombre d'occurences de l'élément "am" de `mylist`

### 2.3. Manipulation de fonctions
a) créer une fonction qui prend en paramètre une variable intitulée `name` et qui affiche "Hello" suivi du prénom choisi
b) écrire un programme qui demande à l'utilisateur son prénom et lui retourne un message lui disant "Hello" suivi de son prénom

### 2.4. Manipulation des conditions
a) écrire un programme qui affiche "vous êtes majeur !" si votre âge est supérieur ou égal à 18 et "vous êtes mineur" sinon.
b) écrire un programme qui affiche "a est pair" si la valeur de la variable a est paire et "a est impair" sinon. 

### 2.5. Manipulation des boucles
a) écrire un programme qui demande à l'utilisateur un nombre puis affiche la table de multiplication du nombre choisi
b) écrire un programme qui demande à l'utilisateur un nombre d'étoiles (qui correspond au nombre d'étoiles de la ligne centrale du triangle) et puis qui affiche le triangle en question. 
Ex pour 4, le programme affichera : 
```
*
**
***
****
***
**
*
```

### 2.6. Manipulation des fichiers
a) écrire un programme qui ouvre un fichier texte, modifie les lignes affichées afin qu’elles commencent par une majuscule, puis affiche le contenu du fichier texte.
b) écrire une fonction NbrLignes qui a pour paramètre le nom d'un fichier (texte) et qui renvoie le nombre de lignes de ce fichier.

### 2.7. Exercice bonus
Soit un fichier typé intitulé concours.txt qui comporte les enregistrements relatifs aux candidats d’un concours. Chaque enregistrement est composé de : NCIN, NOM, PRENOM, AGE, DECISION : (type contenant les identificateurs suivants : admis, refusé, ajourné), et séparé par point virgule (;).

a) Définir la fonction saisir() qui permet de remplir les données relatives aux candidats dans le fichier concours.txt.
b) Définir la fonction admis() qui permet de créer le fichier admis.txt comportant les données relatives aux candidat admis.
c) Afin de sélectionner en priorité les candidats admis et âgés moins de 30 ans, créer la fonction attente() qui produira à partir du fichier admis.txt, un nouveau fichier intitulé attente.txt comportant les données relatives aux candidats admis et âgés de plus de 30 ans. Une ligne du fichier attente.txt comprend le NCIN, le NOM et PRENOM d’un candidat séparés par point virgule (;).
d) Définir la fonction statistiques(dec) qui permet de retourner le pourcentage des candidats pour la décision dec (admis, refusé et ajourné). Exemple : Le pourcentage des candidats admis = (Nombre des candidats admis / Nombre des candidats)x100
e) Définir la fonction supprimer() qui supprimera du fichier admis.txt les candidat âgés de plus de 30 ans

## 3. Rendu attendu
Un fichier .ipynb ou un fichier .py qui comprend l'ensemble des scripts demandés. 

