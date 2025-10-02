#Algèbre #polynome #Corps 

Dans cette section, $\mathbb{K}$ est un [[Corps]] et $\mathbb{L}$ est une [[Extension de corps]] de $\mathbb{K}$
# Définition

### Élément Algébrique

Soit $a \in \mathbb{L}$, $a$ est algébrique sur $\mathbb{K}$ si $\exists \ P \in K[X]$ un [[Polynôme]] de $\mathbb{K}$ tel que $a$ est une racine de $P$.

### Élément transcendant

Soit $a \in \mathbb{L}$, $a$ est dit transcendant sur $\mathbb{K}$ si $\forall P \in K[X], \tilde{P}(a) \neq 0$.

Dans le langage commun, un nombre transcendant est un nombre réel transcendant sur $\mathbb{Q}$.

### Polynôme minimal

Soit $a$ un élément algébrique de $\mathbb{K}$, il existe un unique polynôme unitaire de $\mathbb{K}[X]$ de degré minimum admettant pour racine $a$.

# Propriété

**Polynôme minimal**: Soit $P_a$ le polynôme minimal de $a$ dans $\mathbb{K}$
	- $\forall P \in \mathbb{K}[X] \ | \ \tilde{P}(a) = 0, P_a | P$
	- $P_a$ est irréductible dans $\mathbb{K}$
	- Toute racine de $P_a$ dans $\mathbb{L}$ admet $P_a$ comme polynôme minimal
	- Si $\mathbb{L}$ est un corps de caractéristique $0$, $a$ est une racine simple de $P_a$. On dira que $P$ est séparable