(3) $\because 1 = \det(I) = \det(\text{adj}(A)) = \det(A)^{n-1}$，$\therefore \det(A) = \pm 1$，$\therefore A \cdot I = \det(A) \cdot I$，

$\therefore A = \pm I$。

---

> **試題 24**
>
> If $A$ is nonsingular and the row sums of $A$ are 1, show that row sums of $A^{-1}$ are also 1.
>
> 【108 交大統計】

**解** 本題用特徵向量性質比較容易。

$\because A^{-1} = \dfrac{1}{\det(A)}\text{adj}(A)$。

其中 $\text{adj}(A) = \begin{bmatrix} A_{11} & A_{21} & \cdots & A_{n1} \\ A_{12} & A_{22} & \cdots & A_{n2} \\ \vdots & \vdots & & \vdots \\ A_{1n} & A_{2n} & \cdots & A_{nn} \end{bmatrix}$，$A_{ij} = \text{cof}(a_{ij}) = (-1)^{i+j}\det(M_{ij})$。

$\therefore A^{-1}$ 中第 $i$ 行的和 $= \dfrac{1}{\det A}(A_{1i} + A_{2i} + \cdots + A_{ni})$

對 $A$ 做行運算：將第 $i$ 行（除了第 $i$ 行外）加到第 $i$ 行，則

$$\det A = \begin{vmatrix} a_{11} & \cdots & a_{1i} & \cdots & a_{1n} \\ \vdots & & \vdots & & \vdots \\ a_{n1} & \cdots & a_{ni} & \cdots & a_{nn} \end{vmatrix}$$

第 $j$ 行時展開間 $\det A = A_{1i} + A_{2i} + \cdots + A_{ni} = \det A$，$\forall 1 \leq i \leq n$。

$\therefore A^{-1}$ 中第 $i$ 行的和 $= \dfrac{1}{\det A} \times \det A = 1$，$\forall 1 \leq i \leq n$。

---

> **試題 25**
>
> (15%) Let $A$ be a $4 \times 4$ nonsingular matrix, $a$ be a $4 \times 1$ vector, and $c$ be a scalar such that $c > a^T A a \geq 0$. Show that the matrix $B = A - aa^T/c$ is nonsingular.
>
> 【102 高雄統計】

**解** 題目代入假設，推導 $a^T A a \geq 0$。

$\det(B) = \det(A - aa^T/c) = \det\!\left(A\!\left(I - \dfrac{A^{-1}aa^T}{c}\right)\right)$

$= \det(A)\det\!\left(I - \dfrac{A^{-1}a \cdot a^T}{c}\right) = \det(A)\det(I - XY)$（其中 $X = A^{-1}a$，$Y = a^T$，此處中

$\neq 0$，……$a^T A^{-1} a \geq 0$

$\neq 0$，$\therefore \det A \neq 0$，$\because \det\!\left(1 - \dfrac{a^T A^{-1} a}{c}\right) \times 1 = 1 - \dfrac{a^T A^{-1} a}{c} > 0$

故 $B$ 可逆。
