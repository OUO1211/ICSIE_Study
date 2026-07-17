## 生成空間 (span) 與生成集 (spanning set, generating set)

> 考慮向量空間 $V$ 下的子集 $S$，
>
> 稱 $\text{span}(S)$ 為 $S$ 中的所有元素的有限線性組合 $\}$ 為 $S$ 的生成空間，也稱 $S$ 為 $\text{span}(S)$ 的一個生成集。

**例如：**

(1) $\text{span}\{(1, 0)\} = \{a(1, 0) \mid a \in R\} = \{(a, 0) \mid a \in R\} = x$ 軸。

(2) $\text{span}\{(1, 0), (0, 1)\} = \{a(1, 0) + b(0, 1) \mid a, b \in R\} = xy\text{-plane}$。

(3) $\text{span}\left\{ \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \begin{bmatrix} 0 \\ 0 \end{bmatrix}, \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \begin{bmatrix} 0 \\ 0 \end{bmatrix}, \begin{bmatrix} 1 & 1 \\ 0 & 0 \end{bmatrix} \right\}$ 都是 $\left\{ \begin{bmatrix} a & a \\ b & b \end{bmatrix} \mid a, b \in R \right\}$ 的生成集。

> **Note**
>
> (1) $\text{span}(\emptyset) = \{0\}$：零空間；且定義 $\text{span}(\emptyset) = \{0\}$：零空間。
>
> (2) 由定義可知，$\text{span}(S)$ 滿足封閉條件和純量積的封閉性，故為 $V$ 的一子空間。

****

若 $S = \emptyset$，則 $\text{span}(S) = \{0\}$，為 $V$ 的子空間。

若 $S \neq \emptyset$，則存在 $w \in S$，因此 $0w = 0w = 0 \in \text{span}(S)$，所以 $\text{span}(S) \neq \emptyset$。

又 $\forall a \in F$，$u, v \in \text{span}(S)$，

存在 $a_1, a_2, \ldots, a_m, \beta_1, \beta_2, \ldots, \beta_n, s_1, \ldots, s_n \in S$，使得

$u = a_1 s_{i_1} + a_2 s_{i_2} + \cdots + a_m s_{i_m}$，$v = \beta_1 s_{j_1} + \beta_2 s_{j_2} + \cdots + \beta_n s_{j_n}$，

使得 $a \cdot u + v = a a_1 s_{i_1} + a a_2 s_{i_2} + \cdots + a a_m s_{i_m} + \beta_1 s_{j_1} + \cdots + \beta_n s_{j_n} \in \text{span}(S)$，

即 $\text{span}(S)$ 為 $V$ 的子空間。

(3) 若 $A$ 為 $m \times n$，則 $RS(A) = \text{span}\{A_{r_1}, A_{r_2}, \ldots, A_{r_m}\}$；$CS(A) = \text{span}\{A^{(1)}, A^{(2)}, \ldots, A^{(n)}\}$。