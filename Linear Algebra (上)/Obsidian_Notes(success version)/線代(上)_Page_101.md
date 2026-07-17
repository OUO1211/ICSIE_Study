# 第一章 矩陣 100

$\because AB + BA = O$，$\therefore 0 = \text{tr}(O) = \text{tr}(AB + BA) = 2\text{tr}(AB)$，$\therefore \text{tr}(AB) = 0$。

令 $AB = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$，則 $\det(AB) = \begin{bmatrix} a^2 + bc & 0 \\ 0 & a^2 + bc \end{bmatrix} = (a^2 + bc)I$，故取 $y = a^2 + bc$。

> **試題 4**
>
> Let $A$ and $B$ be $n \times n$ matrices, and $A + B = AB$. Prove that $AB = BA$.

**解**

因為 $AB - A - B = O$。

$\therefore AB - A - B + I = I$，即 $(A-I)(B-I) = I$，$\therefore (A-I)^{-1} = (B-I)$，

故可得到 $(B-I)(A-I) = I$，即 $BA - B - A + I = I$，即得 $BA = B + A$，故得 $AB = BA$。

> **試題 5**
>
> Let $X_n = (x_1, \ldots, x_n)^T$ be an $n$ by $k$ dimensional matrix where the $x_i$'s are $k$-vectors. Show that
>
> $(X_{n-1}^T X_{n-1})^{-1} = (X_n^T X_n)^{-1} + \dfrac{(X_n^T X_{n-1})^{-1} x_n x_n^T (X_n^T X_n)^{-1}}{1 - x_n^T (X_n^T X_n)^{-1} x_n}$
>
> 【89 台大電機‧94 高雄統計‧95 中央統計】

**解**

$x_n$ 為行向量且由定義可得 $X_{n-1}^T X_{n-1} = A - x_n x_n^T$，$X_n^T X_n = A$。

令 $X_n^T X_n = A$，$- x_n = u$，$v^T = x_n^T$，則利用前面範例 11 的類題討論可得

$(X_{n-1}^T X_{n-1})^{-1} = (A - x_n x_n^T)^{-1}$
$= A^{-1} - A^{-1}U(I + V^T A^{-1} U)^{-1} V^T A^{-1}$
$= (X_n^T X_n)^{-1} - (X_n^T X_n)^{-1}(-x_n)(1 + x_n^T (X_n^T X_n)^{-1}(-x_n))^{-1} x_n^T (X_n^T X_n)^{-1}$
$= (X_n^T X_n)^{-1} + \dfrac{(X_n^T X_n)^{-1} x_n x_n^T (X_n^T X_n)^{-1}}{1 - x_n^T (X_n^T X_n)^{-1} x_n}$

> **試題 6**
>
> (10%) Given an invertible $n \times n$ real matrix $A$ and one column vector $u \in R^n$, consider $x = A^{-1}u$ and $y = (A + \lambda u v^T)^{-1} u$ for any scalar $\lambda$ and column vector $v \in R^n$ such that $A + \lambda u v^T$ is also invertible. Determine whether $y$ is parallel to $x$.
>
> 【102 中央統計】

**解**

$\because (A + UV^T)^{-1} = A^{-1} - A^{-1}U(I + V^T A^{-1}U)^{-1} V^T A^{-1}$，

$\therefore (A + \lambda u v^T)^{-1} = A^{-1} - \lambda A^{-1} u (1 + \lambda v^T A^{-1} u)^{-1} v^T A^{-1}$，
