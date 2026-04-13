# 第二章 線性方程組與求解 141

## Rank(A)與線性系統解的個數

> **定理**
>
> 考慮線性方程組 $Ax = b$，$A$ 為 $m \times n$，則
>
> (1) 若 $\text{rank}(A) \neq \text{rank}([A \mid b])$，則方程組無解。
>
> (2) 若 $\text{rank}(A) = \text{rank}([A \mid b]) = n$，則方程組恰有一解。
>
> (3) 若 $\text{rank}(A) = \text{rank}([A \mid b]) < n$，則方程組有無限多解。
>
> （且有 $n - \text{rank}(A)$ 個自由變數，即 $\text{rank}(A)$ 個基本變數。）
>
> (4) $\forall b \in R^{m}$，$Ax = b$ 有解 $\Leftrightarrow \text{rank}(A) = m$。
>
> （且有解時，若 $m = n$，則方程組恰一解；若 $m < n$，則方程組無限多解。）

在第三章會給上述性質的說明，在此先以舉例給直觀的看法。

例如：

(1) $\begin{cases} x + y = 5 \\ 2x + 2y = 7 \end{cases}$，為無解的系統。

$\text{rank}(A) = \text{rank}\begin{pmatrix} 1 & 1 \\ 2 & 2 \end{pmatrix} = 1$，$\text{rank}([A \mid b]) = \text{rank}\begin{pmatrix} 1 & 1 & 5 \\ 2 & 2 & 7 \end{pmatrix} = 2$。

(2) $\begin{cases} x + y = 5 \\ x + 2y = 7 \end{cases}$，為恰一解的系統。

$\text{rank}(A) = \text{rank}\begin{pmatrix} 1 & 1 \\ 1 & 2 \end{pmatrix} = 2$，$\text{rank}([A \mid b]) = \text{rank}\begin{pmatrix} 1 & 1 & 5 \\ 1 & 2 & 7 \end{pmatrix} = 2$ 且 $n =$ 變數個數 $= 2$。

(3) $\begin{cases} x + y = 5 \\ 2x + 2y = 10 \end{cases}$，為多解的系統。

$\text{rank}(A) = \text{rank}\begin{pmatrix} 1 & 1 \\ 2 & 2 \end{pmatrix} = 1$，$\text{rank}([A \mid b]) = \text{rank}\begin{pmatrix} 1 & 1 & 5 \\ 2 & 2 & 10 \end{pmatrix} = 1 < n = 2$。

$\times$ 補充：$Ax = b$ 有解 $\Leftrightarrow \text{rank}(A) = $ 列秩
