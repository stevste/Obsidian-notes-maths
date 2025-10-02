#Algèbre #Groupe 
# Définition

### Groupe symétrique
Soit $E$ un ensemble, l'ensemble $\mathbb{G}(E)$ des bijections de $E$ vers lui même munit de la composition est un groupe nommé le groupe symétrique de $E$. Pour $n \in \mathbb{N}$ on note $\mathbb{G}_n$ le sous groupe $\mathbb{G}(\{1,2,...,n\})$.
### Permutation
L'ensemble $\mathbb{G}_n$ des permutations des éléments $\{1,...,n\}$ est un groupe de cardinal $|\mathbb{G}_n| = n!$.
### Partie stable
Une partie A de $\{1,...,n\}$ est stable par $\sigma \in \mathbb{G}_n$ si $\sigma(A) \subset A$
### Support
L'ensemble $\{1,...,n\}$ privé des points fixes de la permutation $\sigma \in \mathbb{G}_n$, est appelé support de $\sigma$ noté Supp($\sigma$).
### Cycle
Soit $l\in \mathbb{N}, l \geqslant 1$. et $(i_k)_{k\in [[1, l]]}$ des éléments distincts de $\{1,...,n\}$. La permutation $\gamma \in \mathbb{G}_n$ est une application défini par:
$$
\gamma(j) = 
\begin{cases}
j \text{ si } j \notin (i_k)_{k\in [[1, l]]}\\
i_{k+1}  \text{ si } j = i_k, k < l \\
i_1 j \text{ si } = i_l \\
\end{cases}
$$

# Théorème

### Décomposition en cycle
Tout $\sigma \in \mathbb{G}_n$ s'écrit comme produit de cycles $\gamma_i$ de longueur $l \geqslant 2$ dont les supports sont deux à deux disjoints et correspondent aux orbites de l'action $\langle\sigma\rangle \longrightarrow \mathbb{G}_n$ sur l'ensemble $\{1,...,n\}$
# Proposition
- Soit $\sigma , \rho$ deux permutations, alors: $$ Supp(\sigma\rho) \subset Supp(\sigma) \cup Supp(\rho)$$
- Si Supp($\sigma$) $\cap$ Supp($\rho$) = $\emptyset$, alors:
	- $\sigma\rho(i) = \sigma(i)$ si $i \in$ Supp($\sigma$) (idem pour $\rho$)
	- $\sigma\rho = \rho\sigma$
	- $\sigma\rho = e \Leftrightarrow \rho = \sigma = e$