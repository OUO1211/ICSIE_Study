> **例題 6**
>
> (10%) Find a basis for the intersection of the subspaces $F = span\{(1,0,1,1), (2,1,1,2)\}$ and $W = span\{(0,1,3,0), (2,0,1,2)\} \subseteq \mathbb{R}^4$。
>
> 【97.99 清大統計，99 台大電信 題組，101 台大資工】

**解**

(1) $\begin{bmatrix} 1 & 0 & 1 & 1 \\ 2 & 1 & 1 & 2 \end{bmatrix}$ 可約簡並知 $\begin{bmatrix} 1 & 0 & 1 & 1 \\ 0 & 1 & -1 & 0 \end{bmatrix}$，則 $V = span\left\{ \begin{bmatrix} 1 \\ 0 \\ 1 \\ 1 \end{bmatrix}, \begin{bmatrix} 0 \\ 1 \\ -1 \\ 0 \end{bmatrix} \right\}$，

令 $v \in V \cap W$，$\therefore v = a\begin{bmatrix} 1 \\ 0 \\ 1 \\ 1 \end{bmatrix} + b\begin{bmatrix} 0 \\ 1 \\ -1 \\ 0 \end{bmatrix} = c\begin{bmatrix} 0 \\ 1 \\ 3 \\ 0 \end{bmatrix} + d\begin{bmatrix} 2 \\ 0 \\ 1 \\ 2 \end{bmatrix}$ for some $a, b, c, d \in \mathbb{R}$，

則 $\begin{bmatrix} 1 & 0 & 0 & -2 \\ 0 & 1 & -1 & 0 \\ 1 & -1 & -3 & -1 \\ 1 & 0 & 0 & -2 \end{bmatrix} \in \ker\begin{bmatrix} a \\ b \\ c \\ d \end{bmatrix} = \ker\begin{bmatrix} 1 & 0 & 0 & -2 \\ 0 & 1 & -1 & 0 \\ 0 & 0 & -2 & 1 \\ 0 & 0 & 0 & 0 \end{bmatrix}$，$\begin{bmatrix} a \\ b \\ c \\ d \end{bmatrix} = t\begin{bmatrix} 2r \\ 1/2 \\ 1/2 \\ r \end{bmatrix}$（$t \in \mathbb{R}$），

得 $V \cap W = \left\{ 2t\begin{bmatrix} 1 \\ 0 \\ 1 \\ 1 \end{bmatrix} + \frac{t}{2}\begin{bmatrix} 0 \\ 1 \\ -1 \\ 0 \end{bmatrix} \mid t \in \mathbb{R} \right\} = span\left\{ \begin{bmatrix} 2t \\ t/2 \\ 3t/2 \\ 2t \end{bmatrix} \mid t \in \mathbb{R} \right\} = span\left\{ \begin{bmatrix} 2 \\ 1/2 \\ 3/2 \\ 2 \end{bmatrix} \right\}$，

可取基底為 $\begin{bmatrix} 2 \\ 1/2 \\ 3/2 \\ 2 \end{bmatrix}$。
