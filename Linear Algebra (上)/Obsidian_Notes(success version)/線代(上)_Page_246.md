> **試題 14**
>
> Show that if $f_1(x)$，$f_2(x)$，$g_1(x)$，$g_2(x)$ are differentiable functions and if
>
> $W = \begin{vmatrix} f_1(x) & f_2(x) \\ g_1(x) & g_2(x) \end{vmatrix}$，then $\dfrac{d}{dx} \begin{vmatrix} f_1(x) & f_2(x) \\ g_1(x) & g_2(x) \end{vmatrix} = \begin{vmatrix} f_1'(x) & f_2'(x) \\ g_1(x) & g_2(x) \end{vmatrix} + \begin{vmatrix} f_1(x) & f_2(x) \\ g_1'(x) & g_2'(x) \end{vmatrix}$
>
> 【95 暨南資工】

**解** $W = f_1 g_2 - f_2 g_1$，

$\therefore \dfrac{d}{dx} W = (f_1 g_2 - f_2 g_1)' = (f_1' g_2 + f_1 g_2') - (f_2' g_1 + f_2 g_1') = f_1' g_2 - f_2' g_1 + f_1 g_2' - f_2 g_1'$

$= \begin{vmatrix} f_1'(x) & f_2'(x) \\ g_1(x) & g_2(x) \end{vmatrix} + \begin{vmatrix} f_1(x) & f_2(x) \\ g_1'(x) & g_2'(x) \end{vmatrix}$

故等式成立。

---

> **試題 15**
>
> Find the derivative of the function $f(x)=\det\begin{bmatrix} 1 & 1 & 2 & 3 & 4 \\ 9 & 0 & 2 & 3 & 4 \\ 9 & 0 & 0 & 3 & 4 \\ x & 1 & 2 & 9 & 1 \\ 7 & 0 & 0 & 0 & 4 \end{bmatrix}$
>
> 【95 雲科資工】

**解** 對第 1 列降階展開，得

$$f(x)=1\cdot\begin{vmatrix} 0 & 2 & 3 & 4 \\ 0 & 0 & 3 & 4 \\ 1 & 2 & 9 & 1 \\ 0 & 0 & 0 & 4 \end{vmatrix}-9\cdot\begin{vmatrix} 1 & 2 & 3 & 4 \\ 0 & 0 & 3 & 4 \\ x & 2 & 9 & 1 \\ 0 & 0 & 0 & 4 \end{vmatrix}+9\cdot\begin{vmatrix} 1 & 2 & 3 & 4 \\ 0 & 2 & 3 & 4 \\ x & 2 & 9 & 1 \\ 0 & 0 & 0 & 4 \end{vmatrix}-x\cdot\begin{vmatrix} 1 & 2 & 3 & 4 \\ 0 & 2 & 3 & 4 \\ 0 & 0 & 3 & 4 \\ 0 & 0 & 0 & 4 \end{vmatrix}+7\cdot\begin{vmatrix} 1 & 2 & 3 & 4 \\ 0 & 2 & 3 & 4 \\ 0 & 0 & 3 & 4 \\ 1 & 2 & 9 & 1 \end{vmatrix}$$

$$\therefore f'(x)=-\begin{vmatrix} 1 & 2 & 3 & 4 \\ 0 & 2 & 3 & 4 \\ 0 & 0 & 3 & 4 \\ 0 & 0 & 0 & 4 \end{vmatrix}=-1\cdot2\cdot3\cdot4=-24$$