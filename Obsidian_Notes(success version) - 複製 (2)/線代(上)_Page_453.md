## 線性映射的存在性與唯一性

> **定理**
>
> 令 $\beta = \{b_1, b_2, \ldots, b_n\}$ 為向量空間 $V$ 之一基底，令 $T \in L(V, V')$，則
>
> (1) 若 $T, U \in L(V, V')$，則 $T(b_i) = U(b_i)$ $\Rightarrow$ $T = U$。
>
> (2) 若 $T$ 為任意元素，$\{w_1, w_2, \ldots, w_n\}$ 為向量空間 $V'$ 中的任意 $n$ 個向量，則唯一一個線性映射 $T: V \to V'$ 使得 $T(b_i) = w_i$，$\forall i = 1, 2, \ldots, n$，
>
> 且其唯一性即由 $T(v) = \sum a_i T(b_i)$ 決定。

> **【證明】**
>
> (1) $\Rightarrow$ 明顯成立：
>
> $\forall v \in V$，令 $v = \sum a_i b_i$，
>
> 則 $T(v) = T\left(\sum a_i b_i\right) = \sum a_i T(b_i) = \sum a_i U(b_i) = U\left(\sum a_i b_i\right) = U(v)$，
>
> 故得 $T = U$。
>
> (2) 因為 $\beta = \{b_1, b_2, \ldots, b_n\}$ 為 $V$ 之一基底，故 $\forall v \in V$，可表示為 $v = \sum a_i b_i$。
>
> 定義函數 $T: V \to V'$ 為 $T(v) = \sum a_i w_i$，以下計算函數的唯一性如下述：
>
> (i) 對 $i = 1, 2, \ldots, n$，$\because$ $b_i = 0b_1 + \cdots + 0b_{i-1} + 1b_i + 0b_{i+1} + \cdots + 0b_n$，
>
> 故 $T(b_i) = 0w_1 + \cdots + 0w_{i-1} + 1w_i + \cdots + 0w_n = w_i$。
>
> (ii) 再驗 $T$ 為線性映射：
>
> $\forall u, v \in V$，$\alpha \in F$，令 $u = \sum a_i b_i$，$v = \sum \beta_i b_i$，
>
> 則 $T(\alpha u + v) = T\left(\sum (\alpha a_i + \beta_i) b_i\right) = \sum (\alpha a_i + \beta_i) w_i$
>
> $= \alpha \sum a_i w_i + \sum \beta_i w_i = \alpha T(u) + T(v)$，
>
> 故 $T$ 為一線性映射。
