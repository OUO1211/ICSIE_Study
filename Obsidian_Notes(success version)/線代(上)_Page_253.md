## 第 2 章　線性方程組與求解

> **試題 26**
>
> Let $A$ be a nonsingular $n \times n$ matrix with a nonzero cofactor $A_{nn}$ at $(n, n)$ entry and set $\det A = A_{nn}$. Show that if we subtract $c$ from $(n, n)$ entry of $A$ then the resulting matrix will be singular.

**解** $\tilde{A} = [a_{ij}]_n$，$\tilde{B} = [\tilde{b}_{ij}]$，其中 $\tilde{b}_{ij} = \begin{cases} a_{ij} & \text{if } (i,j) \neq (n,n) \\ a_{nn} - c & \text{if } (i,j) = (n,n) \end{cases}$

則 $\det(\tilde{B}) = \displaystyle\sum_{j=1}^{n} \tilde{b}_{nj} B_{nj} = \displaystyle\sum_{j=1}^{n} a_{nj} B_{nj} + \tilde{b}_{nn} A_{nn} - a_{nn} A_{nn} = \displaystyle\sum_{j=1}^{n} a_{nj} A_{nj} + (a_{nn} - c)A_{nn} - a_{nn} A_{nn}$

$= \displaystyle\sum_{j=1}^{n-1} (a_{nj} A_{nj}) + a_{nn} A_{nn} - \det(A) - \det(A) = \det(A) - \det(A) = 0$，所以 $\tilde{B}$ singular。

---

> **試題 27**
>
> (10%) Analyze the complexity of evaluating the determinant of all $n \times n$ matrix by cofactors.
>
> 【104 成大資工】

**解** 今計算 $n$ 階矩陣所需乘法次數 $S_n$，因為同排列計算量如下：

$\det(A = [a_{ij}]_{n \times n}) = \displaystyle\sum_{j} a_{1j} \cdot \text{cof}(a_{1j})$，其中 $\text{cof}(a_{1j})$ 其中為 $n$ 階的餘因子，需計算 $n-1$ 階的行列式。

行列式（有 $n$ 個），且還要乘以 $a_{1j}$，故計算量如下：

$S_n = n(S_{n-1} + 1)$，且還要 $n = n-1 + (n-1)n \cdot 1 \cdot n + \cdots$

由直接代入法可得

$S_n = n(n-1)S_{n-2} + n(n-1) + n$

$= n(n-1)(n-2)S_{n-3} + n(n-1)(n-2) + n(n-1) + n$

$= \cdots$

$= n! \cdot S_1 + n! + \dfrac{n!}{2!} + \cdots + \dfrac{n!}{(n-1)!}$

$= n! \cdot 0 + n! \cdot \dfrac{1}{0!} + n! \cdot \dfrac{1}{1!} + \cdots + n! \cdot \dfrac{1}{(n-1)!}$

$\approx n! \cdot e$

$= \Theta(n!)$
