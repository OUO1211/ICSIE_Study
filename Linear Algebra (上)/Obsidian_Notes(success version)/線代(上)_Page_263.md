## 判斷歐式空間的子空間

> **試題 1**
>
> Determine whether $S$ is a subspace of $V$:
>
> (1) $S = \{(x, \cos x) \mid x \in R\}$，$V = R^2$。
>
> (2) $S = \left\{\begin{bmatrix} x \\ y \end{bmatrix} \mid xy \geq 0\right\}$，$V = R^2$。 【94 中台資工、107 海洋資工】
>
> (3) $S = \{(x_1, x_2, x_3) \mid \sum x_i = 1\}$，$V = R^3$。 【95 清大統計機械、84 中正資工、95 中興資科】
>
> (4) $S = \{(x_1, x_2, x_3) \mid x_1 < 0\}$，$V = R^3$。 【95 雲科資工、106 成大資科】
>
> (5) $S = \{(x_1, x_2, \ldots, x_n) \mid x_1 = 0 \text{ or } x_n = 0\}$，$V = R^n$。 【95 清大統計】

**解** (1) False.

$\because (0, 0) \notin S$。

(2) False.

$\because \begin{bmatrix} -1 \\ 0 \end{bmatrix} \in S$，$\begin{bmatrix} 0 \\ 1 \end{bmatrix} \in S$，但 $\begin{bmatrix} -1 \\ 0 \end{bmatrix} + \begin{bmatrix} 0 \\ 1 \end{bmatrix} = \begin{bmatrix} -1 \\ 1 \end{bmatrix} \notin S$。

(3) False.

$\because (0, 0, 0) \notin S$。

(4) False.

$\because (-1, 1, 1) \in S$，但 $(-1)(-1, 1, 1) = (1, -1, -1) \notin S$。

(5) False.

因為 $u = (1, 0, \ldots) \in S$，$v = (0, 0, \ldots, 1) \in S$，但 $u + v = (1, 0, \ldots, 1) \notin S$。
