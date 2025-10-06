#Algèbre #Prépa #EspaceVectoriel

Dans ce chapitre $\mathbb{K}$ désigne un [[Corps]]
# Définition

### Espace Vectoriel

Soit $E$ un [[Ensemble]] non vide muni d'une [[Loi de composition]] interne $+$ et d'une loi externe $cd$ de $\mathbb{K}$ sur $E$, On dit que $(E, +, \cdot)$ est un $\mathbb{K}$-espace vectoriel (abrégé $\mathbb{K}$-ev) si:
- $(E, +)$ est un groupe commutatif
- $\forall (\lambda, \mu) \in \mathbb{K}^2, \forall x \in E, (\lambda + \mu) \cdot x = \lambda \cdot x + \mu \cdot x$ (Distributivité de $\cdot$ sur les scalaires)
- $\forall (\lambda, \mu) \in \mathbb{K}^2, \forall x \in E, \lambda \cdot (\mu \cdot x) = (\lambda \mu)x$ (Associativité des scalaires)
- $\forall x \in E, \forall y \in E, \lambda\cdot (x + y) = \lambda\cdot x + \lambda \cdot y$ (distributivité sur les vecteurs)
- $\forall x \in E, 1\cdot x = x$
Les éléments de $E$ sont appelé vecteurs, les éléments de $\mathbb{K}$ sont appelé des scalaires.
### Vecteur nul

On appelle vecteur nul l'élément neutre de l'addition dans $E$ noté $0_E$
### Combinaison linéaire

Soient $x$ et $y$ deux vecteurs de $E$ et $\lambda, \mu$ deux scalaires. la somme $\lambda x + \mu y$ est appelé combinaison linéaire des vecteurs $x$ et $y$. Cette notion est généralisable à toute combinaison composés d'un nombre finis de vecteurs: Soient $n \in \mathbb{N}, x_i \in E, \forall i \in [\![1, n]\!]$, le vecteur $\sum_{i = 1}^n \lambda_i \cdot x_i$ est une combinaison linéaire des $(x_i)_{i \in [\![1, n]\!]}$.
### Sous espace Vectoriel

Soit $F$ un sous ensemble de l'espace vectoriel $(E, +, \cdot)$. On dit que $F$ est un $\mathbb{K}$-sous-espace vectoriel (abrégé $\mathbb{K}$-sev) de $E$ si:
$$
F \subset E \, \land \, (F, +, \cdot) \text{ est un espace vectoriel}
$$
### Somme de sous espace vectoriel

Soit $A$ et $B$ deux $\mathbb{K}$-sev de $E$. On appelle somme de $A$ et $B$ l'ensemble noté $A+B$ défini par:
$$
A + B = \{x + y | x \in A, y \in B\}
$$
De même, si on a $n \in \mathbb{N}^*$ $\mathbb{K}$-sev de $E$ noté $(E_i)_{i \in [\![1, n]\!]}$, on a la somme des $n$ sev de $E$ défini par:
$$
E_1 + E_2 + \dots +E_n = \{\sum_{i = 1}^n x_i \, \forall x_i \in  E_i\}
$$
### Somme directe

Soit $A$ et $B$ deux -sev de $E$ . On dit que  et  sont en somme direct, notée $A \oplus B$, si tout élément de $A + B$ possède une unique écriture de la forme: $u = u_A + u_B$:
De même, si on a $n \in \mathbb{N}^*$ $\mathbb{K}$-sev de $E$ noté $(E_i)_{i \in [\![1, n]\!]}$, on a la somme directe des $n$ sev de $E$ défini par:
$$
E_1 \oplus E_2 \oplus \dots \oplus E_n = \{ \exists! (x_i)_{i \in [\![1, n]\!]} \} | x = \sum_{i=1}^n x_i
$$
### Espace supplémentaire

Soit $A$ et $B$ deux $\mathbb{K}$-sev de $E$. On dit que $A$ et $B$ sont supplémentaires si: $A \oplus B = E$.
### Espace vectorielle engendré

Soit $(e_{1,} \dots, e_n)$ une famille de vecteur de $E$. On appelle $\mathbb{K}$-sous-espace-vectoriel engendré par les vecteurs $(e_i)_{i \in [\![1, n]\!]}$ l'ensemble, noté Vect$(e_{1,}\dots, e_n)$ définit par:
$$
\text{Vect}(e_{1},\dots, e_{n)}= \{\lambda_{1}e_{1} + \lambda_2e_{2}+ \dots + \lambda_n e_{n} | (\lambda_{1}, \dots, \lambda_{n})\ \in \mathbb{K}^n\}
$$
# Théorèmes

### Théorèmes 1
# Propriétés

- Propriétés du vecteur nul:
	- $\lambda \cdot x = 0$
	- $0 \cdot x = 0$
	- $\lambda \cdot x = 0 \Leftrightarrow \lambda = 0 \text{ ou } x = 0$
	- $\lambda \cdot (-x) = (-\lambda) \cdot x = - \lambda \cdot x$
- Soit $E$ un $\mathbb{K}$-ev et $F \subset E$. $F$ est un $\mathbb{K}$-sev de $E$ ssi:
	- $F \neq \emptyset$
	- $\forall (x, y) \in F^2, \forall \lambda \in \mathbb{K}, \lambda \cdot x + y \in F$
- Intersection: si $F$ et $G$ sont deux $\mathbb{K}$-sev de $E$, alors $F \cap G$ est aussi un $\mathbb{K}$-sev de $E$.
- Soit $A$ et $B$ deux sev de $E$, alors $A + B$ est un sev de $E$
- Soit $A$ et $B$ deux sev de $E$, $A$ et $B$ sont en somme directe ssi: $A \cap B = \{0_E\}$
- Vect$(e_{1,}\dots, e_n)$ est le plus petit $\mathbb{K}$-sev contenant la famille $(e_{1},\dots, e_n)$.