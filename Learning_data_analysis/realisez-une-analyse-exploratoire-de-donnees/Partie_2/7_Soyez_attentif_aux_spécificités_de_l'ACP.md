# Points d'attention

Si dans le cercle des corrélations des variables semblent corrélées , c'est bien de revenir au variables initiales en calculant leurs coefficients de corrélation ou la matrice de corrélation pour s'en assurer .

Si des individus sur un plan factoriel ont l'air similaires ou différents on peut revenir à nos données pour le confirmer.

Il ne faut pas oublier les deux objectifs principaux de l'ACP :

- Etudier la variabilité des individus
- Etudier les liaisons entre les variables


Limites

L'ACP utilise le coefficient de pearson `r`.Elle ne peut donc mesurer que les corrélations linéaires.On peut utiliser l'ACP avec noyau ou Kernel ACP pour y remédier

Le coefficient `r` est très sensible aux outliers (avantages/inconvénients).Sur le plan factoriel on remarque visuellement des outliers par le fait qu'ils s'ecartent beaucoup des autres individus.

La non robustesse de l'ACP aux outliers permet de les detecter facilement donc n'est pas vraiment problématique

L'ACP a comme autre inconvénient de se limiter aux variables quantitatives.D'autres méthodes factorielles permettent cependant d'y remédier:

- l'analyse des correspondances multiples pour des variables qualitatives ;

- l'analyse factorielle des données mixtes.
