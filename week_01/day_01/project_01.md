# Petits programmes en Python

C'est parti, tu vas créer ton premier Jupyter Notebook et tes premiers programmes Python. Good luck my friend 🚀

## 1. Introduction
Pour ton premier jour de développeur Python 😎😎😎, rien de mieux que de te faire la main avec une série de programmes ... dont certains que tu as déjà faits en Ruby !

## 2. A toi de jouer !
La difficulté des exercices est croissante alors pas d'inquiétude si tu as du mal vers la fin du projet.

## 2.1. Rapide exerice de chauffe : manipulation de chaînes de caractères ⛓
- créer et afficher la variable `bonjour` qui contient une chaîne de caractères `hello world !`  
- afficher le premier caractère de `bonjour`  
- afficher le dernier caractère de `bonjour`  
- afficher les caractères de `bonjour` de la position 1 à la position 3  
- afficher les caractères de `bonjour` de la position 3 jusqu'à la fin  
- vérifier que `bonjour` commence par `hel`
- vérifier que `bonjour` se termine par `world !`  

## 2.2. Manipulation de fonctions 🔗
- créer une fonction qui prend en paramètre une variable intitulée `name` et qui affiche `Hello` suivi du prénom choisi  
- écrire un programme qui demande à l'utilisateur son prénom et lui retourne un message lui disant `Hello` suivi de son prénom  

## 2.3. Manipulation des conditions ↙️
- écrire un programme qui demande à l'utilisateur de saisir son âge et affiche `vous êtes majeur !` si l'âge est supérieur ou égal à 18 et `vous êtes mineur` sinon    
- écrire un programme qui demande à l'utilisateur de saisir un nombre et affiche `a est pair` si la valeur de `a` est paire et `a est impair` sinon  

___

👾👾 ALERTE 👾👾 

On arrête les exercices de chauffe ici. Retour à nos chers exercices de mardi dernier. 

Le fait de reprendre les mêmes programmes que mardi de la semaine dernière va t'aider à bien comprendre les différences entre Ruby et Python. D'ailleurs, on te déconseille de chercher à traduire ton programme Ruby en Python mais cherche plutôt, pour chaque programme, à reprendre la logique de décomposition que tu as apprise la fois dernière. Puis à voir comment tu écrirais le morceau en Python avec ce que tu as appris ce matin dans les ressources et ton nouvel oeil de Data Analyst en herbe !

___

## 2.4. Multiples de 3 et 5 🎲🎲

### 2.4.1. L'énoncé
Cédric Villani a besoin d'aide pour enfin décrocher le prix Nobel de Mathématiques. Il a besoin de résoudre le problème suivant :

>Si on liste tous les entiers naturels strictement inférieurs à 11 et qui sont multiples de 3 ou 5, on obtient 3, 5, 6, 9 et 10. La somme de ces nombres est égale à 33.
=> Trouve la somme des entiers naturels strictement inférieurs à 1000 et qui sont multiples de 3 ou 5.

Pour t'aider sur ce premier exercice, on va décomposer des étapes qui vont nous permettre de le résoudre.

### 2.4.2. Mise en oeuvre de l'approche analytique

Comme on l'a appris, pour résoudre ce problème compliqué, on va le découper en plein de petits problèmes simples. Ici, on doit écrire un programme qui prend un nombre, et qui ressort la somme des multiples de 3 ou 5 inférieurs à ce nombre.

Moi, quand je lis ça, je me dis "ok, mon programme va aller de zéro jusqu'à 1000 (par exemple) et à chaque chiffre va tester s'il est multiple de 3 ou 5. Si c'est le cas, il met le chiffre de côté, dans une boite, pour faire une somme à la fin. Si le chiffre n'est pas multiple, on l'oublie et on passe au suivant".

Hum, en écrivant ça sur papier, j'ai identifié 2 choses qui vont composer mon programme final :

"mon programme va aller de zéro jusqu'à 1000 (par exemple)" => Il va y avoir une boucle !
"à chaque chiffre [mon programme] va tester s'il est multiple de 3 ou 5" => voilà un problème simple et bien défini : être capable d'identifier si un nombre est multiple de 3 ou 5 !

Allez c'est parti, tu peux te lancer maintenant !
___

🙈🙈 SPOILER ALERT 🙈🙈

Tu peux voir à la suite deux solutions pour ce programme. Essaye d'abord de faire ta version avant de les regarder. 
On te montre la solution pour que tu voies qu'on n'est plus exactement dans la même démarche qu'avec Ruby (écrire des méthodes qu'on imbrique entre elles). A partir de maintenant et car précisément tu souhaites te spécialiser dans la donnée, tu peux aller au plus vite et au plus efficace. L'objectif dans l'analyse de données, c'est d'utiliser le code pour obtenir le bon résultat.

Une des solutions peut s'écrire ainsi : 
```
resultat = 0
for i in range(1, 1000):
    if i%3 == 0 or i%5 == 0:
        resultat += i
print(resultat)
```

Ou, en version plus condensée, ainsi :
```
> print(sum(i for i in range(1, 1000) if i%3 == 0 or i%5 == 0))
```

___


## 2.5. Cryptofolies 💳💳
Après ce petit tour de chauffe, voici un autre exercice sous forme d'initiation à la cybersécurité, avec un algorithme de chiffrement hyper secure (lol) : le chiffrement par décalage. En effet, la NSA a besoin de chiffrer ses e-mails et veut faire appel à toi pour implémenter cette méthode indéchiffrable par un enfant de 5 ans.

>En cryptographie, le chiffrement par décalage, aussi connu comme le chiffre de César ou le code de César, est une méthode de chiffrement très simple utilisée par Jules César dans ses correspondances secrètes.
Le texte chiffré s'obtient en remplaçant chaque lettre du texte clair original par une lettre à distance fixe, toujours du même côté, dans l'ordre de l'alphabet. Si jamais on dépasse la dernière lettre de l'alphabet, on continue à compter depuis le début. Par exemple avec un décalage de 3 vers la droite, A est remplacé par D, B devient E, W devient Z, X devient A, Y devient B, etc.
Il s'agit d'une permutation circulaire de l'alphabet. La longueur du décalage, 3 dans l'exemple évoqué, constitue la clé du chiffrement qu'il suffit de transmettre au destinataire — s'il sait déjà qu'il s'agit d'un chiffrement de César — pour que celui-ci puisse déchiffrer le message. Dans le cas de l'alphabet latin, le chiffre de César n'a que 26 clés possibles (plus la clé nulle, qui ne modifie pas le texte).

Ta mission : créer une méthode `caesar_cipher` qui prend en paramètres un string et une clé de chiffrement (nombre de lettres à décaler) pour en sortir le string modifié.

```
> caesar_cipher("What a string!", 5)
=> "Bmfy f xywnsl!"
```

## 2.6 Jean-Michel Trader 💸💸
Si tu es arrivé à bout des deux premiers exercices, bien joué ! On continue sur notre lancée.

Après la cybersécurité à la NSA, Lehman Brothers veut te débaucher pour faire de la finance. Hyper cool. Ils te demandent cette fois de coder un programme qui permet, à partir d'un array de prix, de connaître le meilleur jour d'achat et le meilleur jour de revente pour faire le maximum de bénéfices.

Si l'on considère la liste de prix suivant : `[17, 3, 6, 9, 15, 8, 6, 1, 10]`, la fonction `day_trader` doit renvoyer qu'il s'agit du deuxième jour à l'achat et du cinquième jour à la revente.

```
> day_trader([17, 3, 6, 9, 15, 8, 6, 1, 10])
=> [1,4]  # $15 - $3 == $12
```

## 2.7 Compter les mots

### 2.7.1. La première version
Après Lehman Brothers, Google a besoin de toi pour faire de la Data Science. Quelle star ! Écris une fonction intitulée `word_counter` qui prend en paramètres 2 éléments :
- le corpus, string dans lequel tu devras checker le nombre d'occurrences de différents strings
- la référence, une liste de mots (strings) qui seront recherchés dans le corpus
La fonction devra renvoyer le nombre d'occurrences de chaque mot de la référence dans le corpus sous la forme d'un dictionnaire. Ainsi :

```
> reference = ["below", "down", "go", "going", "horn", "how", "howdy", "it", "i", "low", "own", "part", "partner", "sit"]
> word_counter("below", reference)
=> {"below" : 1, "low" : 1}
> word_counter("Howdy partner, sit down! How's it going?", reference)
=> {"down" : 1, "how" : 2, "howdy" : 1, "go" : 1, "going" : 1, "it" : 2, "i" : 3, "own" : 1, "part" : 1, "partner" : 1, "sit" : 1}
```

### 2.7.2. Compter chez Shakespeare 🤓🤓

#### a) Les mots communs
Google veut savoir combien de fois l'on peut trouver dans l'œuvre intégrale de Shakespeare les mots suivants :

`reference = ["the", "of", "and", "to", "a", "in", "for", "is", "on", "that", "by", "this", "with", "i", "you", "it", "not", "or", "be", "are"]`
Crée un fichier shakespeare.txt qui reprend [le corpus intégral de l'oeuvre de l'écrivain anglais](https://ocw.mit.edu/ans7870/6/6.006/s08/lecturenotes/files/t8.shakespeare.txt). Ton programme appellera le fichier shakespeare.txt (indice : c'est plus facile s'ils sont dans le même dossier) pour s'en servir comme corpus, pour ensuite compter les occurrences du dictionnaire.

#### b) Les gros mots lol
Après les mots communs, Google est de plus en plus curieux. Ils voudraient savoir combien de gros mots sont contenus dans l'œuvre de Shakespeare, pour voir si l'auteur anglais était un coquin. Voici une liste de [gros mots](http://www.bannedwordlist.com/lists/swearWords.txt) au format .txt. Télécharge ce fichier, mets-le à côté de Shakespeare.txt. Trouve un moyen pour transformer cette liste de mots au format .txt en une array de string qui te servira de dictionnaire.



## 3. Rendu attendu
Un fichier .ipynb ou un fichier .py qui comprend l'ensemble des scripts demandés. 

