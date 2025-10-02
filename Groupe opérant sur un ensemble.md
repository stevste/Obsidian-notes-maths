#Algèbre #Groupe 

Dans cette section, $E$ est un ensemble et $G$ un [[Groupe]]
# Définition

### Action sur un groupe

Soit $G$ un Groupe et $E$ un ensemble. On appelle action à gauche de $G$ sur $E$ toute [[Application]]:
$$\begin{array}{l rcl}  G \times E & \longrightarrow & \mathbb{R} \\
(g,x) & \longmapsto & g_{\bullet}x \end{array}
$$
$E$ est alors appelé un $G$-ensemble
de la même manière, on peut créer des opérations à droite

### Point fixe

1. On dit que $x \in E$ est un point fixe sous l'action de si $g_{\bullet}x = x, \forall g \in G$
2. On dit que $F \subset E$ est une partie stable si $g(F) \subset F \forall g \in G$

### Morphisme structurel

À une action d'une groupe $G$ sur un ensemble $E$ correspond un [[Morphisme de groupe]] structurel
$$\begin{array}{l rcl} \Phi : & G & \longrightarrow & \mathbb{G} \\
& g & \longmapsto & \sigma_g \end{array}
$$
avec $\sigma_g = g_{\bullet}x$
Ainsi, toute action de $G$ sur $E$ est lié à une unique application $E \longrightarrow E$. Pour un élément de $G$, on a donc $g_{\bullet}x = \Phi(g)(x)$.
# Propriété

- Soit $G$ un groupe et $\psi \longrightarrow \mathbb{G}$. Si $\psi: \Gamma \longrightarrow G$ est un morphisme, alors $E$ est aussi un $\Gamma$-ensemble et $\gamma_{\bullet}x = \Phi(\psi(\gamma))(x)$
- Si $F \subset E$ est stable sur $E$, alors $F$ est un $G$-ensemble
- Soit $H$ un sous groupe de $G$, alors $E$ est un $H$-ensemble
- Si $E$ est un ensemble fini  à $n \in \mathbb{N}$ éléments, à toute numérotation des éléments de $E$ correspond une bijection entre les éléments de $G$ et les morphismes structurels de $G$
- $(\mathbb{G}, \circ)$ est un groupe appelé [[Groupe symétrique]]