> **例題 8**
>
> (3%) Assume $A$ is an $m \times n$ matrix with rank $r$ and $b$ is a column vector. Which statements are true?
>
> (1) If $m > r$ and $n = r$, then $Ax = b$ must have no solution for some $b$ and exactly one solution for other $b$.
>
> (2) If $m > r$ and $n > r$, then $Ax = b$ has infinitely many solutions for some $b$ and exactly one solution for other $b$.
>
> (3) If $n = r$, then $Ax = b$ has either one solution or none.
>
> 【98 交大資工】

解：$(1)$ True. $(2)$ False. $(3)$ True.

(1) True.

因為 $\operatorname{rank}(A)=n$，故 $Ax=b$ 若有解，則恆唯一解，

又 $\operatorname{rank}(A)=CS(A)=r<m=\dim(R^{m\times 1})$，

故存在 $b\in R^{m\times 1}$ 且 $b\notin CS(A)$，則某些 $b$ 使 $Ax=b$ 無解。

(2) False.

因為 $\operatorname{rank}(A)<n$，故 $Ax=b$ 若有解，必為無限多解，

又 $\operatorname{rank}(A)<m=\dim(R^{m\times 1})$，

故存在 $b\in R^{m\times 1}$ 且 $b\notin CS(A)$，則某些 $b$ 使 $Ax=b$ 無解。

(3) True.

由 (1) 可知。