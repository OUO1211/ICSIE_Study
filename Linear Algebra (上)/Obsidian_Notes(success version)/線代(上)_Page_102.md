# 第一章 矩陣 101

$$
\therefore y = (A + \lambda uv^T)^{-1}u = A^{-1}u - \lambda A^{-1}u(1 + \lambda v^T A^{-1}u)^{-1}v^T A^{-1}u
$$

$$
= x - \lambda x(1 + \lambda v^T A^{-1}u)^{-1}v^T A^{-1}u
$$

$$
= x\left(1 - \dfrac{\lambda v^T x}{1 + \lambda v^T x}\right)
$$

$$
= x \cdot \dfrac{1}{1 + \lambda v^T x}
= x\left(\dfrac{1 - \lambda v^T x}{1 + \lambda v^T x}\right)
x \quad \therefore y // x
$$

> **試題 7**
>
> (10%) Find $M^{-1}$ if $M_{n \times n} = \begin{bmatrix} 1 & 2 & \cdots & 2 \\ 2 & 1 & \cdots & \vdots \\ \vdots & & \ddots & 2 \\ 2 & \cdots & 2 & 1 \end{bmatrix}$. Hint: If $C$ and $D$ are $n$ by $k$ such that $(I + D^T A^{-1} C)^{-1}$ exists, then $(A + CD^T)^{-1} = A^{-1} - A^{-1}C(I + D^T A^{-1} C)^{-1}D^T A^{-1}$。
>
> 【97 中興統計】

**解**

令 $A = -I_n$，$C = \begin{bmatrix} 1 \\ 1 \\ \vdots \\ 1 \end{bmatrix}$，$D = \begin{bmatrix} 2 \\ 2 \\ \vdots \\ 2 \end{bmatrix}$，則 $M = A + CD^T$

且 $A^{-1} = -I_n$，$(I + D^T A C)^{-1} = \left\{1 + [2, 2, \ldots, 2]\begin{bmatrix} -1 & 0 & \cdots & 0 \\ 0 & -1 & \cdots & 0 \\ \vdots & & \ddots & \vdots \\ 0 & 0 & \cdots & -1 \end{bmatrix}\begin{bmatrix} 1 \\ 1 \\ \vdots \\ 1 \end{bmatrix}\right\}^{-1} = \dfrac{1}{1 - 2n}$

$$
\therefore M^{-1} = (A + CD^T)^{-1} = A^{-1} - A^{-1}C(I + D^T A^{-1} C)^{-1}D^T A^{-1}
$$

$$
= -I_n + \dfrac{1}{2n - 1}CD^T
$$

$$
= \dfrac{1}{2n - 1}\left\{\begin{bmatrix} 1 - 2n & 0 & \cdots & 0 \\ 0 & 1 - 2n & \cdots & 0 \\ \vdots & & \ddots & \vdots \\ 0 & 0 & \cdots & 1 - 2n \end{bmatrix} + \begin{bmatrix} 2 & 2 & \cdots & 2 \\ 2 & 2 & \cdots & 2 \\ \vdots & & \ddots & \vdots \\ 2 & 2 & \cdots & 2 \end{bmatrix}\right\}
$$

$$
= \dfrac{1}{2n - 1}\begin{bmatrix} 3 - 2n & 2 & \cdots & 2 \\ 2 & 3 - 2n & \cdots & \vdots \\ \vdots & & \ddots & 2 \\ 2 & \cdots & 2 & 3 - 2n \end{bmatrix}
$$