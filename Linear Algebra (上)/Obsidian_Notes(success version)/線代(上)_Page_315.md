## 3-3 基底與維度

### 基底(basis)與維度(dimension)

考慮向量空間 $V$ 的一子集 $S$，若 $S$ 滿足：
(1) $span(S) = V$，(2) $S$ 為獨立集，
則稱 $S$ 為 $V$ 的一組基底，且 $S$ 中的向量個數稱作 $V$ 的維度，記做 $\dim(V)$。

例如：
可取 $\{(1,1),(1,0)\}$ 為 $\mathbb{R}^2$ 的一組基底且 $\dim(\mathbb{R}^2) = 2$。
也可取 $\{(1,0),(0,1)\}$ 為 $\mathbb{R}^2$ 的一組基底且 $\dim(\mathbb{R}^2) = 2$。
可取 $\left\{ \begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 1 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 \\ 1 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 \\ 0 & 1 \end{bmatrix} \right\}$ 為 $\mathbb{R}^{2\times 2}$ 的一組基底，$a, b \in \mathbb{R}$ 的一組基底且 $\dim(\mathbb{R}^{2\times 2}) = 2$。

> **Note**
>
> (1) 若向量空間的基底是有限集，則稱此向量空間為有限維向量空間；否則稱為無限維向量空間。
>
> (2) $V$ 的任一組基底元素個數均相同（此性質我們後述）。
>
> (3) 空集合為零空間 $\{0\}$ 的唯一基底且 $\dim(\{0\}) = 0$。
>
> (4) 考慮空零空間 $V$ 的行子空間的任意一組基底，若 $S$ 為 $F$ 的一組基底則 $V$ 中的任意向量均可由 $S$ 唯一線性組合。

【101 成大數學】

**【定理】**

$(a)$ 設 $span(S) = V$，取 $v \in V$，取 $\alpha_1, \alpha_2, \ldots, \alpha_k \in F$，使 $v = \alpha_1 v_1 + \alpha_2 v_2 + \cdots + \alpha_k v_k$，

若若 $X$ 亦是另外的 $\beta_1 v_1 + \beta_2 v_2 + \cdots + \beta_k v_k$，

則由 $v - v = (\alpha_1 - \beta_1)v_1 + (\alpha_2 - \beta_2)v_2 + \cdots + (\alpha_k - \beta_k)v_k = 0$，

故因 $\{v_1, v_2, \ldots, v_k\}$ 為獨立集，故得 $\alpha_1 - \beta_1 = 0$，即 $\alpha_1 = \beta_1$，$i = 1, \ldots, k$，

故 $\{v_1, \ldots, v_k\}$ 為獨立集，代得 $v \in V$ 為 $S$ 的線性組合。

$(b)$ 由此繼續推 $span(S) = V$，依得 $S \subseteq V$，

則 $F$ 中的向量 $0v_1 + 0v_2 + \cdots + 0v_k = 0$，故得 $S$ 為獨立集。

例：$F$ 中向量 $0v_1 + \cdots = 0$，

且 $F$ 中的向量 $v \in V$ 為 $S$ 的線性組合，故得 $S$ 為獨立集。
