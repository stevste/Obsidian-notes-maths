#Probabilité #Prépa 

Dans ce chapitres, $\Omega$ désigne un univers, $\mathcal{A}$ une tribu, $\mathbb{P}$ une probabilité et $(\Omega, \mathcal{A}, \mathbb{P})$ un espace probabilisé (cf [[Fondement de probabilité]])
# Définition

### Moyenne empirique

On considère une suite de [[Variables Aléatoires]] $(X_i)_{i \in \mathbb{N}, i > 0}$ indépendantes de même loi, on appelle moyenne empirique d'ordre $n$ la variable aléatoire définit par:
$$
\overline{X_n} = \frac{1}{n}\sum_{i = 1}^n X_i
$$
### Convergence en probabilité

Soient $(\Omega, \mathcal{A}, \mathbb{P})$, $(X_i)_{i \in \mathbb{N}, i > 0}$ une suite de VA et $X$ une VA.
On dit que $(X_i)_{i \in \mathbb{N}, i > 0}$ converge en probabilité vers $X$ ssi:
$$
\forall \alpha > 0, \lim_{n \to +\infty} \mathbb{P}(|X_n - X| > \alpha) = 0
$$
### Convergence en loi

Soient $(\Omega, \mathcal{A}, \mathbb{P})$,  une suite de VA et  une VA de fonction de répartition respectives $F_{X_n}$ et $F_X$.
On dit que $(X_i)_{i \in \mathbb{N}, i > 0}$ converge en loi vers $X$ en tout point où $F_X$ est continue ssi:
$$
\forall t \in \mathbb{R}, \lim_{n \to + \infty} F_{X_n}(t) = F_X(t)
$$
On le note $X_n \xrightarrow{\text{loi}} X$
# Théorèmes

### Inégalité de Bienaymé-Tchebychev

Soit $X$ une VA d'espérance $\mathbb{E}(X)$ finie de variance $\mathbb{V}(X)$ finie, on a alors:
$$
\forall \epsilon > 0, \mathbb{P}(|X - \mathbb{E}(X)| \geqslant \epsilon) \leqslant \frac{\mathbb{V}(X)}{\epsilon^2}
$$
### Loi faible des grands nombre

Soient $n \in \mathbb{N}$ et $(X_i)_{i \in \mathbb{N}, i > 0}$ une suite de variable aléatoire indépendantes de même loi admettant un moment d'ordre 2 et une même espérance $m$, on a alors:
$$
\forall \epsilon > 0, \lim_{n \to +\infty} \mathbb{P}(|\overline{X_n} - m| \geqslant \epsilon) = 0
$$
### Théorème central limite

 une suite de variable aléatoire indépendantes de même loi admettant une espérence $m$ et une variance $\sigma^2$, alors:
$$
\frac{\overline{X_n} - m}{\frac{\sigma}{\sqrt{n}}} \xrightarrow{\text{loi}} \mathcal{N}(0; 1)
$$
# Propriétés

- Inégalité de Markov: Soit $X$ une VA positive d'espérance $\mathbb{E}(X)$, on a: $\forall t > 0, \mathbb{P}(X \geqslant t) \leqslant \frac{\mathbb{E}(X)}{t}$.
- Soit $(X_i)_{i \in \mathbb{N}, i > 0}$ une suite de variable aléatoire indépendantes de même loi d' espérance $m$ et de variance $\sigma^2$, alors:
	- $\mathbb{E}(\overline{X_n}) = m$
	- $\mathbb{V}(\overline{X_n}) = \frac{\sigma^2}{n}$
	- $\sigma(\overline{X_n}) = \frac{\sigma}{\sqrt{n}}$
- Soit $(\Omega, \mathcal{A}, \mathbb{P})$, $(X_n)_{n\in \mathbb{N}}$ une suite de VA discrète et $X$ une VA discrète telle que: $\forall n \in \mathbb{N}, X_n(\Omega) \subset \mathbb{N}$ et $X(\Omega) \subset \mathbb{N}$, alors: $X_n \xrightarrow{\text{loi}} X \Leftrightarrow \forall k \in \mathbb{N}, \lim_{n \to +\infty} \mathbb{P}(X_n = k) = \mathbb{P}(X = k)$.