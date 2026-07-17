## 可逆矩陣與 rank

令 $A$ 為 $m \times n$ 矩陣，則

> **定理**
>
> (1) $A$ 有左反矩陣 $\Leftrightarrow$ $A$ 各行向量線性獨立 $\Leftrightarrow \dim(CS(A)) = n$。
>
> 【99 成大資工】
>
> (2) $A$ 有右反矩陣 $\Leftrightarrow$ $A$ 各行向量張成 $R^m$ $\Leftrightarrow \dim(CS(A)) = m$。
>
> 【94 中興資工、99 各渠應數、99 成大資工】
>
> (3) $A$ 有反矩陣 $\Leftrightarrow$ $A$ 各行向量為 $F^{m \times n}$ 的一組基底。

> **【證明】**
>
> (1-a) 若 $A$ 有左反矩陣，則存在 $L \in F^{n \times m}$，使得 $LA = I$，故 $\text{rank}(LA) = \text{rank}(I) = n$，
>
> 又因 $\text{rank}(L) \leq \text{rank}(LA)$，故 $n \leq \text{rank}(A)$，
>
> 又 $\text{rank}(A) \leq n$，故 $\text{rank}(A) = n$。
>
> (1-b) $\Rightarrow$ 若 $\text{rank}(A) = n$，故 $\dim(RS(A)) = n$，因此 $A$ 各行向量為 $F^{n \times 1}$ 的一組基底，
>
> 又因 $\dim(F^{m \times n}) = m$，存在 $L \in F^{n \times m}$，使得 $LA = I_n$，
>
> 令 $y \in F^{m \times 1}$，存在 $e_i \in F^{n \times 1}$ 使 $y = A e_i$，即 $LAy = Le_i = e_i$，故 $LA = I$。
>
> （其他由此可以類推）

(2) 仿(1)可得。

(3) 由(1)(2)可得。
