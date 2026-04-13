## 秩與線性系統的解的個數

$A：m \times n$，

> **定理**
>
> (1) $Ax = b$ 有解 $\Leftrightarrow$ $\text{rank}([A|b]) = \text{rank}(A)$。
>
> 【91 交大應數、92 清大進數、93 中山法工、101 台大電信、103 台大電機】
>
> (2) 若 $b \in R^m$，$Ax = b$ 有解 $\Leftrightarrow \forall b \in R^m$，$b \in CS(A)$。
>
> 【101 台大電機、103 台大電機】
>
> 且有時候 if $m = n$，then $|b|$ 多一解；if $m < n$，則多解。

> **【證明】**
>
> (1) $Ax = b$ 有解
>
> $\Leftrightarrow$ 存在 $x \in F^{n \times 1}$ 使 $Ax_0 = b$，
>
> $\Leftrightarrow b \in CS(A)$，
>
> $\Leftrightarrow b \in \text{span}(A^{(1)}, A^{(2)}, \ldots, A^{(n)})$，
>
> $\Leftrightarrow \text{span}(A^{(1)}, A^{(2)}, \ldots, A^{(n)}) = \text{span}(A^{(1)}, A^{(2)}, \ldots, A^{(n)}, b)$，
>
> $\Leftrightarrow \text{rank}(A) = \text{rank}(A|b)$。
>
> (2) 若 $\forall b \in R^m$，$Ax = b$ 有解，
>
> 即 $CS(A) = R^m$，故 $\text{rank}(A) = m$。
>
> 故 $\forall b \in R^m$，$\therefore CS(A) = R^m$，故 $\text{rank}(A) = m$，
>
> 故 $\forall b \in R^m$，$b \in CS(A)$，
>
> 即 $\forall b \in R^m$，$Ax = b$ 有解。