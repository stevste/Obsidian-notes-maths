#Probabilité #Prépa 

Dans ce chapitres, $\Omega$ désigne un univers, $\mathcal{A}$ une tribu, $\mathbb{P}$ une probabilité et $(\Omega, \mathcal{A}, \mathbb{P})$ un espace probabilisé (cf [[Fondement de probabilité]])

# Définition

### Variable aléatoire

- On appelle variable aléatoire réel (abrégé VA) toute application: $$
\begin{array}{l rcl} X : & \Omega & \longrightarrow & \mathbb{R} \\
& \omega & \longmapsto & X(\omega) \end{array}
$$
- On note $X(\Omega)$ l'ensemble des valeurs prises par $X$.
- La VA $X$ est dites discrète si $X(\Omega)$ est un ensemble dénombrable de $\mathbb{R}$.
- La VA $X$ est dites finie si $X(\Omega)$ est un ensemble finie
### Loi de probabilité

On appelle loi de probabilité (ou distribution de probabilité) d'une VA $X$ l'application $\mathbb{P}_X$ telle que:
$$
\begin{array}{l rcl} \mathbb{P}_X : & \mathcal{A} & \longrightarrow & [0, 1] \\
& A & \longmapsto & \mathbb{P}(X^{-1}(A)) \end{array}
$$
L'application $\mathbb{P}_X$ est une probabilité sur l'espace probabilisable $(R, \mathcal{B})$ avec $\mathcal{B}$ une tribu de $\mathbb{R}$.
Ensemble de [[Lois de probabilités usuelles]].
### Fonction de répartition

On appelle fonction de répartition de $X$ l'application $F_X$ telle que:
$$
\begin{array}{l rcl} F_X : & \mathbb{R} & \longrightarrow & \mathbb{R} \\
& x & \longmapsto & \mathbb{P}(X \leqslant x) \end{array}
$$
### Variable aléatoire discrète

Une VA $X$ est dite discrète si $X(\Omega)$ est fini ou dénombrable.
Déterminer la loi de probabilité de $X$, c'est donner $X(\Omega)$ et $\forall x \in X(\Omega), p_x = \mathbb{P}(X = x)$.
#### Moment d'une Variable discrète

Soit $X$ une VA discrète. Soit $q \in \mathbb{N}, q > 0$. On dit que la variable $X$ admet moment d'ordre $q$ si la [[Série Numérique]] $\sum_{i \in I} (x_i)^q \mathbb{P}(X = x_i)$ converge absolument.
On note $m_q(X)$ la somme de la série que l'on appelle le moment d'ordre $q$ de $X$.
$$
m_q(X) = \sum_{i \in I} (x_i)^q \mathbb{P}(X = x_i)
$$
#### Espérance mathématique

Soit $X$ un VA discrète, on appelle espérance mathématique de $X$ le réel $\mathbb{E}(X)$ définit par:
- Pour $X(\Omega) = \{x_1; \dots ; x_n\}$ fini: $$ \mathbb{E}(X) = \sum_{i = 1}^n x_i \mathbb{P}(X = x_i) $$
- Si $X(\Omega) = I$, I espace dénombrable non fini: $$  \mathbb{E}(X) = \sum_{i \in I} x_i \mathbb{P}(X = x_i)  $$
#### Variance et écart type

Soit $X$ une VA réel. Si $X$ admet un moment d'ordre 1 et d'ordre 2 alors on définit:
- La variance de $X: \mathbb{V} = \mathbb{E}[(X - \mathbb{E}(X))^2]$.
- L'écart type de $X : \sigma(X) = \sqrt{\mathbb{V}(X)}$
### Variable à densité

Soit $X$ une variable aléatoire réelle. On dit que $X$ est une variable à densité ou que $X$ admet une densité $f$ si sa fonction de répartition $F_X$ est continue et peu s'écrire sous la forme: $\forall x \in \mathbb{R}, F_X(x) = \int_{-\infty}^x f(t) \, \mathrm{d}t$. avec:
- $\forall x \in \mathbb{R}, f(x) \geqslant 0$
- $f$ est continue par morceaux sur $\mathbb{R}$
- $\int_{-\infty}^{+\infty} f(t) \, \mathrm{d}t = 1$
La fonction $f$ est appelé densité de $X$.
#### Espérance

Soit $X$ une VA de densité $f$ telle que $\int_{-\infty}^{+\infty} tf(t) \, \mathrm{d}t$ soit absolument convergente. On appelle espérance de $X$, notée $\mathbb{E}(X)$, le réel:
$$
\mathbb{E}(X) = \int_{-\infty}^{+\infty} tf(t)\mathrm \,{d}t
$$
#### Moment d'une Variable à densité

Soit $q \in \mathbb{N}, q > 0$. Soit  une VA de densité $f$. On dit que la variable $X$ admet moment d'ordre $q$ si l' [[Intégrale Généralisé]] $\int_{-\infty}^{+\infty} t^qf(t) \, \mathrm{d}t$ converge absolument.
On note $m_q(X)$ le réel appelé moment d'ordre $q$:
$$
m_q(X) = \int_{-\infty}^{+\infty} t^qf(t) \, \mathrm{d}t
$$
#### Variance et écart type

Soit $X$ une variable aléatoire de densité $f$ admettant un moment d'ordre 2, alors on définit:
- La variance de $X$, le nombre réel $\mathbb{V}(X) = \mathbb{E}[(X - \mathbb{E}(X))^2] = \int_{-\infty}^{+\infty}(t - \mathbb{E}(X))^2f(t) \, \mathrm{d}t$.
- L'écart-type de $X$, le nombre réel $\sigma(X) = \sqrt{\mathbb{V}(X)}$
# Théorème

### Théorème de transfert pour variable discrète

Soit $f: \mathbb{R} \longrightarrow \mathbb{R}$ telle que la série $\sum_{i \in E} f(x_i)\mathbb{P}(X = x_i)$ converge absolument, alors $f(X)$ admet une espérance et on a:
$$
\mathbb{E}(f(X)) = \sum_{i \in I} f(x_i)\mathbb{P}(X = x_i)
$$
### Théorème de transfert pour variable à densité

soit $X$ une VA de densité $f$ et $\Phi : \mathbb{R} \longrightarrow \mathbb{R}$ telle que $|\Phi|f$ soit intégrable sur $\mathbb{R}$, alors $\Phi(X)$ admet une espérance et:
$$
\mathbb{E}(X) = \int_{-\infty}^{+\infty} \Phi(t)f(t) \, \mathrm{d}t
$$
# Propositions

- Soit l'espace probabilisé $(\Omega, \mathcal{A}, \mathbb{P})$ et $X$ un VA de fonction de répartition $F_X$. Alors:
	- $F_X$ est croissante
	- $\lim_{x \to -\infty} F_X(x) = 0$ et $\lim_{x \to +\infty} F_X(x) = 1$
	- $F_X$ est continue à droite en tout point de $\mathbb{R}$
	- $F_X$ à une limite à gauche en tout point de $\mathbb{R}$
- Soit $X$ une VA discrète telle que $X(\Omega) = \{x_i\}_{i\in I} avec I \in \mathbb{N}$. Alors la famille d'évènement $(\{X = x_i\}_{i \in I})$ forme un système complet d'évènements. On en déduit que: $\sum_{i \in I} \mathbb{P}(X = x_i) = 1$.
- Soient $X$ et $Y$ des VA admettant chacune une espérance. Soit $(a,b)\in \mathbb{R}^2$.
	- Linéarité de l'espérance: $\mathbb{E}(aX + Y + b) = a\mathbb{E}(X) + \mathbb{E}(Y) + b$
	- Positivité de l'espérance: $X \geqslant 0 \Rightarrow \mathbb{E} \geqslant 0$.
- Formule de Koening-Huygens: $\mathbb{V} = \mathbb{E}(X^2) - \mathbb{E}(X)^2$.
- Soit $X$ une VA admettant une variance, soit $(a, b) \in \mathbb{R}$:
	- $\mathbb{V}(aX + b) = a^2\mathbb{V}(X)$
	- $\sigma(aX + b) = |a|\sigma(X)$
- Soit $f$ une densité de répartition $F_X$, en tout $x_0$ point où $f$ est continue, $F_X$ est dérivable et on a: $F_X'(x_0) = f(x_0)$
- Une fonction $f$ définie sur $\mathbb{R}$ est une densité de probabilité ssi:
	- $\forall x \in \mathbb{R}, f(x) \geqslant 0$
	- $f$ est continue par morceau sur $\mathbb{R}$
	- $\int_{-\infty}^{+\infty} f(t) \, \mathrm{d}t = 1$
- Si $X$ est une variable aléatoire à densité, alors on a: $\forall(a;b) \in \mathbb{R}^2, a \leqslant b$:
	- $\mathbb{P}(X \leqslant b) = \int_{-\infty}^b f(t) \mathrm{d}t = F_X(b)$
	- $\mathbb{P}(a \leqslant X \leqslant b) = \int_a^b f(t) \mathrm{d}t = F_X(b) - F_X(a)$
	- $\mathbb{P}(X = a) = \mathbb{P}(X = b) = 0$
	- $\mathbb{P}(a < X \leqslant b) = \mathbb{P}(a \leqslant X \leqslant b) = \mathbb{P}(a \leqslant X < b) = \mathbb{P}(a < X < b)$
- Soit $(p, q) \in \mathbb{N}^2, p > 0, q > 0$ et $p < q$. Soit $X$ une VA de densité $f$ admettant un moment d'ordre $q$, alors $X$ admet également un moment d'ordre $p$.