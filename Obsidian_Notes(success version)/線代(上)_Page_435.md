> **試題 3**
>
> (15%) Let $R$ denote the set of real numbers. Show that $R$, together with the usual addition and scalar multiplication of real numbers, is a vector space.
>
> 【108 分大資工】

解：即證明 $(R, +, \cdot)$ 為一個向量空間，

(1) 向量加法具結合性：

$\forall u, v, w \in R$，$(u + v) + w = u + (v + w)$（實數加法結合律）。

(2) 具零元素 $0 \in R$：

$\forall v \in R$，$v + 0 = v = 0 + v$。

(3) 向量加法法反元素：

$\forall v \in R$，取 $-v \in R$，則 $v + (-v) = 0 = (-v) + v$。

(4) 向量加法具交換性：

$\forall u, v \in R$，$u + v = v + u$。

(5) 純量乘積對向量加法有分配性：

$\forall \alpha \in R$，$u, v \in R$，$\alpha(u + v) = \alpha u + \alpha v$。

(6) 純量乘積對純量加法有分配性：

$\forall \alpha, \beta \in R$，$v \in R$，$(\alpha + \beta) \cdot v = \alpha v + \beta v$。

$(R, +, \cdot)$ 為佈於 $R$ 的向量空間。

> **試題 4**
>
> (15%) Given an infinite sequence $a_1, a_2, \ldots$, in $R$, we write the sequence by $\{a_n\}_{n \geq 1}$. Let $R^\infty$ denote the set of vectors over $R$ with vector addition $+$ and scalar multiplication, denote by $\lambda\{a_n\}_{n \geq 1} = \{\lambda a_n\}_{n \geq 1}$ for all $\lambda \in R$.
>
> Show that $R^\infty$ is an infinite-dimensional vector space over $R$.
>
> 【108 中央教學】

解：即證明 $(R^\infty, +, \cdot)$ 為一個向量空間：

(1) 向量加法具結合性：

$\forall \{a_n\}, \{b_n\}, \{c_n\} \in R^\infty$，$(\{a_n\} + \{b_n\}) + \{c_n\} = \{a_n\} + (\{b_n\} + \{c_n\})$。

(2) 具零元素 $\{0\} = \{0_n\} \in R^\infty$，全部分量均為 $0$。

$\forall v = \{a_n\} \in R^\infty$，$v + \{0\} = \{a_n + 0\} = \{a_n\} = v$，$\{0\} + v = v$。
