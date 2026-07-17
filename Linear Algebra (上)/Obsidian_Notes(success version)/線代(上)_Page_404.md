## 特殊矩陣的 rank－$A = xy^T$

> **定理**
>
> Let $x$ and $y$ be nonzero vectors in $R^m$ and $R^n$, respectively, and let $A = xy^T$.
>
> (1) Find the column space of $A$. What is $\text{rank}(A)$?
>
> (2) Find the null space of $A$. What is its dimension?
>
> 【94 中央數學、94 交大電資、107 台科資工】

解：

(1) $\text{rank}(xy^T) \leq \text{rank}(x) \cdot \text{rank}(y) = 1$，

又因為 $A$ 不為零矩陣，故 $\text{rank}(A) = 1$，

又因 $CS(A) = \{x : x = Ay\} = \text{span}\{x\}$。

(2) $\ker(A) = \{v : Av = 0\} = \{v : xy^T v = 0\} = \{v : x(y^T v) = 0\} = \{v : y^T v = 0\}$（因 $x \neq 0$）

又 $\dim(\ker(A)) = n - \dim(CS(A)) = n - 1$。

> **例題**
>
> (10%) Let $A$ be an $n \times n$ matrix. Prove that if $\text{rank}(A) = 1$, then there exist two $n \times 1$ vectors $x$ and $y$ such that $A = xy^T$.
>
> 【92 成大進數、94 中央數學、99 各渠計數、107 台科資工】

解：

故 $A$ 的列空間以 $A$ 的某些非零列生成，且 $A$ 的其他列都是此列的係數倍，

令 $A_{i,\cdot}$ 為此非零列，設為 $a_{i_0}$，

$$x = \begin{bmatrix} a_1 \\ a_2 \\ \vdots \\ a_n \end{bmatrix} \in R^{n \times 1},\quad y^T = \begin{bmatrix} A_{i_0,1} & A_{i_0,2} & \cdots & A_{i_0,n} \end{bmatrix}$$

則 $xy^T = A$，其中 $A_{j,\cdot} = a_j A_{i_0,\cdot}$，$j = 1, 2, \ldots, n$，

$$A = \begin{bmatrix} a_1 A_{i_0} \\ a_2 A_{i_0} \\ \vdots \\ a_n A_{i_0} \end{bmatrix} = \begin{bmatrix} a_1 \\ a_2 \\ \vdots \\ a_n \end{bmatrix} A_{i_0} = xy^T$$
