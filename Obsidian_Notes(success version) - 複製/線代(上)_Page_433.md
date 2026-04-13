# 3-7 進階試題練習

> **試題 1**
>
> Show that the set $R^+$ of positive real is a linear space when "$x + y$" is interpreted to mean the product of $x$ and $y$ (so that $2 + 3$ is 6), and "$r \cdot x$" is interpreted as the $r$-th power of $x$.
>
> 【94 暨南資工、100 交大資工、103 成大數學】

解：即證明 $(R^+, +, \cdot)$ 為一個向量空間，其中 $x + y = xy$，$r \cdot x = x^r$，

(1) 向量加法具結合性：

$\forall u, v, w \in R^+$，$(u + v) + w = (uv)w = u(vw) = u + (v + w)$。

(2) 具零元素 $0 \in R^+$（即乘法單位元 $1$）：

$\forall v \in R^+$，取加法零元素為 $1$，則 $v + 1 = v \cdot 1 = v = 1 \cdot v = 1 + v$。

(3) 向量加法反元素存在：

$\forall v \in R^+$，取 $-v = \dfrac{1}{v}$，則 $v + (-v) = v \cdot \dfrac{1}{v} = 1 = 0$（加法單位元）。

(4) 向量加法具交換性：

$\forall u, v \in R^+$，$u + v = uv = vu = v + u$。

(5) 純量乘積對向量加法有分配性：

$\forall \alpha \in R$，$u, v \in R^+$，$\alpha(u + v) = (uv)^\alpha = u^\alpha v^\alpha = (\alpha \cdot u) + (\alpha \cdot v)$。

(6) 純量乘積對純量加法有分配性：

$\forall \alpha, \beta \in R$，$v \in R^+$，$(\alpha + \beta) \cdot v = v^{\alpha + \beta} = v^\alpha \cdot v^\beta = (\alpha \cdot v) + (\beta \cdot v)$。

(7) 純量乘積純量乘法具結合性：

$\forall \alpha, \beta \in R$，$v \in R^+$，$(\alpha\beta) \cdot v = v^{\alpha\beta} = (v^\beta)^\alpha = \alpha \cdot (\beta \cdot v)$。

(8) 單位純量乘積的不變性：

$\forall v \in R^+$，$1 \cdot v = v^1 = v$。

故 $(R^+, +, \cdot)$ 為佈於 $R$ 的向量空間。
