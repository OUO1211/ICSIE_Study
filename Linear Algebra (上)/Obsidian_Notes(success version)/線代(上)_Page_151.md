# 第二章 線性方程組與求解 151

> **例題 8**
>
> (25%) Let $A$ be a $r$ by $s$ matrix with rank $t$ such that $Ax=(1,0,0)^T$ has no solutions and $Ax=(0,1,0)^T$ has exactly one solution.
>
> (1) Find all possible $(r,s,t)$.
>
> (2) Find all solutions of $Ax=(0,0,0)^T$.
>
> (3) Give an example of $A$ for each possible $(r,s,t)$.
>
> 【109 交大統計】

**解**

由 $Ax=\begin{bmatrix}1\\0\\0\end{bmatrix}$ 無解，故 $t=\operatorname{rank}(A)<$ 列數 $r$；

由 $Ax=\begin{bmatrix}0\\1\\0\end{bmatrix}$ 恰一組解，故 $t=\operatorname{rank}(A)=$ 行數 $s$；

由 $Ax$ 成為 $3\times 1$，故 $r=3$。

(1) 由上述討論知 $(r,s,t)$ 可是 $(3,2,2)$ 或 $(3,1,1)$。

(2) $\operatorname{rank}(A)=s=2$ 時，$Ax=\begin{bmatrix}0\\0\\0\end{bmatrix}$ 的解：$\begin{bmatrix}0\\0\end{bmatrix}$；

$\operatorname{rank}(A)=s=1$ 時，$Ax=0$ 的解：$0$。

(3) $(r,s,t)=(3,2,2)$：

例如取
$$
A=\begin{bmatrix}
0 & 0\\
1 & 0\\
0 & 1
\end{bmatrix}
$$
可使 $Ax=\begin{bmatrix}1\\0\\0\end{bmatrix}$ 無解，由 $Ax=\begin{bmatrix}0\\1\\0\end{bmatrix}$ 恰一組解；

$(r,s,t)=(3,1,1)$：

例如取
$$
A=\begin{bmatrix}
0\\
1\\
0
\end{bmatrix}
$$
可使 $Ax=\begin{bmatrix}1\\0\\0\end{bmatrix}$ 無解，且 $Ax=\begin{bmatrix}0\\1\\0\end{bmatrix}$ 恰一組解。