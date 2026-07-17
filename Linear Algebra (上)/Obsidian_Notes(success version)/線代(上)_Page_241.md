## 第 2 章　線性方程組與求解

> **試題 7**
>
> Let $\delta: M_{n \times n}(R) \to R$ be a function defined on the space of all real $n \times n$ matrices $M_{n \times n}(R)$ with the following three properties:
>
> (i) $\delta$ is a linear function of each row of the matrix when the other row is held fixed.
>
> (ii) If two rows of $A \in M_{n \times n}(R)$ are identical, then $\delta(A) = 0$.
>
> (iii) If $I$ is the identity matrix, then $\delta(I) = 1$.
>
> (1) Let $B = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 0 & 1 \\ 0 & 1 & 0 \end{bmatrix}$，$C = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 2 \\ 0 & 0 & 1 \end{bmatrix}$. Find $\delta(B)$，$\delta(C)$. 【105 高雄應數】
>
> (2) (5%) Show that if $B \in M_{n \times n}(R)$ is the matrix that interchange the $i$-th and $j$-th rows of $A$, $i \neq j$ then $\delta(A) = -\delta(B)$.
>
> (3) (10%) Show that $\delta$ is the determinant function，$\delta = \det$.
>
> 【103,104 交大應數、104 清大數學】

**解** (1) $-1$；$-3$。

(2) 令 $A = \begin{bmatrix} \vdots \\ A_i \\ \vdots \\ A_j \\ \vdots \end{bmatrix}$，$B = \begin{bmatrix} \vdots \\ A_j \\ \vdots \\ A_i \\ \vdots \end{bmatrix}$，則

$$0 = \delta\!\left(\begin{bmatrix} \vdots \\ A_i + A_j \\ \vdots \\ A_i + A_j \\ \vdots \end{bmatrix}\right) = \delta\!\left(\begin{bmatrix} \vdots \\ A_i \\ \vdots \\ A_i \\ \vdots \end{bmatrix}\right) + \delta\!\left(\begin{bmatrix} \vdots \\ A_i \\ \vdots \\ A_j \\ \vdots \end{bmatrix}\right) + \delta\!\left(\begin{bmatrix} \vdots \\ A_j \\ \vdots \\ A_i \\ \vdots \end{bmatrix}\right) + \delta\!\left(\begin{bmatrix} \vdots \\ A_j \\ \vdots \\ A_j \\ \vdots \end{bmatrix}\right) = \delta(A) + 0 + 0 + \delta(B)$$

$\therefore \delta(A) = -\delta(B)$。

(3) 先證明：若 $E$ 為任一列基本矩陣，則 $\delta(E) = \det(E)$，…證明在最下方：

則對一般矩陣 $A$，

若 $A$ 可逆，則 $A$ 可以表成列基本矩陣之積 $A = E_1 \cdots E_t$，

則 $\delta(A) = \delta(E_1 \cdots E_t) = \delta(E_1) \cdots \delta(E_t) = \det(E_1) \cdots \det(E_t) = \det(E_1 \cdots E_t) = \det(A)$。

若 $A$ 不可逆，則 $\det(A) = 0$，且 $A$ 可列運算成 $R$，其中 $R$ 有零列，

令 $A = E_1 \cdots E_r \cdot R$，$R$ 為列梯形矩陣，$i = 1 \sim t$，

則 $\delta(A) = \delta(E_1 \cdots E_r) = \delta(E_1 \cdots E_r)\delta(R) = 0 = \det(A)$。

接著