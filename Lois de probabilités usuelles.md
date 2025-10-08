#Probabilité #Prépa #Formules 

# Lois discrètes

## Loi uniforme

#### Contexte

Expérience consistant à extraire une unité dans un ensemble de $N$ éléments au hasard avec la même chance de choisir n'import quel éléments.
#### Probabilité:

Soient $n \in \mathbb{N}, n > 0$ et $k \in [\![1, n]\!]$, $\mathbb{P}(X = i) = \frac{1}{n}$.
#### Espérance

$$\mathbb{E}(X) = \frac{n+1}{2}$$
#### Variance
$$\mathbb{V}(X) = \frac{n^2-1}{12}$$
## Loi de Bernoulli

#### Contexte

Expérience où la variable ne prend que deux valeurs: 1 pour un succès et 0 pour un échec. Le paramètre $p$ représente la probabilité de succès.
#### Probabilité:

$$
\begin{array}{c}
X \rightsquigarrow B(p) \\
X(\Omega) = \{0; 1\} \\
\mathbb{P}(X = 0) =) 1 - p, \mathbb{P}(X = 1) = p
\end{array}
$$
#### Espérance

$$
\mathbb{E}(X) = p
$$
#### Variance
$$
\mathbb{V}(X) = p(1-p)
$$
#### Convergence (Théorème de Moivre Laplace)

Soit $(X_{n})$ une suite de VA indépendantes suivant une loi de Bernoulli de paramètre $p$, soit$S_{n}= \sum_{i=1}^{n}X_{i}$.
Alors $\frac{S_{n} - np}{\sqrt{np(1-p)}} \xrightarrow{\text{loi}} \mathcal{N}(0, 1)$.
## Loi binomiale

#### Contexte

Expérience où on répète $n$ fois une expérience de Bernoulli. La variable comptabilise le nombre de succès dans les $n$ expérience.
#### Probabilité:

$$\begin{array}{c}
X \rightsquigarrow B(n,p) \\
X(\Omega) = [\![0, n]\!] \\
\forall k \in X(\Omega), \,\mathbb{P}(X = k) = \begin{pmatrix} n \\ k \end{pmatrix} p^k(a-p)^{n-k}
\end{array}$$
#### Espérance

$$
\mathbb{E}(X) = np
$$
#### Variance
$$
\mathbb{V}(X) = np(1-p)
$$
#### Convergence

Si $n \geqslant 30, p \leqslant 0.1, np \leqslant 15$, alors la variable $Y \rightsquigarrow \mathcal{P}(np)$ est une bonne approximation de $X$
## Loi géométrique

#### Contexte

Donne le nombre de tentative nécessaire avant d'obtenir un premier succès pour une répétition d'un nombre élevé d'évènements indépendants.
#### Probabilité:

$$\begin{array}{c}
X \rightsquigarrow \mathcal{G}(p) \\
X(\Omega) = \mathbb{N} \setminus 0 \\
\forall k \in X(\Omega), \,\mathbb{P}(X = k) = p(1-p)^k-1
\end{array}$$
#### Espérance

$$
\mathbb{E}(X) = \frac{1}{p}
$$
#### Variance
$$
\mathbb{V}(X) = \frac{1-p}{p^2}
$$
## loi de Poisson

#### Contexte

Modélise les phénomènes rares, équivalent d'une loi binomiale pour une probabilité de succès faible et un très grand nombre d'évènement
#### Probabilité:

$$\begin{array}{c}
X \rightsquigarrow \mathcal{P}(\lambda) \\
X(\Omega) = \mathbb{N} \\
\forall k \in X(\Omega), \,\mathbb{P}(X = k) = \frac{\lambda^k}{k!}e^{-\lambda}
\end{array}$$
#### Espérance

$$
\mathbb{E}(X) = \lambda
$$
#### Variance
$$
\mathbb{V}(X) = \lambda
$$

#### Convergence

Soit $(X_n)$ une suite de VA indépendantes suivant une loi de poisson de paramètre $\mu$.
Soit $S_{n}= \sum_{i=1}^{n}X_{i}$.
Alors $\frac{S_{n} - n\mu}{\sqrt{n\mu}} \xrightarrow{\text{loi}} \mathcal{N}(0, 1)$
# Lois continues

## Loi uniforme
#### Contexte

Généralisation de la notion d'équiprobabilité sur un intervalle de $\mathbb{R}$
#### Probabilité:

$$\begin{array}{c}
X \rightsquigarrow \mathcal{U}([a, b]) \\
f(t) =
\begin{cases}\frac{1}{b - a} & \text{si} t \in [a, b] \\
0 & \text{sinon}
\end{cases}
\end{array}$$
#### Espérance

$$
\mathbb{E}(X) = \frac{a+b}{2}
$$
#### Variance
$$
\mathbb{V}(X) = \frac{(b-a)^2}{12}
$$
## Lois exponentielle

#### Contexte

Généralisation de la loi de poisson sur $\mathbb{R}$. Loi sans mémoire
#### Probabilité:

$$\begin{array}{c}
X \rightsquigarrow \mathcal{E}(\lambda) \\
f(t) =
\begin{cases} \lambda e^{-\lambda t} & \text{si } t \geqslant 0 \\
0 & \text{sinon}
\end{cases}
\end{array}$$
#### Espérance

$$
\mathbb{E}(X) = \frac{1}{\lambda}
$$
#### Variance
$$
\mathbb{V}(X) = \frac{1}{\lambda^2}
$$
## Loi gamma

#### Probabilité:

$$\begin{array}{c}
X \rightsquigarrow \mathcal{G}_{a}(\alpha, \lambda) \\
f(t) =
\begin{cases} \frac{{\lambda^{\alpha}x^{\alpha-1}}}{{\Gamma(\alpha)}}e^{-\lambda t} & \text{si } t \geqslant 0 \\
0 & \text{sinon}
\end{cases}
\end{array}$$
Avec $\Gamma$ la fonction défini comme:
$$
\Gamma(\alpha) = \int_{0}^{+\infty}t^{\alpha-1}e^{-1}\mathrm{d}t
$$
#### Espérance

$$
\mathbb{E}(X) = \frac{\alpha}{\lambda}
$$
#### Variance
$$
\mathbb{V}(X) = \frac{\alpha}{\lambda^2}
$$
## Loi normale

#### Contexte

Loi régulière se concentrant autour de la moyenne et dont la répartition autour de la moyenne dépend de l'écart type
#### Probabilité:

$$\begin{array}{c}
X \rightsquigarrow \mathcal{N}(m, \sigma) \\
f(t) = \frac{1}{\sigma\sqrt{2\pi}}e^{-\frac{(x-m)^2}{2\sigma^2}}
\end{array}$$
#### Espérance

$$
\mathbb{E}(X) = m
$$
#### Variance
$$
\mathbb{V}(X) = \sigma^2
$$