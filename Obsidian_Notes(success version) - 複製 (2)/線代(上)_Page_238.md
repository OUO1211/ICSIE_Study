## 2-5 進階試題練習

> **試題 1**
>
> (10%) Consider the following two linear systems. Where $A_{ij}$, $B_{ij}$, $Y_i$, $Z_i$ are constants and $x_j$ are unknown variables for $1 \leq i \leq m$, $1 \leq j \leq n$. Prove they have exactly the same solutions if they are equivalent
>
> $$\begin{cases} A_{11}x_1 + A_{12}x_2 + \cdots + A_{1n}x_n = Y_1 \\ A_{21}x_1 + A_{22}x_2 + \cdots + A_{2n}x_n = Y_2 \\ \vdots \\ A_{m1}x_1 + A_{m2}x_2 + \cdots + A_{mn}x_n = Y_m \end{cases} \quad \text{and} \quad \begin{cases} B_{11}x_1 + B_{12}x_2 + \cdots + B_{1n}x_n = Z_1 \\ B_{21}x_1 + B_{22}x_2 + \cdots + B_{2n}x_n = Z_2 \\ \vdots \\ B_{m1}x_1 + B_{m2}x_2 + \cdots + B_{mn}x_n = Z_m \end{cases}$$
>
> 【97,100,108 暨南資工】

**解** 令 $A = [A_{ij}]_{m \times n}$，$Y = [Y_i]_{m \times 1}$，$B = [B_{ij}]_{m \times n}$，$Z = [Z_i]_{m \times 1}$，$X = [x_i]_{n \times 1}$。

已知：$[A|Y]$ 中的列向量均可為 $[B|Z]$ 中的列向量的線性組合，

且 $[B|Z]$ 中的列向量均可為 $[A|Y]$ 中的列向量的線性組合，

故得 $RS([A|Y]) = RS([B|Z])$，

故存在可逆矩陣 $P$ 使滿足 $P(A|Y) = [B|Z]$，而得 $\ker([A|Y]) = \ker([B|Z])$。

設 $\bar{X}$ 為 $AX = Y$ 的一組解，則 $A\bar{X} = Y = 0$，故 $\begin{pmatrix} \bar{X} \\ -1 \end{pmatrix} \in \ker([A|Y]) = \ker([B|Z])$，

$\therefore B\bar{X} - Z = 0$，$\therefore \bar{X}$ 為 $BX = Z$ 的一組解，

同理也可得知：若 $\bar{X}$ 為 $BX = Z$ 的一組解，則 $\bar{X}$ 為 $AX = Y$ 的一組解，得證。

---

> **試題 2**
>
> The following is the pseudo-code for Gauss-Jordan method. Which of the following statements are correct?
>
> ```
> for k=1 to n
>     for j=k+1 to n+1
>         a_{kj} = a_{kj}/X
>     for i=1 to n (i is not equal to k)
>         for j=k+1 to n+1
>             a_{ij} = a_{ij} - (a_{ik})(a_{kj})
> ```
>
> (1) The solution is stored in $a(i,n)$, $i = 1 \sim n$.
>
> (2) The solution is stored in $a(n+1, i)$, $i = 1 \sim n$.
>
> (3) $X$ is $a_{nn}$.
>
> (4) $X$ is $a_{kk}$.
>
> (5) The solution is stored in $a(i, n+1)$, $i = 1 \sim n$.
>
> 【107 中央資工】

**解** (4), (5) true.

由原來高斯消去為以 pivot 做列運算：運算後的解在第 $n+1$ 行的各列。
