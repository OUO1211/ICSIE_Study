## 第 4 章 線性映射 571

## 4-5 不變子空間

> **不變子空間** (invariant subspace)
>
> 令 $T$ 為向量空間 $V$ 上的算子，$W$ 為 $V$ 的一個子空間，
> 若 $T(W) \subseteq W$，則稱 $W$ 為 $T$ 不變子空間。

例如：

令 $T: R^3 \to R^3$，$T(x,y,z) = (x+y, y+z, 0)$，

令 $S = \{(x, y, 0) \mid x, y \in R\}$；即 $xy$-平面，

則取 $(x,y,0) \in S$，得 $T(x,y,0) = (x+y, y, 0) \in S$，即 $T(S) \subseteq S$，

故 $S$ 為 $T$-不變子空間。

令 $W = \{(x, 0, 0) \mid x \in R\}$；即 $x$-軸，

則取 $(x,0,0) \in W$，得 $T(x,0,0) = (x,0,0) \in W$，即 $T(W) \subseteq W$，

故 $W$ 為 $T$-不變子空間。

> **Note**
>
> (1) $\{0\}$、$V$、$\ker(T)$、$\operatorname{Im}(T)$ 均為 $T$ 不變子空間，
>
> (2) 若 $W_1,\ldots,W_k$ 均為 $T$ 不變子空間，則
>
> (a) $W_1 + \cdots + W_k$ 為 $T$ 不變子空間。 【99 交大應數】
>
> **【證明】**
>
> 設 $w \in W_1 + W_2 + \cdots + W_k$，
>
> 令 $w = w_1 + w_2 + \cdots + w_k$，即 $w_i \in W_i$，for $1 \leq i \leq k$，
>
> $\because$ $W_i$ 為 $T$ 不變子空間，$\therefore T(W_i) \subseteq W_i$，for $1 \leq i \leq k$，$\therefore T(w_i) \in W_i$，for $1 \leq i \leq k$，
>
> $$T(w)=T(w_1+w_2+\cdots+w_k)=T(w_1)+T(w_2)+\cdots+T(w_k)$$
>
> $\therefore T(w) \in W_1 + W_2 + \cdots + W_k$，
>
> $\therefore T(W_1 + W_2 + \cdots + W_k) \subseteq W_1 + W_2 + \cdots + W_k$，
>
> $\therefore W_1 + W_2 + \cdots + W_k$ 為 $T$-不變子空間。
>
> (b) $W_1 \cap \cdots \cap W_k$ 為 $T$ 不變子空間。 【99 交大應數】
>
> **【證明】**
>
> 設 $w \in W_1 \cap W_2 \cap \cdots \cap W_k$，即 $w \in W_i$，for $1 \leq i \leq k$，
>
> $\because$ $W_i$ 為 $T$ 不變子空間，$\therefore T(W_i) \subseteq W_i$，for $1 \leq i \leq k$，
>
> $\therefore T(w) \in W_i$，for $1 \leq i \leq k$，
>
> $\therefore T(w) \in W_1 \cap W_2 \cap \cdots \cap W_k$，
>
> $\therefore T(W_1 \cap W_2 \cap \cdots \cap W_k) \subseteq W_1 \cap W_2 \cap \cdots \cap W_k$，
>
> $\therefore W_1 \cap W_2 \cap \cdots \cap W_k$ 為 $T$-不變子空間。