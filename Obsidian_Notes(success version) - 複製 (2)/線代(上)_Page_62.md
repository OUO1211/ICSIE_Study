## 方陣多項式

> **定義：方陣多項式**
>
> 考慮方陣 $A$ 的多項式 $f(x) = a_0 + a_1 x + a_2 x^2 + \cdots + a_k x^k = \sum_{i=0}^{k} a_i x^i$，
>
> 定義 $f(A) = a_0 I + a_1 A + a_2 A^2 + \cdots + a_k A^k = \sum_{i=0}^{k} a_i A^i$，稱為一方陣多項式，其中 $A^0 = I$。

可用來求反矩陣（即例如）：

若 $A^2 + 2A + 3I = 0$，

則 $A(A + 2I) = -3I$，

故 $A^{-1} = -\dfrac{1}{3}(A + 2I)$。

> **例題 13**
>
> Let $A = [a_{ij}]$ be the $4 \times 4$ matrix that has 0 at each diagonal entry and 1 at all other entries.
>
> that is, $a_{ij} = \begin{cases} 0 & \text{if } i = j \\ 1 & \text{if } i \neq j \end{cases}$
>
> (1) Find constants $a$ and $b$ such that $A^2 = aA + bI$.
>
> (2) Prove that $A$ is nonsingular and calculate $A^{-1}$.
>
> 〔94 成大統計〕
>
> **解：**
>
> (1) $A = \begin{bmatrix} 0 & 1 & 1 & 1 \\ 1 & 0 & 1 & 1 \\ 1 & 1 & 0 & 1 \\ 1 & 1 & 1 & 0 \end{bmatrix}$，$A^2 = \begin{bmatrix} 3 & 2 & 2 & 2 \\ 2 & 3 & 2 & 2 \\ 2 & 2 & 3 & 2 \\ 2 & 2 & 2 & 3 \end{bmatrix} = 2A + 3I$
>
> 另解：
>
> 令 $J$ 為元素都是 1 的矩陣，則 $A = J - I$，
>
> 且 $A^2 = (J-I)^2 = J^2 - 2J + I = 4J - 2J + I = 2J + I = 2(A+I) + I = 2A + 3I$
>
> (2) 由 (1) 得 $A^2 = 2A + 3I$，即 $\dfrac{1}{3}A^2 - \dfrac{2}{3}A - I = 0$，即 $A\left(\dfrac{1}{3}A - \dfrac{2}{3}I\right) = I$，
>
> 故 $A^{-1} = \dfrac{1}{3}A - \dfrac{2}{3}I = \dfrac{1}{3}(A - 2I) = \begin{bmatrix} -\frac{2}{3} & \frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\ \frac{1}{3} & -\frac{2}{3} & \frac{1}{3} & \frac{1}{3} \\ \frac{1}{3} & \frac{1}{3} & -\frac{2}{3} & \frac{1}{3} \\ \frac{1}{3} & \frac{1}{3} & \frac{1}{3} & -\frac{2}{3} \end{bmatrix}$
