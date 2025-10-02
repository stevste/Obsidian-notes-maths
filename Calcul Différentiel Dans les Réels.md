#Analyse #Prépa 

Le calcul différentiel énonce les principes de dérivation des fonction de $\mathbb{R}$.

Dans cette section, $I$ désigne un intervalle non vide de $\mathbb{R}$. $x_0\in I$ et $f:I\longrightarrow \mathbb{R}$.

# Définition

### Taux d'accroissement

Le taux d'accroissement de $f$ en $x_0$ comme étant la fonction $\Delta_{x_0,f}$ définit par:
$$
\begin{array}{l rcl} \Delta_{x_0,f} : & I & \longrightarrow & \mathbb{R} \\
& x & \longmapsto & \dfrac{f(x)-f(x_0)}{x+x_0} \end{array}

$$
On dit que $f$ est dérivable en $x_0$ lorsque $\Delta_{x_0,f}$ admet une [[Limite]] finie.
On dit que $f$ est dérivable à droite de $x_0$ lorsque $\Delta_{x_0,f}$ admet une limite finie à droite en $x_0$ (définition analogue pour dérivabilité à gauche).

### Fonctions dérivés

- **Domaine de dérivabilité**: ensemble des points $x_0$ pour lesquelles $f$ est dérivable en $x_0$.
- **Fonction dérivé**: fonction noté $f^{'}$ qui à tout point $x$ de $I$ associe le nombre dérivé de $f$ en $x$ si il existe. Ci joint les [[Dérivés Usuelles]].
- **Fonction Dérivable**: $f$ est dérivable sur $I$ ssi $f$ est dérivable en tout point de $I$.

### Dérivées successives

Soit $f$ dérivable sur $I$. On définit les dérivées successives de $f$ par récurrence.
Soit $n \geqslant 1$ tel que $f^{(n-1)}$ est dérivable sur $I$. Alors:
$$
f^{(n)} = (f^{(n-1)})^{'}
$$

### Classe $C^n$

Soit $f$ défini sur $I$. Soit $n \in \mathbb{N}$, on dit que $f$ est de classe $C^n$ sur $I$ ssi:

- $f$ est $n$ fois dérivable sur $I$.
- $f^{(n)}$ est continue sur I.
On note $C^n(I, \mathbb{R})$ l'ensemble des fonctions de classe $C^n$ sur I. On note $C^{\infty}(I,\mathbb{R})$ l'ensemble des fonctions de classe $C^{\infty}$ sur $I$.

### Extremum

Soit $f: I \longrightarrow \mathbb{R}$, $x_0 \in I$, on dit que:
- $f$ admet un maximum local en $x_0$ si $\exists V \in V(x_0)$ tel que $\forall x \in V, f(x_0) \geqslant f(x)$.
- $f$ admet un minimum local en $x_0$ si $\exists V \in V(x_0)$ tel que $\forall x \in V, f(x_0) \leqslant f(x)$.
- $f$ admet un maximum global en $x_0$ si $\forall x \in I, f(x_0) \geqslant f(x)$.
- $f$ admet un minimum global en $x_0$ si $\forall x \in I, f(x_0) \geqslant f(x)$.
# Théorèmes

### Conditions de dérivabilités
$f$ dérivable en $x_0 \iff f$ dérivable à gauche et à droite de $x_0$.

$f$ est dérivable en $x_0$ ssi $f$ admet un [[Développement limité]] d'ordre 1 en $x_0$.

### Opération de dérivabilité
Soit $f,g: I \longrightarrow \mathbb{R}$. Si $f$ et $g$ sont dérivables en $x_0$, alors:
	1. $\lambda \in \mathbb{R}, \lambda f$ est dérivable en $x_0$ de dérivé $\lambda f^{'}$.
	2. $f+g$ est dérivable en $x_0$ de dérivé $f^{'} + g^{'}$.
	3. $fg$ est dérivable en $x_0$ de dérivé $f^{'}g + g^{'}f$.
	4. Si $g(x_0) \ne 0$, alors $\dfrac{f}{g}$ est dérivable en $x_0$ de dérivé $\dfrac{f^{'}g - g^{'}f}{g^2}$.
	5. $gof$ est dérivable en $x_0$ de dérivé $f^{'}g^{'}of$.
	6. Si $f$ est bijective et que $f^{'}$ est non nul sur $I$, alors $f^{-1}$ existe et est dérivable sur I de dérivé: $\dfrac{1}{f^{'}of^{-1}}$.

### Dérivées n-ième
Soit $f,g: I \longrightarrow \mathbb{R}$, $n \in \mathbb{N}^*$. Si $f$ et $g$ sont $n$ fois dérivables sur $I$, alors:
1. Soit $\lambda \in \mathbb{R}$, $\lambda f$ est $n$ fois dérivable sur $I$ et $(\lambda f)^{(n)} = \lambda f^{(n)}$.
2. $f+g$ est $n$ fois dérivable sur $I$ et:
   $$(f+g)^{(n)}=f^{(n)} + g^{(n)}$$
3. **Formule de Leibniz** : $fg$ est dérivable sur $I$ et:
   $$
   (fg)^{(n)} = \sum_{k=0}^{n} \begin{pmatrix} n \\ k \end{pmatrix}f^{(k)}g^{(n-k)}
   $$
4. Si $g$ ne s'annule pas sur $I$, alors $\dfrac{f}{g}$ est $n$ fois dérivable sur $I$.
5. Si $g$ est $n$ fois dérivable sur $f(I)$, si $f$ est $n$ fois dérivable sur $I$, alors $gof$ est $n$ fois dérivable sur $I$.

### Théorème d'annulation de la dérivé
Si $f$ est dérivable sur $I$, et si $f$ admet un extremum en $x_0$, alors $f^{'}(x_0) = 0$

### Théorème de Rolle
Soit $(a, b) \in \mathbb{R}^2$ tel que $a < b$ et $f : [a,b] \longrightarrow \mathbb{R}$. Supposons que:
1. $f$ est continue sur $[a,b]$ et dérivable sur $]a,b[$
2. $f(a) = f(b)$
Alors $\exists c \in ]a,b[$ tel que $f^{'}(c) = 0$

### Théorème des accroissements fini
Soit $(a, b) \in \mathbb{R}^2$ tel que $a < b$ et $f : [a,b] \longrightarrow \mathbb{R}$. On suppose $f$ continue sur $[a,b]$ et dérivable sur $]a,b[$. Alors $\exists c \in ]a,b[$ tel que
$$
f^{'}(c) = \dfrac{f(a)-f(b)}{a-b}
$$
**Corollaire**: Si $\exists (m,M) \in \mathbb{R}^2$ tel que $f^{'}(]a,c[) = [m,M]$, alors: 
$$
m(b-a) \leqslant f(b)-f(a) \leqslant M(b-a)
$$

### Variation des fonctions
Soit $(a,b) \in \mathbb{R}^2, a < b$ et $f$ continue sur $[a,b]$ et dérivable sur $]a,b[$. Alors:
- $f$ est croissante sur $[a,b] \iff \forall x \in ]a,b[, f^{'}(x) > 0$.
- $f$ est décroissante sur $[a,b] \iff \forall x \in ]a,b[, f^{'}(x) < 0$.

### Théorème du prolongement de la dérivé
Soit $(a,b) \in \mathbb{R}^2, a < b$, soit $x_0 \in ]a,b[$ et soit $f$ continue sur $[a,b]$ et dérivable sur $]a,b[ \setminus {x_0}$. Alors:
- Si $\lim_{x \to x_0^+} f^{'}(x) = l \in \mathbb{R}$ , alors $f$ est dérivable à droite en $x_0$ (homologue pour dérivé à gauche).
- Si $\lim_{x \to x_0} f^{'}(x) = l \in \mathbb{R}$ , alors $f$ est dérivable en $x_0$ et $f^{'}(x_0) = l$.
- Si $\lim_{x \to x_0} = \infty$, alors $f$ n'est pas dérivable en $x_0$.