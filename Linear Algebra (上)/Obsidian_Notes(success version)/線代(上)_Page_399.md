## rank 的性質一進階版

> **例題**
>
> Let $A$ be a $m \times n$ real matrix, $B$ a $n \times p$ real matrices.
>
> (1) Prove that $\text{rank}(AB) \geq \text{rank}(A) + \text{rank}(B) - n$.
>
> 【89 交大進數、92 清大應數、93 103 高長應數、99 中處統計、110 台大數學】
>
> (2) Use (1) to show that if $A_1, \ldots, A_k$ are $n \times n$ real matrices satisfying $A_1 A_2 \cdots A_k = O$，則 $\text{rank}(A_1) + \cdots + \text{rank}(A_k) \leq (k-1)n$。
>
> 【92 清大數學】

解：

(1) $\text{rank}\begin{pmatrix} A & B \\ O & AB \end{pmatrix} \geq \text{rank}\begin{pmatrix} I_n & B \\ O & O \end{pmatrix} \cdot \text{rank}\begin{pmatrix} A \\ O \end{pmatrix}$，

又 $\text{rank}\begin{pmatrix} A \\ O & AB \end{pmatrix} = n + \text{rank}(B)$，故得

$\geq 2 \cdot \text{rank}(B) + \text{rank}(-A) = \text{rank}(B) + \text{rank}(A)$，

故得 $n + \text{rank}(AB) \geq \text{rank}(A) + \text{rank}(B)$，即 $\text{rank}(AB) \geq \text{rank}(A) + \text{rank}(B) - n$。

(2) $\text{rank}(A_1) + \text{rank}(A_2) \leq \text{rank}(A_1 A_2) + n$

故得 $\text{rank}(A_1 A_2) \leq \text{rank}(A_1 A_2 A_3) + n$

$\leq n + \text{rank}(A_1) + \text{rank}(A_2) + \cdots + \text{rank}(A_k)$

$\leq (k-3)n + \text{rank}(A_{k-2} A_{k-1} A_k) + \cdots + (k-1) n$。
