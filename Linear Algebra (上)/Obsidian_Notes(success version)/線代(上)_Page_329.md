334 線性代數(上)

> **例** 3  
> Determine the dimension of each of the following subspaces $V$.  
> (1) $V=\operatorname{span}([1,2,3],[3,4,7],[5,-2,3])\subseteq \mathbb{R}^3$。$\qquad[100\ \text{中央資工二類組}]$  
> (2) $V=\{[x_1,x_2,x_3,x_4]\mid x_1+x_2+x_3+x_4=0,\ x_2+x_4=0\}\subseteq \mathbb{R}^4$。  
> (3) $V=U+W$，
> $$\text{where} \left\{ 
\begin{aligned}
U &= \text{span} ([1, 0, 1, 1], [2, 1, 1, 2]) \subseteq \mathbb{R}^4 \\
W &= \text{span} ([0, 1, 1, 0], [2, 0, 1, 2]) \subseteq \mathbb{R}^4
\end{aligned}
\right.$$ 
> 。$\qquad[98\ \text{政大資料概論}]$

解 $\qquad[92\ \text{台大資工}]$

(1)

$$
\begin{bmatrix}
1 & 2 & 3\\
3 & 4 & 7\\
5 & -2 & 3
\end{bmatrix}
\rightarrow
\begin{bmatrix}
1 & 2 & 3\\
0 & -2 & -2\\
0 & -12 & -12
\end{bmatrix}
\rightarrow
\begin{bmatrix}
1 & 2 & 3\\
0 & -2 & -2\\
0 & 0 & 0
\end{bmatrix}
$$

$\therefore\ V=\operatorname{span}\{[1,2,3],[0,-2,-2]\}$，

又因 $S=\{[1,2,3],[0,-2,-2]\}$ 為獨立集，

故 $S$ 為 $V$ 的 basis，$\therefore\ \dim(V)=2$。

(2)

$$
\left\{
\begin{array}{l}
x_1+x_2+x_3+x_4=0,\\
x_2+x_4=0
\end{array}
\right.
\Leftrightarrow
\left\{
\begin{array}{l}
x_1+x_3=0,\\
x_2+x_4=0
\end{array}
\right.
\Leftrightarrow
\left\{
\begin{array}{l}
x_1=-x_3,\\
x_2=-x_4
\end{array}
\right.
$$

$\therefore\ V=\{[s,t,-s,-t]\mid s,t\in \mathbb{R}\}$，

$=\operatorname{span}\{[1,0,-1,0],[0,1,0,-1]\}$

又因 $S=\{[1,0,-1,0],[0,1,0,-1]\}$ 為獨立集

故 $S$ 為 $V$ 的 basis，$\therefore\ \dim(V)=2$。

(3)

$$
U+W=\operatorname{span}\{[1,0,1,1],[2,1,1,2],[0,1,1,0],[2,0,1,2]\}
$$

$$
\begin{bmatrix}
1 & 0 & 1 & 1\\
2 & 1 & 1 & 2\\
0 & 1 & 1 & 0\\
2 & 0 & 1 & 2
\end{bmatrix}
\rightarrow
\begin{bmatrix}
1 & 0 & 1 & 1\\
0 & 1 & -1 & 0\\
0 & 1 & 1 & 0\\
0 & 0 & -1 & 0
\end{bmatrix}
\rightarrow
\begin{bmatrix}
1 & 0 & 1 & 1\\
0 & 1 & -1 & 0\\
0 & 0 & 2 & 0\\
0 & 0 & -1 & 0
\end{bmatrix}
\rightarrow
\begin{bmatrix}
1 & 0 & 1 & 1\\
0 & 1 & -1 & 0\\
0 & 0 & 2 & 0\\
0 & 0 & 0 & 0
\end{bmatrix}
$$

$\therefore\ V=\operatorname{span}\{[1,0,1,1],[0,1,-1,0],[0,0,2,0]\}$，

又因 $\{[1,0,1,1],[0,1,-1,0],[0,0,2,0]\}$ 為獨立集，故為 $V$ 的 basis，$\therefore\ \dim(V)=3$。