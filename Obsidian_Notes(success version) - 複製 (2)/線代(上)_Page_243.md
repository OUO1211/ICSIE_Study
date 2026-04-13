## 第 2 章　線性方程組與求解

> **試題 9**
>
> A vector $x$ in $R^n$ is called **integral** if every component of $x$ is an integer. Let $A$ be a nonsingular $n \times n$ matrix with integer entries. Prove that the system of equations $Ax = b$ has an integral solution for every integral vector $b$ in $R^n$ if and only if $\det(A) = \pm 1$.
>
> 【105 清大數學】

**解** $\Leftarrow$：$\because A \in Z^{n \times n}$，故 $A$ 的每個位置的餘因子 (cofactor) 均為整數，

故 $A$ 的伴隨矩陣 $(\text{adj}) \in Z^{n \times n}$，

$\therefore A^{-1} = \dfrac{1}{\det(A)} \text{adj}(A) = \pm \text{adj}(A) \in Z^{n \times n}$，

$\therefore Ax = b$ 有整數解 $x = A^{-1}b$，$\forall b \in Z^n$，

$\Rightarrow$：考慮 $b$ 依序代入標準基底的方向向量 $e_1 \sim e_n$，則所得的解為 $v_1 \sim v_n$，均為整數向量，

則 $[v_1 \cdots v_n] = A^{-1} \in Z^{n \times n}$，$\det(A^{-1}) \in Z$，

又 $A \in Z^{n \times n}$，$\det(A) \in Z$，且 $\det(A^{-1}) \times \det(A) = 1$，$\therefore \det(A) = \pm 1$。

---

> **試題 10**
>
> (10%) Define the **absolute determinant** of a $m \times n$ matrix $A$ ($n \leq m$) (denoted as $\text{abs\_det}(A)$) is given by the definition $\text{abs\_det}(A) = \det(A^T A)^{1/2}$. For example, $A = \begin{bmatrix} 1 \\ 2 \end{bmatrix}$,
>
> $A^T = [1, 2]$, $\text{abs\_det}(A) = (\det(A^T A))^{1/2} = (\det[5])^{1/2} = \sqrt{5}$. Let $B = \begin{bmatrix} 1 & 3 \\ 2 & 0 \\ 1 & 4 \end{bmatrix}$.
>
> Find $\text{abs\_det}(B)$.
>
> 【101 彰師資工】

**解** $\text{abs\_det}(B) = \det\!\left(\begin{bmatrix} 1 & 2 & 1 \\ 3 & 0 & 4 \end{bmatrix}\begin{bmatrix} 1 & 3 \\ 2 & 0 \\ 1 & 4 \end{bmatrix}\right)^{1/2} = \det\!\begin{bmatrix} 6 & 7 \\ 7 & 25 \end{bmatrix}^{1/2} = \sqrt{101}$

---

> **試題 11**
>
> (5%) If
>
> $$
> P_n =
> \begin{bmatrix}
> \dfrac{1}{2} & \dfrac{1}{3} & \cdots & \dfrac{1}{n+1} \\
> \dfrac{1}{3} & \dfrac{1}{4} & \cdots & \dfrac{1}{n+2} \\
> \vdots & \vdots & & \vdots \\
> \dfrac{1}{n+1} & \dfrac{1}{n+2} & \cdots & \dfrac{1}{2n}
> \end{bmatrix},
> $$
>
> then $\dfrac{\det(P_{n+1})}{\det(P_n)} =$ ________.
>
> 【100 台大資工】