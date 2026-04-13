## 第 4 章 線性映射 527

## 4-3 線性映射的核空間與值域

> **定義** (direct image)與反像(inverse image)
>
> 令 $S$ 為向量空間 $V$ 的子集合，$F$ 的函數，且 $T:A \to B$ 為 $F$ 的一線性映射。
>
> 定義 $T(S) = \{T(v) \mid v \in S\}$ 稱為 $S$ 在 $F$ 的正向直像。
>
> 定義 $T^{-1}(S) = \{v \in V \mid T(v) \in S\}$ 稱為 $S$ 在 $F$ 的反像。

**Note**

(1) 此處 $T^{-1}$ 並非指了的反函數，稱為其反圖像對應集。

(2) $T(S) \subseteq T$；$T^{-1}(S) \subseteq V$。

(3) 線性映射保留子空間：即 $T$ 為 $T \in L(V, V')$，則

(a) 若 $W$ 為 $V$ 的一子空間，則 $T(W)$ 為 $V'$ 的一子空間

(b) 若 $W'$ 為 $V'$ 的一子空間，則 $T^{-1}(W')$ 為 $V$ 的一子空間

> **【證明】**
>
> (a) $T(W) \subseteq V'$，且：$0 = T(0) \in T(W)$，$T(W) \neq \emptyset$。
>
> 又 $\forall u, \forall w \in T(W)$，存在 $x, y \in W$，使得 $T(x) = u$，$T(y) = w$，
>
> 則 $u + w$ 為 $V'$ 的子空間，$au + w \in W'$，$T(ax + y) \in T(W)$，$\therefore T(x) + T(y) \in T(W)$
>
> 故 $T(W)$ 為 $V'$ 的子空間。
>
> (b) $T^{-1}(W')$ 為 $V$ 的一子空間，且 $T^{-1}(W') \subseteq V$
>
> $\forall u, \forall w \in T^{-1}(W')$，故 $T(u), T(w) \in W'$，
>
> $\Rightarrow a \cdot T(u) + T(w) = T(au + w) \in W'$
>
> $\therefore au + w \in T^{-1}(W')$，故 $T^{-1}(W')$ 為 $V$ 的一子空間。
