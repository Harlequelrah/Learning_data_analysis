# Résumé
Nous avons deux espaces : 

- L'espace $\mathbb{R}^p$ à p dimension où on place le nuage des individus $N_I$
- L'espace $\mathbb{R}^k$ à n dimension où on place le nuage des variables $N_K$

Pour repondre à nos deux objectifs nous allons créer deux graphiques : 
- La projection du nuage des individus $N_I$ sur le premier plan factoriel
- La projection du nuage des variables $N_K$ sur le premier plan factoriel : `cercle des corrélations`

**note** : le premier plan factoriel représente les deux premiers axes d'inertie


## Cercle des corrélations 

Les fleches ne depassent jamais le cercle tant que les données sont centrées (ce qui est standard en ACP) et si elle sont réduites on dit que l'ACP est normées.

L'objectif est de trouver des variables corrélées entre elles pour avoir des variables synthétiques qui seront composantes principales.

Exemple : 
![cercle des corrélations](Learning_data_analysis/realisez-une-analyse-exploratoire-de-donnees/assets/cercle_correlations_P2C3.png)

La projection d'une variable v sur F1 par exemple donne son coefficient de correlation avec F1 . 

On remarque alors que le coefficient de correlation de $v_1$ et F1 vaut `0.9`


## Analyse de votre jeu de données

Cercle du jeu de donnée sur openclassroom s

![Cercle jeu de donnée Openclassrooms](Learning_data_analysis/realisez-une-analyse-exploratoire-de-donnees/assets/cercle_correlation_dataset_Openclassrooms.png)


Les variables les plus corrélées avec F1 sont : 

- la durée ;

- le nombre de chapitres (nbChapitres) ;

- le nombre d’évaluations du cours (nbEvaluations).

En plus de la progression qui est corrélée négativement à F1.

Ces variables sont unies par un mode commun c'est à dire une notion . Ici il s'agit de la longueur du cours.
Quand un cours est long , sa durée et son nombre de chapitres sont conséquents aussi , et sa progression est plus lente.

les variables les plus corrélées à F2 sont :

- la difficulté (avec une corrélation négative) ;

- la moyenne de classe ;

- la proportion de quiz par rapport au nombre total d’évaluations.

On peut donc interpréter F2 comme la facilité du cours.

Si on doit résumé notre jeu de données on peut le faire suivant ces deux tendances : 

- La longueur du cours : on a des cours plus long que d'autres
- La facilité du cours : on a des cours qui sont faciles et d'autres difficiles

## Attention aux pièges

Sur un plan factoriel il est préférable de ne pas interpréter que les variables avec les flêches les plus longues.
Les variables avec les flêches courtes sont mal représentées , c'est à dire qu'elles font perdent assez d'information .
Une variable bien représentée est une variable pour laquelle on perd très peu d'information ce qui se traduit par une flêche de longueur proche de 1 donc proche du cercle des corrélations.


**note** : Plus on avance dans les dimensions synthétiques plus l'interpretation est complexe : F1,F2 sont plus faciles à interpreter que F5 et F6.
**attention** : Le cercle des corrélations n'est pas fait pour étudier les corrélations entre les variables initiales mais entre une variable initiale et un axe d'inertie.
