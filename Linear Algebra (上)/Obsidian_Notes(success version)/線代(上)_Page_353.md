故其解空間為 $\left\{ \begin{bmatrix} a \\ b \\ c \\ d \end{bmatrix} \middle| \begin{array}{l} a + 2b + 4d = 0 \\ c + 3d = 0 \end{array} \right\} = \left\{ \begin{bmatrix} -2b - 4d \\ b \\ -3d \\ d \end{bmatrix} \middle| b, d \in \mathbb{R} \right\} = \operatorname{span}\left\{ \begin{bmatrix} -2 \\ 1 \\ 0 \\ 0 \end{bmatrix}, \begin{bmatrix} -4 \\ 0 \\ -3 \\ 1 \end{bmatrix} \right\}$

> **例題 18**
>
> Which vectors form the basis for null($A$)? $A = \begin{bmatrix} 1 & 1 & 3 & 1 & 6 \\ 2 & -1 & 0 & 1 & -1 \\ -3 & 2 & 1 & -2 & 1 \\ 4 & 1 & 6 & 1 & 3 \end{bmatrix}$
>
> (1) $[-3,2,1,-1,1]$. (2) $[-1,-2,1,0,0]$. (3) $[1,-3,0,-4,1]$. (4) $[2,-1,0,-1,-1]$. (5) None.
>
> 【110 中央資工】

**解** (2), (3).

$\begin{bmatrix} 1 & 1 & 3 & 1 & 6 \\ 2 & -1 & 0 & 1 & -1 \\ -3 & 2 & 1 & -2 & 1 \\ 4 & 1 & 6 & 1 & 3 \end{bmatrix} \xrightarrow{\text{列運算}} \begin{bmatrix} -3 & -1 & 1 & 2 \\ 2 & -2 & -3 & -1 \\ 1 & 1 & 0 & 0 \\ -1 & 0 & -4 & -1 \\ 1 & 0 & 1 & -1 \end{bmatrix} \xrightarrow{} \begin{bmatrix} 7 & 0 & 0 & -6 \\ \ast & 0 & 0 & \ast \\ \ast & \ast & 0 & 0 \\ \ast & \ast & \ast & 0 \end{bmatrix}$，即

只有第二與第三選項在 null($A$) 中，又剛剛可得第二與第三選項形成獨立集，故可以當作 null($A$) 的一組基底。