# 3-1　向量空間

> **向量空間 (vector space) 的定義**
>
> 令 $V$ 為非空集合（其中的元素稱為向量），$F$ 為體（其中的元素稱為純量）
>
> 函數：$V \times V$ 定義為 $(u, v) = u + v$，稱向量加法 (vector addition)。
>
> 函數：$F \times V$ 定義為 $(a, u) = a \cdot u$，稱純量積 (scalar multiplication)。
>
> 則稱滿足下列八個特性的代數系統 $(V, +, \cdot)$ 為體 $F$ 的向量空間：
>
> (1) $\forall u, v, w \in V$，$(u + v) + w = u + (v + w)$。 向量加法具結合性
>
> (2) $\exists 0 \in V$，使 $\forall v \in V$，$v + 0 = 0 + v = v$。 其向量加法單位元有：$0$
>
> (3) $\forall v \in V$，$\exists -v \in V$，使 $v + (-v) = (-v) + v = 0$。 其向量加法反元素有：$-v$
>
> (4) $\forall u, v \in V$，$u + v = v + u$。 向量加法具交換性
>
> (5) $\forall \alpha \in F$，$u, v \in V$，$\alpha \cdot (u + v) = \alpha \cdot u + \alpha \cdot v$。 純量積對向量加法有分配性
>
> (6) $\forall \alpha, \beta \in F$，$v \in V$，$(\alpha + \beta) \cdot v = \alpha \cdot v + \beta \cdot v$。 純量對純量加法亦有分配性
>
> (7) $\forall \alpha, \beta \in F$，$v \in V$，$(\alpha \beta) \cdot v = \alpha \cdot (\beta \cdot v)$。 純量對純量乘法有結合性
>
> (8) $\forall v \in V$，$1v = v$。 單位純量的不變性
>
> （$1$ 為 $F$ 的乘法單位元素）
>
> 【92.94 中興資科、98 中興應數、99.100 成大數學、107 中山應數、108 成大統計】

> **Note**
>
> (1) 一般比較常討論的體為實數($R$)或複數($C$)，少數有討論到有限體。
>
> (2) 倘若 $F$ 的向量空間 $(V, +)$，常記成 $V_F$，也稱線性空間。
>
> (3) 向量空間中必含有零向量。
>
> (4) 上述性質(6)：左側的 $+$ 是純量加法；右側的 $+$ 是向量加法。
>
> (5) 上述性質(7)：左側的 $\alpha \beta$ 是用純量乘法；右側的 $\alpha \cdot (\beta \cdot v)$ 是純量積。