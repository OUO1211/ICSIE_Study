> **例題 1**
>
> (1) What linear combination of $(u_1 = 3 + x^2,\ u_2 = 1 + 2x,\ u_3 = x - x^2)$ can be obtained to form $2 - 3x - 2x^2$?
>
> (2) (2%) Let $a = \begin{bmatrix} 1 \\ 1 \\ 0 \end{bmatrix}$, $b = \begin{bmatrix} 1 \\ 2 \\ 0 \end{bmatrix}$, $c = \begin{bmatrix} 1 \\ 1 \\ 2 \end{bmatrix}$ and $d = \begin{bmatrix} -7 \\ 2 \\ 2 \end{bmatrix}$. Give $d$ as a linear combination of $a$, $b$ and $c$.
>
> 【94 中正電機碩題、97 成大統計】
>
> (3) Is $[-3, 0, 3]^T$ a linear combination of $[1\ 2\ 3]^T$ and $[4\ 5\ 6]^T$?

**解** (1) 設 $(2 - 3x - 2x^2) = au_1 + bu_2 + cu_3 = a(3 + x^2) + b(1 + 2x) + c(x - x^2)$，

比較各項係數得
$$
\begin{cases}
3a + b = 2 \\
2b + c = -3 \\
a - c = -2
\end{cases}
$$

解得 $a = \dfrac{9}{5}$，$b = -\dfrac{17}{5}$，$c = \dfrac{19}{5}$。

故得 $2 - 3x - 2x^2 = \dfrac{9}{5}u_1 - \dfrac{17}{5}u_2 + \dfrac{19}{5}u_3$。

(2) $d = -17a + 9b + c$。

(3) yes.

故
$$
\begin{bmatrix}
-3 \\
0 \\
3
\end{bmatrix}
=
\alpha
\begin{bmatrix}
1 \\
2 \\
3
\end{bmatrix}
+
\beta
\begin{bmatrix}
4 \\
5 \\
6
\end{bmatrix}
$$

即
$$
\begin{cases}
\alpha + 4\beta = -3 \\
2\alpha + 5\beta = 0 \\
3\alpha + 6\beta = 3
\end{cases}
$$

得 $\alpha = 5$，$\beta = -2$。

另解：

$$
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
-3 & 0 & 3
\end{bmatrix}
\xrightarrow{\text{列變}}
\begin{bmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 12
\end{bmatrix}
\xrightarrow{\text{列變}}
\begin{bmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & 0
\end{bmatrix}
$$

因最下方一列變成零列，故回答可被線性組合。