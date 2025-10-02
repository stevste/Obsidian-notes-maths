#Probabilité #Prépa
# Définitions

### Expérience aléatoire

On appelle expérience aléatoire une expérience dont l'issue dépend du "hasard". À chaque expérience aléatoire, on associe un ensemble $\Omega$ appelé univers, dont les éléments $\omega$ représentes les différentes issues possibles de l'expérience.
### Tribu

On dit que $\mathcal{A} \subset P(\Omega)$ est une tribu de parties de $\Omega$ ssi:
	- $\Omega \in \mathcal{A}$ (L'univers est dans la tribu)
	- $A \in \mathcal{A} \Rightarrow \overline{A} \in \mathcal{A}$
	- $(\forall i \in I \subset \mathbb{N}, A_i \in \mathcal{A}) \Rightarrow \bigcup_{i\in I} A_i \in \mathcal{A}$ (Stabilité par union dénombrable)
### Évènement

On appelle évènement relatif à une expérience aléatoire, tout élément de la tribu $\mathcal{A}$ de $\Omega$.
On appelle évènement élémentaire tout singleton de la tribu $\mathcal{A}$ de $\Omega$ .
### Système complet d'évènement

Soit $J \in \mathbb{N}$. On dit qu'une famille d'évènement $\{A_j\}_{j \in J}$ forme un système complet d'évènement ssi:
	1) Les évènements $A_j$ sontg incompatibles deux à deux: $\forall(i, j) \in J^2, i \neq j \Rightarrow A_i \cap A_j = \emptyset$
	2) Leurs union est égale à $\Omega$: $\bigcup_{j \in J} A_j = \Omega$
### Espace probabilisable

Le couple $(\Omega, \mathcal{A})$ est appelé espace probabilisable
### Probabilité

On appelle probabilité sur $(\Omega, \mathcal{A})$ toute application $\mathbb{P} \longrightarrow [0; 1]$ tel que:
	- $\mathbb{P}(\Omega) = 1$
	- Pour toute suite $(A_n)$ d'évènement incompatible de $\mathcal{A}$, on a:
	$$
	\mathbb{P}(\bigcup_{i \in \mathbb{N}}A_i) = \sum_{i=0}^{+\infty} \mathbb{P}(A_i)
	$$

On dit que $(\Omega, \mathcal{A}, \mathbb{P})$ est un espace probabilisé
### Presque impossibilité/sûreté

Soit $A \in \mathcal{A}$,

- Si $\mathbb{P}(A) = 0$, on dit que l'évènement $A$ est presque impossible (négligeable)
-  Si $\mathbb{P}(A) = 1$, on dit que l'évènement $A$ est presque certain
### Équiprobabilité

Soit $\Omega = \{\omega_1 \dots \omega_n\}$ un univers fini non vide. On dit qu'il y a équiprobabilité si:
$$
\forall (i, j) \in [\![1, n]\!]^2, \mathbb{P}(\{w_i\}) = \mathbb{P}(\{w_j\})
$$
### Indépendance

Soit $(\Omega, \mathcal{A}, \mathbb{P})$ un espace probabilisé. On dit que deux évènements $A, B$ sont indépendants si $\mathbb{P}{A \cap B} = \mathbb{P}(A) \times \mathbb{P}(B)$.
### Indépendance mutuelle

On dit que les évènements $A_1 \dots A_n$ sont mutuellement indépendants ssi:
$$
\forall I \subset [\![1, n]\!], \mathbb{P}(\bigcap_{i\in I}A_i) = \prod_{i \in I}(A_i)
$$
### Probabilité conditionnelle

Soit $A$ et $B$ deux évènements et $\mathbb{P}(B) \neq 0$, On définit la probabilité de $A$ sachant $B$ par:
$$
\mathbb{P}_B(A) = \frac{\mathbb{P}(A \cap B)}{\mathbb{P}(B)}
$$
# Théorèmes
### Croissance/Décroissance

Soit $(\Omega, \mathcal{A}, \mathbb{P})$ un espace probabilisé, soit $n \in \mathbb{N}$ et $A_1 \dots A_n$ une suite d'évènements.
	1) Si $(A_n)$ est croissante au sens de l'inclusion, alors la suite $\mathbb{P}(A_i)_{i \in \mathbb{N}}$ est croissante et on a: $$\lim_{n \to +\infty} \mathbb{P}(A_n) = \mathbb{P}(\bigcup_{i=0}^{+\infty} A_i)$$ 
	2) Si $(A_n)$ est décroissante au sens de l'inclusion, alors la suite $\mathbb{P}(A_i)_{i \in \mathbb{N}}$ est décroissante et on a: $$ \lim_{n \to +\infty} \mathbb{P}(A_n) = \mathbb{P}(\bigcap_{i=0}^{+\infty} A_i) $$
#### Corollaire

Soit $(\Omega, \mathcal{A}, \mathbb{P})$ un espace probabilisé, soit $n \in \mathbb{N}$ et $A_1 \dots A_n$ une suite d'évènements.
$$
\mathbb{P}(\bigcup_{i=0}^{+\infty}A_i) = \lim_{n \to +\infty} \mathbb{P}(\bigcup_{i=0}^nA_i)
$$
De même:
$$
\mathbb{P}(\bigcap_{i=0}^{+\infty}A_i) = \lim_{n \to +\infty} \mathbb{P}(\bigcap_{i=0}^nA_i)
$$
### Formule des probabilités composées

Soit $(\Omega, \mathcal{A}, \mathbb{P})$ un espace probabilisé, soit $n \in \mathbb{N}$ et $A_1 \dots A_n$ une suite d'évènements tel que $\mathbb{P}(A_1 \cap \dots \cap A_n) \neq 0$. Alors:
$$
\mathbb{P}(A_1 \cap \dots \cap A_n) = \mathbb{P}(A_1)\times\mathbb{P}_{A_1}(A_2)\times \mathbb{P}_{A_1 \cap A_2}(A_3) \times \dots \times \mathbb{P}_{A_1 \cap \dots \cap A_{n-1}}(A_n)
$$
### Formule des probabilités totales

Soit $(\Omega, \mathcal{A}, \mathbb{P})$ un espace probabilisé. Soit $(A_i)_{i  \geqslant 0}$ un système complet d'évènements tel que, $\forall i \in \mathbb{N}, \mathbb{P}(A_i) \neq 0$. Soit $B$ un évènement, alors:
$$
\mathbb{P}(B) = \sum_{i=1}^{+\infty} \mathbb{P}_{A_i}(B) \times \mathbb{P}(A_i)
$$
### Formule de Bayes

Soit $(\Omega, \mathcal{A}, \mathbb{P})$ un espace probabilisé. Soit $(A_i)_{i  \geqslant 0}$ un système complet d'évènements tel que, $\forall i \in \mathbb{N}, \mathbb{P}(A_i) \neq 0$. Soit $B$ un évènement, alors:
$$
\forall k \in \mathbb{N}, \mathbb{P}_B(A_k) = \frac{\mathbb{P}_{A_k}(B) \times \mathbb{P}(A_k)}{\sum_{i = 0}^{+\infty}\mathbb{P}_{A_i}(B) \times \mathbb{P}(A_i)}
$$
# Propriété

- Soit $\Omega$ un univers et soit $A \in \Omega, A \neq \emptyset$:
	- $\mathcal{A} = {\emptyset, \Omega}$ est la plus petite tribu sur $\Omega$
	- $\mathcal{A} = {\emptyset, A, \overline{A}, \Omega}$ est la plus petite tribu contenant l'élément $A$
	- $\mathcal{A} = P(\Omega)$ est la plus grande tribu possible sur $\Omega$
- Soit $\Omega$ un univers et $\mathcal{A}$ une tribu de de parties de $\Omega$. On a alors:
	- $\emptyset \in A$
	- $\forall(A, B) \in \mathcal{A}^2, A \cup B \in \mathcal{A}, A \cap B \in \mathcal{A}, A \setminus B \in \mathcal{A}$
	- $(\forall i \in I \subset \mathbb{N}, A_i \in \mathcal{A}) \Rightarrow \bigcap_{i \in I}A_i \in \mathcal{A}$
- Soit $(\Omega, \mathcal{A}, \mathbb{P})$ un espace probabilisé, $A$ et $B$ deux évènements.
	- **Évènement contraire**: $\mathbb{P}(\overline{A}) = 1 - \mathbb{P}(A)$
	- **Évènement impossible**: $\mathbb{P}(\emptyset) = 0$
	- **Croissance**: $A \subset B \Rightarrow \mathbb{P}(A) \leqslant \mathbb{P}(B)$
	- **Union**: $\mathbb{P}(A \cup B) = \mathbb{P}(A) + \mathbb{P}(B) - \mathbb{P}(A \cap B)$
	- **Crible de Poincaré**: Soient $(A_i)_{i \in \mathbb{N}}$ une suite d'évènement incompatible deux à deux: $$ \mathbb{P}(\bigcup_{i=1}^n) = \sum_{k=1}^n \mathbb{P}(A_k)
	 $$
	- Pour une suite quelconque d'évènement, on a: $$  \mathbb{P}(\bigcup_{i=1}^n) \leqslant \sum_{k=1}^n \mathbb{P}(A_k)
	  $$
- Soit $(\Omega, \mathcal{A}, \mathbb{P})$ un espace probabilisé et $\Omega$ fini. Si il y a équiprobabilité, alors: $$ \forall A \in \mathcal{A}, \mathbb{P}(A) = \frac{card(A)}{card(\Omega)} $$
- Soit $(\Omega, \mathcal{A}, \mathbb{P})$ un espace probabilisé, $A$ et $B$ deux évènements. L'application $\mathbb{P}_B \longmapsto \mathbb{P}_B(A)$ est une probabilité sur $\Omega$.
- Soit $(\Omega, \mathcal{A}, \mathbb{P})$ un espace probabilisé, $A$ et $B$ deux évènements indépendants. Alors $\mathbb{P}_B(A) = \mathbb{P}(A)$.