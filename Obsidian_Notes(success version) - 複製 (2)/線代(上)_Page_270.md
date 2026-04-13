## 判斷函數空間的子空間

> **例題 4**
>
> Let $P_n$ denote the set of polynomials of degree less than $n$. Which of the following is a subspace of $P_4$?
>
> (1) $W$: The set of polynomials in $P_4$ of even degree.
>
> (2) $W$: The set of polynomials in $P_4$ of degree 3. 【101 交大資工】
>
> (3) $W$: The set of polynomials in $P_4$ such that $P(0) = 0$.
>
> (4) $W$: The set of polynomials in $P_4$ having at least one real root.

**解** (1) 考慮 $f(x) = -x^2 + x$，$g(x) = x^2 + x$，則 $f(x) + g(x) = 2x$，故所取向量集不滿足封閉性，不為向量空間。

(2) 取 $f(x) = x^3 + 2$，$g(x) = -x^3 + 3x$，則 $f(x) + g(x)$ 不為次數 3。

不滿足加法封閉性。

(3) 滿足加法與純量積封閉性：

（取 $f(x)$，$g(x)$ 滿足 $f(0) = 0$，$g(0) = 0$，$\alpha$ 為純量，則

$(\alpha f + g)(0) = \alpha f(0) + g(0) = 0$。）

(4) 取 $f(x) = x^2$，$g(x) = x + 1$ 均有至少一實根，但 $f(x) + g(x) = x^2 + x + 1$ 卻沒有實根。