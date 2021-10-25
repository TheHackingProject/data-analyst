# Analysons des factures d'énergie 🌠🌠

## 1. Introduction
Un des cas d'usage fréquents de l'analyse de données est ce qu'on appelle la détection d'anomalies. Il s'agit en fait de checker, à travers des gros jeux de donnnées, s'il n'y a pas des éléments de notre chaîne de production qui dysfonctionnent. 

Le contrôle de la facturation est un cas d'école intéressant. Comme la consommation d'énergie n'est pas facilement interprétable par un humain, il peut être utile de vérifier les factures émises par les fournisseurs d'énergie afin de repérer d'éventuelles erreurs et, le cas échéant, économiser de l'argent 💰💰


## 2. Le projet

### 2.1. La mission
L'opérateur de télécommunications national en Slovaquie fait appel à vous pour contrôler ses factures d'électricité. Il vous explique que les réseaux mobiles (et plus directement, les antennes) sont très consommateurs d'énergie. C'est pourquoi, en tant qu'opérateur, il doit dépenser chaque année de très fortes sommes dans l'électricité. 

En revanche, il a le sentiment (et certains de ses salariés lui ont confirmé cela) qu'il y a des erreurs dans les factures et que certaines sommes ne sont pas justifiées. Mais il y a un nombre de factures colossal et son service de comptabilité n'a pas les compétences nécessaires pour traiter autant de données.

Il vous demande donc de récupérer [ici](https://drive.google.com/file/d/1Xpfmecb4PmW-CEqFuiLdelZx4jWxZTD-/view?usp=sharing) le fichier qui regroupe toutes les factures pour l'ensemble des antennes de l'opérateur. Et de le nettoyer pour que les équipes terrain puissent l'utiliser régulièrement, dès qu'un besoin de vérification sera remonté.

**Finalement, ton objectif est de transformer le fichier qu'a récupéré la direction en un fichier exploitable**. Pour les équipes de comptabilité, "exploitable" signifie qu'ils n'ont qu'à rechercher le nom d'une antenne en particulier, et ils peuvent obtenir l'historique sa consommation d'énergie, pour vérifier s'il y a des anomalies. Pour que cet historique soit intéressant, ils ont besoin d'avoir la consommation moyenne journalière (comme ça par ex, ils peuvent comparer un mois de Février qui fait 28 jours avec un mois de janvier qui fait 31 jours, sans se dire que la diminution vient de la différence de jours dans un mois).


### 2.2. Les tâches

1) Le nom d'une antenne a un format bien précis : il est toujours composé de 4 chiffres et deux lettres. On te demande de retirer tout autre caractère de la colonne "SITE_NAME".
2) On te demande de supprimer la colonne "INVOICE_NAME" qui n'apporte rien aux équipes.
3) Il y a des antennes pour lesquelles on a des factures mensuelles tandis que pour d'autres, on les reçoit moins régulièrement (trimestre, semestre, année). Ajoute une colonne à ton tableau qui calcule le nombre de jours entre le début de la période de facturation et la fin de la période de facturation.
4) A partir de cette nouvelle colonne, crée une autre colonne qui nous donne la consommation journalière moyenne de la période.
5) Merci d'ajouter également une colonne qui donne, pour chaque antenne, le nombre de factures dont on dispose au total. Pas grave si l'information se répète à chaque ligne pour une même antenne.
6) Et information bonus si tu y arrives : les équipes aimeraient beaucoup avoir une liste de toutes les antennes avec, pour chaque antenne, le coefficient de variation de la consommation. Cela permettra d'avoir une idée, pour chaque antenne, de la dispersion de sa consommation d'énergie.
7) Enfin, tu dois exporter ces deux fichiers obtenus pour pouvoir l'envoyer aux équipes de l'opérateur et leur demander si c'est bien cela qu'ils attendaient de toi.


## 3. Rendu attendu
- Un fichier .ipynb qui contient l'ensemble de tes analyses.
- Le fichier csv final, beaucoup plus clean et exploitable par les équipes de comptabilité. Et si tu as réussi cette étape, l'autre fichier csv qui donne la liste des coefficients de variation.

