# Recherchez une bonne partition
Ici nous allons regrouper des lignes , c'est à dire créer des groupes d'invidus : `partitionner les données`.

## Partitionnez vos données

Au niveau vocabulaire , partitionnement et clustering sont équivalent.

Les groupes recherchés sont appelés clusters.

Lorsque tous les individus sont affectés à l'un des groupe on parle de partition.

L'objectif premier peut être de determiner les groupes et ensuite de regrouper les individus pour réduire la taille du jeu de donnée.

Ainsi comme les individus d'un groupe sont assez similaires on peut juste étudier les caractéristiques du groupe.Ceci équivaut à étudier les caractéristiques de `l'individu moyen` de chaque groupe.

Ansi pour un jeu de donnée de n individus et p variables  partitionné en 3 groupes on peut le ramener à un tableau de 3 lignes et p variables.

Il y aura cependant perte d'information car deux individus similaires ne sont pas totalement identique .

Le challenge sera de trouver des méthodes qui font perdre le moins d'information .

Nous chercherons alors un critère pour évaluer la qualité d'une partition .

## Évaluez la qualité d'une partition


### Inertie intraclasse

En calculant l'inertie de chaque cluster et en faisant la moyenne on obtient `l'inertie intraclasse` ou `variance interclasse` ou `variation intraclasse`.

Par cet indicateur on cherche à repondre à la question `à quel point nos clusters sont homogènes?` c'est à dire ressérés.

Plus les clusters sont resserés mieux c'est : `on cherche donc à minimiser la variance intraclasse`.

### Inertie Interclasse
Si on s'imagine un nouveau nuage de points avec les centres de gravité respectifs de chaque cluster.

L'inertie de ce nuage de point imaginaire s'appelle `l'intertie interclasse` qui est aussi grande que les centres de gravité sont éloignés.Il est aussi appelé `variance interclasse` ou `variation interclasse`.

On essaye de répondre à la question `à quel point nos clusters sont éloignés les uns des autres?`

Plus les clusters sont éloignés , mieux c'est : `on cherche donc à maximiser l'inertie interclasse`.


### Centroïde
C'est le centre de gravité du cluster . Il correspond à un individu théorique et moyen.
Il se calcule en prennant la moyenne des différentes composantes des individus du cluster.

## Relation entre l' inertie interclasse et l'inertie intraclasse

### Théorème de Huygens
Il se nomme également **équation d'analyse de la variance** et s'exprime comme suite :

`intertie totale = inertie intraclasse + inertie interclasse`

L'inertie totale étant constante ,**minimiser l'inertie intraclasse est équivalent mathématiquement à maximiser l'inertie interclasse**.



## Autres scores pour évaluer un bon clustering
- l'indice de Davies Bouldin qui prend en compte la variance intraclasse et interclasse ;

- le Silhouette Score qui prend en compte l'appartenance de chaque individu au plus proche cluster.


