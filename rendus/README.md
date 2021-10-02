
# TD1 : Programmation Par Contraintes



### <u>Consigne :</u> Réaliser les questions 1 de chacun des exercices.



#### Exercice 1 - Q1 :

* Variables : $X = \{x_{1,1}, ..., x_{1,n}\}$ `// Il s'agit de toutes les cases possibles de notre échiquier de taille NxN`
* Domaine : $D(X) = \{0,1\}$ `// Une reine peut être présente ou ne pas être présente sur une case donnée`
* Contraintes :
  * $\forall i \in \{1, ..., n\} \ \ \sum_{j=1}^{n}x_{i,j}=1$  `// Lignes (une seule reine par ligne)`
  * $\forall j \in \{1, ..., n\} \ \ \sum_{i=1}^{n}x_{i,j}=1$  `// Colonnes (une seule reine par colonne)`
  * $\forall x_{i,j}, x_{k,l} \ \ avec \ \ x_{i,j} \neq x_{k,l} \ \ i+j = k+l \Rightarrow x_{i,j}+x_{k,l}\leqslant1$ `// Diagonales supérieures (au plus une reine par diagonale supérieure)`
  * $\forall x_{i,j}, x_{k,l} \ \ avec \ \ x_{i,j} \neq x_{k,l} \ \ i-j = k-l \Rightarrow x_{i,j}+x_{k,l}\leqslant1$ `// Diagonales inférieures (au plus une reine par diagonale inférieure)`



#### Exercice 2 - Q1 :

* Variables : 

  * $X = \{D, E, M, N, O, R, S, Y\}$  `// Il s'agit des différentes lettres de nos mots`
  * $X' = \{X_1,X_2,X_3\}$ `// Il s'agit des retenues possibles lors de notre addition`

* Domaine : 

  * $D(X \ \textbackslash \ \{S\} \cup\{M\})=\{0, ... ,9\}$ `// Pour toutes les lettres exceptés S et M les valeurs possibles vont de 0 à 9`
  * $D(\{S\}) = D(\{M\}) = \{1,...,9\}$ `// Pour les lettres S et M les valeurs possibles vont de 1 à 9`
  * $D(X') = \{0, 1\}$ `// Soit l'addition de 2 lettres entraine une retenue, soit non`

* Contraintes : 

  > Pour chaque colonne de l'addition, on définit une équation correspondant à une contrainte. À chaque addition il peut y avoir une retenue qui se répercute sur l'addition suivante.

  * $D + E = Y + 10X_1$ 
  * $N + R + X_1 = E + 10X_2$
  * $E + O + X_2 = N + 10X_3$
  * $S + M + X_3 = O + 10M$

#### Exercice 3 - Q1 :

* Variables : 

* Domaine : 

* Contraintes :

  

#### Exercice 4 - Q1 :

* Variables :
* Domaine : 
* Contraintes :

