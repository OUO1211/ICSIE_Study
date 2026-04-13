> **例題 9**
>
> (15%) $A$ is an $m$ by $n$ matrix of rank $r$. Suppose that there are right sides $b$ for which $Ax = b$ has no solution.
>
> (1) (5%) What are all inequalities ($< \text{ or } \leq$) that must be true between $m$, $n$ and $r$?
>
> (2) (4%) Does $A^T y = 0$ have solutions other than $y = 0$? Why?
>
> (3) (4%) Suppose $A^T y = d$ is solvable. Is the solution $y$ unique? Why?
>
> (4) (2%) Suppose column 1+ column 3+ column 4 $= 0$ in a 3 by 4 matrix with rank 3. What is the null space?
>
> 【102 成大統計】

解：

由已知存在右向量 $b$，使 $Ax = b$ 無解，故 $\operatorname{rank}(A) = r < m$。

(1) $r < m$，

$r \leq n$。

(2) $\dim(N(A^T)) = m - \dim(CS(A^T)) = m - \operatorname{rank}(A^T) = m - \operatorname{rank}(A) = m - r > 0$。

故存在非零向量 $y \in N(A^T)$，

即存在非零向量 $y$，使 $A^T y = 0$。

(3) 因為 $A^T y = d$ 有解，且 $\operatorname{rank}(A^T) = \operatorname{rank}(A) = r < m$：$A^T$ 的行數，

故 $A^T y = d$ 的解不唯一。

(4) $\because \dim(N(A)) = 4 - \operatorname{rank}(A) = 4 - 3 = 1$，

且
$$
A \begin{bmatrix}
1 \\
0 \\
-1 \\
1
\end{bmatrix}
= 0,
$$
故
$$
N(A) = \operatorname{span}\left\{
\begin{bmatrix}
1 \\
0 \\
-1 \\
1
\end{bmatrix}
\right\}.
$$