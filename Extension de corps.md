#Algèbre #Corps 

Dans cette section, $\mathbb{K}$ et $\mathbb{L}$ désignes des [[Corps]]
# Définition

### Extension de corps

On dit que $\mathbb{L}$ est une extension de $\mathbb{K}$ si $\mathbb{K}$ est un sous corps de $\mathbb{L}$.

Plus généralement, une extension de $\mathbb{K}$ est un couple $(L,i)$ où $i : \mathbb{K} \rightarrow \mathbb{L}$ est un [[Morphisme d'anneau]] unitaire injectif entre deux corps.

### Degré d'une extension

Soit $\mathbb{L}$ une extension de $\mathbb{K}$, la dimension de $\mathbb{L}$ comme $\mathbb{K}$-Espace vectoriel est appelé degré de l'extension $\mathbb{L}$ sur $\mathbb{K}$ et noté $[\mathbb{L} : \mathbb{K}]$. L'extension $\mathbb{L}$ est dite de degré fini de $\mathbb{K}$ si $[\mathbb{L} : \mathbb{K}]$ est fini.

### Extension engendré

Soit $\mathbb{L}$ une extension de $\mathbb{K}$, et $A \subset \mathbb{L}$:
Il existe une extension de $\mathbb{K}$ noté $\mathbb{K}(A)$ et minimum pour la relation d'inclusion entre les extension de $\mathbb{K}$ contenues dans $\mathbb{L}$
### Tour de corps

Soient $(\mathbb{K}_i)_{i \in \mathbb{N}^*}$ une suite finis de corps, on appelle tour de corps l'extension $\mathbb{K}_0$ tel que $\mathbb{K}_0 = \ \subset_{r \in [\![1, i]\!]} \mathbb{K}_r$.
# Proposition

- Une extension $\mathbb{L}$ de $\mathbb{K}$ est munie d'une structure de $\mathbb{K}$-[[Espace Vectoriel]] et de $\mathbb{K}$-[[Algèbre]]
- Soit $\mathbb{L}$ une extension de degré fini de $\mathbb{K}$, $\mathbb{M}$ une extension de degré fini de $\mathbb{L}$. Alors $[\mathbb{M} : \mathbb{K}] = [\mathbb{M} : \mathbb{L}][\mathbb{L} : \mathbb{K}]$.
- $\mathbb{K}(A)$ est égal à l'ensemble $E$ des éléments de $\mathbb{L}$ de la forme $\dfrac{S(a_1, ... , a_k)}{T(a_1, ... , a_k)}$. avec $(a_k)_{k \in \mathbb{N}}$ des éléments de $A$ et $\dfrac{S}{T}$ un [[Fraction Rationnelle]] du corps de fractions rationnelles de $K(X_1, ... , X_k)$ et $T(a_1, ... , a_k) \neq 0$.
- $K(A \cup B) = K(A)(B)$