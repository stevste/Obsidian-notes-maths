#Groupe #Algèbre #Prépa 
# Définition

### Morphisme de groupe

Soient $(G_1, \oplus)$, $(G_2, \otimes)$ deux [[Groupe]]s. Soit $\phi : G_1 \rightarrow G_2$ une [[Application]]. On dit que $\phi$ est un [[Morphisme]] de groupe ssi : $\forall x \in G_1, \phi(x \oplus y) = \phi(x) \otimes \phi(y)$.

### Noyau et Image

- $Ker(\phi) = \{x \in G_1 \ | \ \phi(x) = e_{G_2}\}$
- $Im(\phi) = \{y \in G_2 \ | \ \exists x \in G_1 \ | \ \phi(x) = y\}$
# Proposition

- Soit $\phi: G_1 \rightarrow G_2$ un morphisme de groupes, alors:
	- $\phi(e_{G_1}) = e_{G_2}$
	- $\forall x \in G_1, \phi(x)^{-1} = \phi(x^{-1})$
- $Ker(\phi)$ et $Im(\phi)$ sont des sous groupes de $G_1$ et $G_2$ respectivement
- $\phi$ est surjective $\Leftrightarrow Im(\phi) = G_2$
- $\phi$ est injective $\Leftrightarrow Ker(\phi) = \{e_{G_1}\}$