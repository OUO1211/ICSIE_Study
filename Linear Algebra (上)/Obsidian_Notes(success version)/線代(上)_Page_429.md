# 3-6 空間直和

## 獨立子空間

> 考慮向量空間 $V$ 上的子空間 $W_1, W_2, \ldots, W_k$，
>
> 若 $W_i \cap \sum_{j \ne i} W_j = \{0\}$，$\forall i = 1, 2, \ldots, k$，
>
> 則稱 $W_1, W_2, \ldots, W_k$ 為獨立子空間。

> 例如，$k = 3$ 時，若 $W_1, W_2, W_3$ 滿足：
>
> $W_1 \cap (W_2 + W_3) = \{0\}$，$W_2 \cap (W_3 + W_1) = \{0\}$，$W_3 \cap (W_1 + W_2) = \{0\}$，
>
> 則稱 $W_1, W_2, W_3$ 為獨立子空間。

> **Note**
>
> (1) 若 $W_i \cap W_j = \{0\}$，$\forall i \ne j$，則稱 $W_1, W_2, \ldots, W_k$ 為兩兩獨立（pairwise independent）。
>
> (2) 若 $W_1, W_2, \ldots, W_k$ 獨立子空間，則 $W_1, W_2, \ldots, W_k$ 為兩兩獨立。
>
> (3) 設 $k \geq 3$，若 $W_1, W_2, \ldots, W_k$ 為兩兩獨立，則 $W_1, W_2, \ldots, W_k$ 不一定為獨立子空間。
>
> 例如取 $V = R^3$，$W_1 = x$-軸，$W_2 = y$-軸，$W_3$：直線 $x = y$。
>
> (4) 等價定義 考慮向量空間 $V$，$W_1, W_2, \ldots, W_k \subset V$，
>
> $W_1, W_2, \ldots, W_k$ 為獨立子空間
>
> $\Leftrightarrow$ $\forall w_i \in W_i$，$1 \leq i \leq k$，若 $w_1 + w_2 + \cdots + w_k = 0$，則 $w_1 = w_2 = \cdots = w_k = 0$。
>
> $\Leftrightarrow$ $\dim(W_1 + W_2 + \cdots + W_k) = \dim(W_1) + \dim(W_2) + \cdots + \dim(W_k)$。