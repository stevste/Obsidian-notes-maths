#Algèbre #Analyse #Prépa #polynome 
# Définition

### Diviseur

Soient $(P,Q) \in \mathbb{K}[X]^2$ des [[Polynôme]]s, On dit que $P$ divise $Q$ ssi $\exists A \in \mathbb{K}[X]$ tel que $Q = AP$. On note alors $P$ | $Q$ et $P$ est un diviseur de $Q$.
### Division Euclidienne
Soient $(P, B) \in \mathbb{K}[X]^2, \; \exists! (Q,R) \in \mathbb{K}[X]^2$ tel que deg($R$) $<$ deg($Q$) et:
$$
P = BQ + R
$$
$Q$ est le quotient de la division euclidienne de $P$ par $B$ et $R$ est le reste.

Pour les divisions non euclidiennes, voir [[Fraction Rationnelle]]

### Polynôme irréductible
On dit que $P$ est irréductible dans $\mathbb{K}$ si:
- deg($P$) $\geqslant 1$
- Les seuls diviseurs de $P$ sont des polynôme constants ou du type $\lambda P$ avec $\lambda \in \mathbb{K}$
### PGCD de polynômes

Soit $(P,Q) \in \mathbb{K}[X]^2$. Le PGCD de $P$ et $Q$ est l'unique polynôme unitaire, de degré maximal, qui divise à la fois $P$ et $Q$. On le note $pgcd(P,Q)$ ou $P \wedge Q$.
# Théorème

### Théorème de Gauss

Soient $P, A, B$ des polynômes de $\mathbb{K}[X]$, si $P|AB$ et $P \wedge A = 1$, alors $P|B$
# Propriété

- $B|A$ ssi le reste de la division euclidienne de $A$ par $B$ est nul.
- Tout polynôme de degré 1 est irréductible dans $\mathbb{K}$.
- Si $A|C$ et $B|C$ et $A \wedge B = 1$, alors $AB|C$