> **例題 12**
>
> True or false:
>
> (1) If $A$ and $B$ are $n \times n$ matrices and $\det(A - B) = 0$, then $\det(A) = \det(B)$.
>
> 【109 交大應數】
>
> 【109 成大電機】
>
> (2) There is no square matrix $A$ such that $\det(AA^T) = -1$.
>
> 【109 成大電機】
>
> (3) It is possible to have real-valued matrix $A$ such that $A^2 = -I$.
>
> 【95 台大資工、108 中央資工】
>
> (4) Let $A \in \mathbb{R}^{n \times n}$ and $n$ is odd. Then it is not possible $A^2 + I = O$.
>
> 【108 交大資工】

**解**

(1) False.

(2) False.

反例可取 $A = \begin{bmatrix} i & 0 \\ 0 & 1 \end{bmatrix}$

(3) True.

可取 $A = \begin{bmatrix} 0 & 1 \\ -1 & 0 \end{bmatrix}$，$A^2 = \begin{bmatrix} -1 & 0 \\ 0 & -1 \end{bmatrix} = -I$。

(4) True.

若存在 $A$ 使成立，則 $A^2 = -I$，

$\therefore \det(A^2) = \det(-I) = (-1)^n = -1$，……（因為 $n$ 為奇數）

但 $A$ 為實數矩陣，$\therefore \det(A^2) = \det(A)^2 \geq 0$ …… 矛盾

故知，不存在 $A$ 使 $A^2 + I = O$。