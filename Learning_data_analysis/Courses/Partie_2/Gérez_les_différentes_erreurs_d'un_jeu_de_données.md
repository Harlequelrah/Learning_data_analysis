# Gérez les différentes erreurs d'un jeu de données


## Les valeurs manquantes 

- Ne rien faire (si peu de valeurs manquantes)

- Oublier une variable (si trop de valeurs manquantes)

- Oublier des individues (risque d'échantillon trop petit ou non représentatif)

- Imputation (par exemple par moyenne : remplacer une valeur manquante par la moyenne des autres )

## Outliers 

On les distingue en connaissance du contexte 

- Pour les valeurs aberrante (on est sur qu'elle est fausse , on la supprime )
  
- Pour les valeurs atypiques (on est pas sur qu'elle soit fausse mais elle est atypique , soit on la conserve soit on crée un sous-echantillon sans elle)

- Les méthodes robustes ne sont pas sensibles au outliers . ex : `la médiane` donc on peut conserver ; alors que `la moyenne ` est très sensible aux outliers donc vaut mieux la supprimer .

## Doublons 

On mix les valeurs des individus et on fait la moyenne entre deux valeurs numériques au besoin .  


**Notes** : Toujours garder l'échantillon originale et faire des copies lorsqu'on souhaite produire des sous-echantillons


  
