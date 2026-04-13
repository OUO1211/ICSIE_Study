## 562 線性代數(上)

## 線性映射與保相依、保獨立、保生成

> 設 $T \in L(V, V')$，對 $V$ 的任意子集 $S$，
>
> (1) 若 $S$ 為 $V$ 的相依集，則 $T(S)$ 亦為 $V'$ 的相依集，則稱映 $T$ 保相依。
>
> (2) 若 $S$ 為 $V$ 的獨立集，則 $T(S)$ 亦為 $V'$ 的獨立集，則稱映 $T$ 保獨立。
>
> (3) 若 $S$ 為 $V$ 的生成集，則 $T(S)$ 亦為 $V'$ 的生成集，則稱映 $T$ 保生成。

> **Note**
>
> (1) 任意線性映射 $T$ 均保相依。 【重要】
>
> 【證明】
>
> 設 $S$ 為 $V$ 的一相依集，則存在 $v_1, \cdots, v_k \in S$，不全為零的純量 $\alpha_1, \cdots, \alpha_k$，使
>
> $$\sum_{i=1}^k \alpha_i v_i = 0,$$
>
> $$\therefore \sum_{i=1}^k \alpha_i T(v_i) = T\left(\sum_{i=1}^k \alpha_i v_i\right) = T(0) = 0。$$
>
> 即存在 $T(v_1), \cdots, T(v_k) \in T(S)$，不全為零的純量 $\alpha_1, \cdots, \alpha_k$，使
>
> $$\sum_{i=1}^k \alpha_i T(v_i) = 0。$$
>
> 故 $T(S)$ 為一相依集。
>
> (2) $T$ 為 1-1 $\Leftrightarrow$ $T$ 保獨立。 【重要】
>
> 【證明】
>
> $\Rightarrow$ 設 $T$ 為 1-1，
>
> 令 $S$ 為 $V$ 的一獨立集，
>
> 若 $\alpha_1 w_1 + \cdots + \alpha_k w_k = 0$，其中，$w_1, \cdots, w_k \in T(S)$
>
> 令 $w_i = T(v_i)$，其中 $v_i \in S$，
>
> 即 $\alpha_1 T(v_1) + \cdots + \alpha_k T(v_k) = T(\alpha_1 v_1 + \cdots + \alpha_k v_k) = 0$，
>
> $$\therefore \alpha_1 v_1 + \cdots + \alpha_k v_k \in \ker(T) = \{0\}, \cdots \text{因 } T \text{ 為 1-1},$$
>
> $$\therefore \alpha_1 v_1 + \cdots + \alpha_k v_k = 0。$$
>
> 又 $S$ 為獨立集，$\therefore \alpha_i = 0，\ \forall i，$
>
> $$\therefore T(S) \text{ 為一獨立集。}$$
>
> $\Leftarrow$ 任取 $v \in \ker(T)$
>
> 若 $v \ne 0$，則 $\{v\}$ 為獨立集，則 $\{T(v)\}$ 亦為獨立集，
>
> 但 $T(v) = 0$，矛盾
>
> $$\therefore \ker(T) = \{0\}，\text{故 } T \text{ 為 1-1。}$$
>
> (3) $T$ 為 onto $\Leftrightarrow$ $T$ 保生成。