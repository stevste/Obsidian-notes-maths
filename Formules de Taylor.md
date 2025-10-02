#Formules #Analyse #Prépa 

Les formules de Taylor sont issues d'une généralisation du théorème des accroissements finis (Cf [[Calcul Différentiel Dans les Réels]]). Elles sont à l'origine des [[Développement limité]].
## I. Formule de Taylor-Lagrange

Soient $n \in \mathbb{N}$ , $(a,b) \in \mathbb{R}^2$,et $f  \in C^n(I,\mathbb{R})$ sur $[a;b]$ tel que $f^{(n)}$ est dérivable sur $]a;b[$ . Alors Il existe $c \in ]a;b[$ tel que:
$$
f(b) = f(a) + \sum_{k=0}^n(\dfrac{(b-a)^k}{k!}f^{(k)}(a)) + \dfrac{(b-a)^{n+1}}{(n+1)!}f^{(n+1)}(c)
$$
## II. Inégalité de Taylor-Lagrange

Il s'agit d'un corollaire de la formule précédente. On reprend les mêmes hypothèses que pour la formule de Taylor Lagrange en supposant que $f^{(n+1)}$ est majoré par M. On a alors:
$$
f(b) - |(f(a) + \sum_{k=1}^n(\dfrac{(b-a)^k}{k!})| \leq \dfrac{(b-a)^{n+1}}{(n+1)!}M

$$
## III. Formule de Taylor-Young

Soient $n \in \mathbb{N}^{*}$ et $x_0 \in \mathbb{R}$ , Soit $I \subset \mathbb{R}$ tel que $x_0 \in I$ . Soit $f \in C^{n-1}(I,\mathbb{R})$ et $f^{(n)}(x_0)$ existe. Alors on a:
$$
f(x) =_{x_0} \sum_{k=0}^{n}(\dfrac{f^{(k)}(x_0)}{k!}(x-x_0)^k) +o((x-x_0)^n)
$$

