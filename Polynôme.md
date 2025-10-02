#Analyse #Algèbre #polynome #Prépa 

Dans cette section, $\mathbb{K}$ désigne un [[Corps]]
# Définitions

### Polynôme à coefficient dans $\mathbb{K}$
Est polynôme à coefficient dans $\mathbb{K}$ toute [[Suite Numériques]] $(a_k)_{k \in \mathbb{N}}$ telle que:

$$
\exists N \in \mathbb{N}, \forall k \in \mathbb{N}, k > N, a_k = 0
$$
### Polynôme Nul
Soit $P$ un polynôme à coefficient dans $\mathbb{K}$, si $P$ vérifie $\forall k \in \mathbb{N}, a_k = 0$, on dit que $P$ est le polynôme nul noté: $0_{\mathbb{K}[X]}$.

### Degré et valuation
Soit $P = (a_i)_{i\in [\! \![1, n]\! \!]}$, un polynôme avec $\forall k \in \mathbb{N}, k>n, a_k = 0$ et $a_n \neq 0$: 
- $n$ est le **degré** du polynôme, noté deg($P$).
- La **valuation** de $P$ noté val(P) est le plus petit entier $k$ tel que $a_k = 0$.
- Par convention, deg($0_{\mathbb{K}[X]}$) = $-\infty$ et val($P$) = $+\infty$.
- Si deg($P$) = val($P$), alors $P$ est un **monôme**
- Si $P \neq 0_{\mathbb{K}[X]}$ est constant, alors deg($P$) = 0.

### Coefficients
**Coefficient**: Soit $P = (a_i)_{i\in [\![1, n]\!]}$, un polynôme avec $\forall k \in \mathbb{N}, k>n, a_k = 0$ et $a_n \neq 0$:
- $a_n$ est le **coefficient dominant** de $P$.
- $a_0$ est le **terme constant** de $P$.
- Si $a_n$ = 1, on dit que $P$ est **unitaire** ou normalisé.
- $P$ est un polynôme pair si $\forall k \in \mathbb{N}, a_{2k+1} = 0$.
- $P$ est un polynôme impair si $\forall k \in \mathbb{N}, a_{2k} = 0$.

### Indéterminé
On pose $X$ le polynôme défini par $(0, 1, 0, 0,...)$. Il s'agit de l'indéterminé.

**Ensembles** :
- L'ensemble des Polynômes à coefficient dans $\mathbb{K}$ est noté $\mathbb{K}[X]$.
- L'ensemble des Polynômes à coefficient dans $\mathbb{K}$ de degré inferieur ou égal à $n$ est noté $\mathbb{K}_n[X]$.
### Polynôme Dérivé
Soit $P \in \mathbb{K}[X]$, deg($P$) = $n$,  Le polynôme dérivé de $P$ est le Polynôme $P^{'}$ suivant
- Si deg($P$) $\leqslant$ 0, alors $P^{'} = 0_{\mathbb{K}[X]}$.
- Si deg($P$) $>$ 0, alors $P^{'} = \sum_{i=1}^nia_iX^{i-1}$.
On définit les dérivé successive de $P$ par récurrence. On obtient $\forall k \in [\![1, n]\!]$:
$$
P^{(k)} = \sum_{i=k}^n \Pi_{j=0}^{i-k}(i-j)X^{i-k}
$$
### Racines
Soit $\alpha \in \mathbb{K}$, soit $P \in \mathbb{K}[X]$ et $\tilde{P}$ la [[Fonction Polynômial]] associé à $P$. On dit que $\alpha$ est racine de $P$ dans $\mathbb{K}$ ssi $\tilde{P}(\alpha) = 0$.
### Racines Multiples
Soit $P \in \mathbb{K}[X]$. Soit $\alpha \in \mathbb{K}$. $\alpha$ est une racine de multiplicité $k$ de $P$ ssi:
$$
\begin{cases}
(X - \alpha)^k & \text{divise } P \\
(X - \alpha)^{k+1} &\text{ne divise pas } P
\end{cases}
$$

### Contenu

Soit $P \in \mathbb{Z}[X] \neq 0_{[X]}$, On appelle contenu de $P$ noté $c(P)$ le pgcd des coefficients de $P$
# Opérations

Soient $\lambda \in \mathbb{K}$, $P = (a_i)_{i\in \mathbb{N}}$, et $Q = (b_i)_i\in \mathbb{N}$ deux polynômes,
- **Somme** : $P + Q$ est un polynôme défini par $(a_i + b_i)_{i \in \mathbb{N}}$.
- **Multiplication par un scalaire** : $\lambda P$ est un polynôme défini par $(\lambda a_i)_{i \in \mathbb{N}}$
- **Produit** : $PQ$ est un polynôme $(c_i)_{i \in \mathbb{N}}$ défini par $c_i = \sum_{j=0}^{i}a_jb_{i-j}$.
- **Composition** : $P\,o\,Q = \sum_{i=0}^n a_kQ^k$.

Opérations sur les degrés:
- deg($P + Q$) $\leqslant max(deg(P), deg(Q))$.
- Si deg($P$) $\neq$ deg($Q$), alors deg($P + Q$) $= max(deg(P), deg(Q))$.
- Si $\lambda \neq 0$, deg($\lambda P$) = deg($P$)
- deg($PQ$) = deg($P$) + deg($Q$)
- deg($P\,o\,Q$) = deg($P$) $\times$ deg($Q$).

# Théorèmes

### Unicité
Tout Polynôme $P$ s'écrit de manière unique comme combinaison linéaire de puissance de l'indéterminé $X$.
$$
P \in \mathbb{K}{[X]}, \; P \neq 0_{\mathbb{K}[X]}, \; \exists!(a_i)_{i \in [\! \![0, n]\! \!]} \in \mathbb{K}^{n+1} \; | \; a_n \neq 0 \: \land \: P = \sum_{i=0}^n a_kX^n
$$
et deg($P$) = $n$.

### Décomposition

Tout polynôme de $\mathbb{K}[X]$ se décompose en produit de polynômes irréductibles de $\mathbb{K}[X]$ à ordres de facteurs près.
### Structures Algébriques
- $(\mathbb{K}{[X]}, +)$ est un [[Groupe]] abélien.
- $(\mathbb{K}{[X]}, +, \times)$ est un [[Anneau]] commutatif intègre.
- $(\mathbb{K}{[X]}, +, .)$ est un $\mathbb{K}$ [[Espace Vectoriel]].


### Théorème Fondamental
Soit $P \in \mathbb{K}[X], \tilde{P}(\alpha) = 0 \Leftrightarrow (X - \alpha) | P$

**Corollaire** : Soient $P \in \mathbb{K}[X], n \in \mathbb{N}$ tel que deg($P$) $\leqslant n$. Alors:
- P admet au maximum $n$ racines dans $\mathbb{K}$
- Si $P$ possède au moins $n + 1$ racines, alors $P = 0$
### [[Formules de Taylor]] appliqués aux polynômes
Soit $P \in \mathbb{K}[X]$ de degré $n$, $\alpha \in \mathbb{K}$, alors:
$$
f(x) = \sum_{k=0}^{n}\frac{P^{(k)}(\alpha)}{k!}(X-\alpha)^k
$$
À multiplication d'un scalaire près, Tout polynôme de $\mathbb{K}$ se décompose de façon unique en produit de polynômes irréductibles.


### Coïncidence
Soit $P \in \mathbb{K}_n[X]$ et $G \in \mathbb{K}_n[X]$ deux polynômes coïncidents en $n + 1$ points, alors ils sont égaux.

### Théorème fondamental n°2
Soit $P \in \mathbb{K}[X], \alpha \in \mathbb{K}$.
$$
\alpha \text{ est racine de } P \text{ de multiplicité } k \Leftrightarrow
\begin{cases}
\tilde{P}(\alpha) = 0 \\
\tilde{P}'(\alpha) = 0 \\
\vdots \\
\tilde{P}^{k-1}(\alpha) = 0 \\
\tilde{P}^{k}(\alpha) \neq 0
\end{cases}
$$
# Propositions

- Deux polynômes sont égaux si tous leurs coefficients sont égaux.

- $PQ = 0 \Rightarrow (P = 0_{\mathbb{K}[X]})\lor(Q = 0_{\mathbb{K}[X]})$.

- Soit $n \in \mathbb{N}, n > 0$, alors $X^n$ est le polynôme défini par:
$$
(b_i)_{i\in \mathbb{N}}, \; b_n = 1, \; \forall i \in \mathbb{N} / \{n\}, b_i = 0
$$

- Binôme de Newton: Soient $(P,Q) \in \mathbb{K}{[X]}$ et $n \in \mathbb{N}$, alors:
$$
(P+Q)^n = \sum_{k=0}^n\begin{pmatrix} n \\ k \end{pmatrix} P^kQ^{n-k}
$$