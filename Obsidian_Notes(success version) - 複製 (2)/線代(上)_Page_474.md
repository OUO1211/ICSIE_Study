# 4-2 線性映射的矩陣表示

## 矩陣表示(matrix representation)

> **定義**
>
> 考慮有限向量空間 $V$、$V'$，若函數 $T: V \to V'$ 為線性映射，令 $\beta = \{\beta_1, \beta_2, \ldots, \beta_n\}$ 為 $V$ 的一組有序基底，令 $\gamma$ 為 $V'$ 的一組有序基底，令 $A = [[T(\beta_1)]_\gamma, [T(\beta_2)]_\gamma, \ldots, [T(\beta_n)]_\gamma]$，
>
> 則稱 $A$ 為 $T$ 的 $\beta$ 到 $\gamma$ 的**矩陣表示**，也記做 $[T]_\beta^\gamma$。

> **Note**
>
> (1) 若 $\beta$ 及 $\gamma$ 均為標準基底，則 $[T]_\beta^\gamma$ 又稱為 $T$ 的**標準矩陣表示**。
>
> (2) 當 $F = V = V'$ 時，$[T]_\beta^\beta$ 記做 $[T]_\beta$；線性算子 $T: V \to V$ 的矩陣表示也稱為 $T$ 的矩陣。
>
> (3) 若 $\beta$ 及 $\gamma$ 分別為 $V$、$V'$ 上的有序基底，$T \in L(V, V')$，那麼有了第二章的基底變換，就可以進一步計算不同基底下 $T$ 的矩陣表示法 $[T]_\beta^\gamma$。
