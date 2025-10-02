#Analyse #Prépa 

Les développements limités sont utilisés pour approcher des fonctions au voisinage d'un point à l'aide de fonctions polynomiales. C'est une technique de calcul très puissante permettant de trouvé des équivalents de fonctions au voisinage d'un point ou dans le calcul de limite. Ils sont une application direct des [[Formules de Taylor]].

# Définition

### Développement limité

Soit $f: I \longrightarrow \mathbb{R}$ et $x_0$ un point adhérent à I, $f$ possède un DL en $x_0$ à l'ordre $n$ si il existe un [[Polynôme]] $P \in \mathbb{R}_{n[X]}$ tel que:
$$
f(x)=_{x_0} P(x-x_0) + o((x-x_0)^n)
$$
$P$ est appelé la partie principal du développement limité, noté $DL_n(x_0)$ 

### Développement asymptotique

Soit $f: I \longrightarrow \mathbb{R}$. Si $f$ admet une limite finie en $+\infty$, alors elle admet un développement asymptotique (ou développement limité en $+\infty$) ssi $\exists (a_i)_{i \in [1;n]}$ tel que:
$$
f(x)=_{+\infty} \sum_{k=0}^n\dfrac{a_k}{x^k} + o(\dfrac{1}{x^n})
$$

### Asymptote

On dit que la courbe $C_g$ d'équation $y = g(x)$ est asymptote en $x_0$ à $C_f$ d'équation $y = f(x)$ ssi:
$$
\lim_{x \rightarrow x_0} f(x)-g(x) = 0
$$
# Propriétés

1. La partie principal d'un DL est unique.
   
2. Soit $f$ une fonction qui possède un $DL_n(0)$, alors:
	1. Si $f$ est pair, alors ses coefficients d'indices impair sont nuls.
	2. Si $f$ est impair, alors ses coefficients d'indices pair sont nuls.

3. Soit $f$ une fonction qui possède un $DL_0(x_0)$, alors:
	1. Si $f$ est défini en $x_0$, alors elle est continue en $x_0$.
	2. Si $f$ n'est pas défini en $x_0$, alors $f$ est prolongeable pas continuité en $x_0$.

 4. Si $f$ possède un $DL_1(x_0)$, alors elle est dérivable en $x_0$ (non vrai pour une dérivé d'ordre supérieure).

 5. Si $f$ possède un $DL_n(x_0)$, alors elle admet un équivalent en $x_0$. Il s'agit du premier terme non nul du DL.

 6. Soit $f$ une fonction admettant un $DL_k(x_0)$ tel que $k>1, a_k \ne 0$:
$$
f(x) =_{x_0} f(x_0) + a_1(x-x_0) + a_k(x-x_0)^k + o((x-x_0)^k)
$$
	 Alors la tangente de $f$ en $x_0$ est la droite d'équation $y=f(x_0) + a_1(x-x_0)$. La position relative de la tangente par rapport à la courbe dépend du signe de $f(x)-y$ ou du signe de $a_k(x-x_0)^k$.
# Opérations

1. Si $f$ admet un $DL_n(x_0)$, alors $\lambda f$ admet aussi un $DL_n(x_0)$. La partie principal de ce DL est le produit de celle de $f$ par $\lambda$.

2. Si $f$ admet un $DL_n(x_0)$, et $g$ un $DL_p(x_0)$, alors:
	- $f+g$ admet un $DL_n(x_0)$. La partie principal de ce DL est la somme des deux parties principales de $f$ et $g$ avec uniquement les termes non négligeables devant $(x-x_0)^{min(n, p)}$.
	   
	- $fg$ admet un $DL_n(x_0)$. La partie principal de ce DL est le produit des deux parties principales de $f$ et $g$ avec uniquement les termes non négligeables devant $(x-x_0)^{min(n, p)}$.
	   
	- Si $g(x_0) \ne 0$ et que $f$ et $g$ admettent un $DL_n(x_0)$, alors $\dfrac{f}{g}$ admet un $DL_n(x_0)$. La partie principal de ce DL est obtenue par division euclidienne des deux parties principales avec uniquement les termes non négligeables devant $(x-x_0)^n$.
	   
	- $gof$ admet un $DL_n(x_0)$. La partie principal de ce DL est obtenue par composition des deux parties principales avec uniquement les termes non négligeables devant $(x-x_0)^{min(n, p)}$.

3. Soit $f: ]a;b[ \longrightarrow \mathbb{R}$ une fonction de classe $C^1$ sur $]a;b[$.
   Si $f^{'}$ admet un $DL_n(x_0)$, alors $f$ admet un $DL_{n+1}(x_0)$, de partie principal égal à la primitive de celle de $f{'}$.

4. Soit $f$ possédant un $DL_n(x_0)$, si $f{'}$ admet un $DL_{n-1}(x_0)$, alors sa partie principal est la dérivé de celle de $f$.