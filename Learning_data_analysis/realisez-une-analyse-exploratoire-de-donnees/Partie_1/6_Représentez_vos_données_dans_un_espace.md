## `Notes`

- L'analyse d'un espace à deux dimensions se nomme algèbre linéaire
- L'algèbre linéaire étudie principalement l'espace vectoriel
- L'espace vectoriel est de manière vulgaire un espace où tous les objets sont des vecteurs.


- On note un vecteur A comme :

$$
\begin{pmatrix} x \\
y
\end{pmatrix}
$$

- Un vecteur peut etre representé en n dimensions (n>2) , on a donc

$$
\begin{pmatrix}
x_{1} \\ 
x_{2} \\ 
x_{3} \\
\ldots \\ 
x_{n} 
\end{pmatrix}
$$

où  $x_{1} ,  x_{2} , x_{3} , \ldots , x_{n}$ sont appeleées les composantes du vecteur X

- Si chaque vecteur est un nombre réel et qu'on associe à cet espace vectoriel un produit scalaire alors on dit qu'on travaille dans un espace euclidien

## La notion d'inertie
Elle définit la dispersion d'un nuage de point.Un objet avec une forte inertie est un objet difficile à mettre en mouvement ou à faire entrer en rotation.

L'inertie du nuage de points N1 est la moyenne des carrés des distances entre les points $M_{i}$ et leur centre de gravité G.

On note la distance entre le point i et G : $d(M_i,G)$

L'inertie totale de $N_I$ par rapport à G est donc : $\frac{1}{n} \sum_{i=1}^{n} d(M_i,G)^2$

Linertie du nuage de points $N_i$ est aussi la somme des variances sur toutes les p dimensions : 
$\frac{1}{n} \sum_{i=1}^{n} d(M_i,G)^2 = \frac{1}{n} \sum_{j=1}^{p} \sum_{i=1}^{n} (x_{ij} - \bar{x_j})^2 = \sum_{j=1}^{p} Var[j]$
