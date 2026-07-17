> **例題 14**
>
> (10%) Find the inverse of $H = I_p - \dfrac{2uu^T}{u^T u}$, where $u$ is a $p \times 1$ nonzero vector.
>
> 〔101 高師統計〕
>
> **解：**
>
> $$H^2 = \left(I_p - \frac{2uu^T}{u^T u}\right)\left(I_p - \frac{2uu^T}{u^T u}\right) = I_p - \frac{2uu^T}{u^T u} - \frac{2uu^T}{u^T u} + \frac{4uu^T uu^T}{u^T u \cdot u^T u}$$
>
> $$= I_p - \frac{4uu^T}{u^T u} + \frac{4u(u^T u)u^T}{(u^T u)^2} = I_p - \frac{4uu^T}{u^T u} + \frac{4uu^T}{u^T u} = I_p$$
>
> $\therefore H^{-1} = H$

> **例題 15**
>
> 考慮方陣 $A$，若 $A^2 = A$，試證明：$(A + I)^n = I + (2^n - 1)A$，$\forall n \in N$。
>
> 〔91 中正資工、107 台大資工〕
>
> **解：**
>
> 由 $A^2 = A$，可推得 $A^3 = A^2A = A$，$A^4 = \cdots$，$A^k = A$，$\forall k \geq 1$。
>
> 考慮函數 $f(x) = (x+1)^n$，
>
> 則 $f(A) = (A + I)^n = \sum_{i=0}^{n} \binom{n}{i} A^i = I + \sum_{i=1}^{n} \binom{n}{i} A = I + (2^n - 1)A$
>
> 另解：
>
> $n = 1$ 時，$(A + I)^1 = I + (2^1 - 1)A$，原式成立；
>
> 假設 $n = k$ 之時原命題成立，
>
> 則 $n = k + 1$ 時
>
> $$(A + I)^{k+1} = (A + I)^k (A + I) = (I + (2^k - 1)A)(A + I)$$
>
> $$= A + (2^k - 1)A^2 + I + (2^k - 1)A$$
>
> $$= A + (2^k - 1)A + I + (2^k - 1)A$$
>
> $$= I + (2^{k+1} - 1)A$$
>
> 故由歸納法知原命題成立。