#Algèbre #EspaceVectoriel #Prépa 

Dans cette note, $E$ et $F$ sont des abréviations des $\mathbb{K}$-ev $(E, +, \cdot)$ et $(F, \oplus, \odot)$.
# Définition

### Applications linéaires

Soient $(E, +, \cdot)$ et $(F, \oplus, \odot)$ deux $\mathbb{K}$-[[Espace Vectoriel]] et $f: E \longrightarrow F$ une application. on dit que $f$ est une application linéaire si:
$$
\forall(x, y) \in E^{2}, \forall \lambda \in \mathbb{K}, f(\lambda \cdot x + y) = \lambda \odot f(x) \oplus f(y)
$$
Il s'agit de l'équivalent d'un [[Morphisme]] pour les espaces vectoriels.
### Ensemble d'application

On note $\mathcal{L}(E, F)$ l'ensemble des applications linéaires de $E$ vers $F$.
On note $\mathcal{L}(E)$ l'ensemble des endomorphismes de $E$.
On note $\mathcal{G}\mathcal{L}(E)$ l'ensemble des automorphismes de $E$.
On note $E^{*}$ l'ensemble des formes linéaires de $E$ appelé le **dual** de $E$.
### Forme linéaires

On appelle forme linéaire de $E$ toute application linéaire de $E$ vers $\mathbb{K}$.
### Noyau

Soit $f \in \mathcal{L}(E, F)$, on définit le noyau de de $f$ comme l'ensemble des éléments de $E$ don l'image par $f$ est 0:
$$
\text{Ker}(f) = f^{-1}(\{0_{F\})}= \{x \in E | f(x) = 0\}
$$
### Image

Soit $A \subseteq E$ et $f \in \mathcal{L}(E, F)$. on définit l'image de $A$ par $f$ comme l'ensemble des images d'éléments de $A$ par $f$:Im
$$
f(A) = \{ y \in F | \exists x \in A, f(x) = y \} = \{ f(x) | x \in A \}
$$

On la note aussi $\text{Im}(f)$ si $A = E$.
### Image réciproque

Soient $B \in F, f \in \mathcal{L}(E, F)$. on définit l'image réciproque de $B$ par $f$ comme l'ensemble des antécédents de $B$ dans $E$:
$$
f^{-1}(B) = \{ x \in E | f(x) \in B \}
$$
### Rang d'une application

Soit $f \in \mathcal{L}(E, F)$ tel que $\text{Im}(f)$ est de dimension fini. On appelle rang de l'application $f$ la dimension de $\text{Im}(f)$ noté $\text{rg}(f)$.
### Hyperplan

On appelle hyperplan de $E$ le noyau d'une forme linéaire non nulle sur $E$.
Si on note $H = \text{Ker}(f)$ un hyperplan de $E$, alors on dit de $f(x) = 0$ qu'elle est **l'équation de l'hyperplan**.
# Théorèmes

### Structure de l'espace des applications

$\mathcal{L}(E, F)$ est un $\mathbb{K}$-sev de $(F^{E}, +, \cdot)$.
$(\mathcal{L}(E, F), +, \circ)$ est un [[Anneau]] non commutatif et non intègre.
$(\mathcal{L}(E, F), +, \cdot, \circ)$ est un $\mathbb{K}$-[[Algèbre]] non commutatif et non intègre.
$(\mathcal{G}\mathcal{L}(E, F), \circ)$ est un [[Groupe]] non commutatif. On le nomme **Groupe linéaire**.
### Théorème du rang

Soit $E, F$ deux $\mathbb{K}$-ev tel que $E$ est de dimension finie, soit $f \in \mathcal{L}(E, F)$. Alors on a:
$$
\text{Dim}(E) = \text{Dim}(\text{Ker}(f)) + \text{rg}(f).
$$
### Corollaire du théorème du rang

Si $\text{Dim}(E) = \text{Dim}(F)$ et sont de dimension finie, alors on a:
$$
f \ \text{bijective} \Leftrightarrow f \ \text{surjective} \Leftrightarrow f \ \text{bijective}
$$
### Changement de base

Soient $E$ et $F$ deux $\mathbb{K}$-ev de dimension finie $n$. Soit $B = (e_{1}, \dots, e_n)$ une base de $E$. Pour toute famille de $n$ vecteurs de $F$, $(b_{1}, \dots, b_n$). Il existe une unique application de $E$ vers $F$ tel que:
$$
\forall i \in [\![1, n]\!], f(e_i) = b_i
$$
# Propriétés

- Soit $f \in \mathcal{L}(E, F)$, on a $f(0_{E)}= 0_F$. 
- Soient $f \in \mathcal{L}(E, F)$ et $g \in \mathcal{L}(F, G)$, alors $g \circ f \in \mathcal{L}(E, G)$.
- Soient $f_{1}, f_{2} \in \mathcal{L}(E, F)$ et $g \in \mathcal{L}(F, G)$, alors $g \circ (f_{1} + f_{2}) = g \circ f_{1} + g \circ f_{2}$. (faux si $g$ est non linéaire).
- Soit $f \in \mathcal{L}(E, F)$. Si $A$ est un $\mathbb{K}$-sev de $E$, alors $f(A)$ est un $\mathbb{K}$-sev de $E$.
- Soit $f \in \mathcal{L}(E, F)$, alors $\text{Ker}(f)$ est un $\mathbb{K}$-sev de $E$.
- Soit $f \in \mathcal{L}(E, F), B \in F$. Si $B$ est un $\mathbb{K}$-sev de $F$, alors $f^{-1}(B)$ est un $\mathbb{K}$-sev de $E$.
- Soit $f \in \mathcal{L}(E, F)$, alors $\text{Im}(F)$ est un $\mathbb{K}$-sev de $E$.
- Soit $f \in \mathcal{L}(E, F)$:
	- $f$ est injective $\Leftrightarrow \text{Ker}(f) = \{0_F\}$
	- $f$ est surjective $\Leftrightarrow \text{Im}(f) = F$.
- Soit $f \in \mathcal{L}(E, F)$, alors l'image d'une famille génératrice de $E$ est une famille génératrice de $F$.
- Soit $f \in \mathcal{L}(E, F)$ injective, alors l'image d'une famille libre de $E$ est une famille libre de $F$.
- Soit $f \in \mathcal{L}(E, F)$ $E$ de dimension $n$ et $(e_{1,}\dots, e_n)$ une base de $E$:
	- $f$ injective $\Leftrightarrow$ $(f(e_i)_{i\in[[1, n]]})$ est une famille libre de $F$.
	- $f$ surjective $\Leftrightarrow$ $(f(e_i)_{i\in[[1, n]]})$ est une famille génératrice de $F$.
	- $f$ bijective $\Leftrightarrow$ $(f(e_i)_{i\in[[1, n]]})$ est une base de $F$.
- Soit $E = \mathbb{K}^{p}$ et $f \in E^{*}$, Alors $\exists (a_{1}, \dots, a_{n}) \in \mathbb{K}^{p} | \forall (x_{1}, \dots x_{n}) \in \mathbb{K}^{p}, f(x_{1}, \dots x_{p}) = \sum_{i=1}^{p} a_{i}x_{i}$.