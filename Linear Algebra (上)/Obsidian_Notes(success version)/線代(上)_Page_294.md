## 和空間的生成集

> **定理**
> 若 $W_1 = span(S_1)$，$W_2 = span(S_2)$，則 $W_1 + W_2 = span(S_1 \cup S_2)$。
> （即 $span(S_1) + span(S_2) = span(S_1 \cup S_2)$）

**【證明】**

$(\subseteq)$：$W_1 = span(S_1) \subseteq span(S_1 \cup S_2)$，$W_2 = span(S_2) \subseteq span(S_1 \cup S_2)$，
且 $W_1, W_2, span(S_1 \cup S_2)$ 均為 $V$ 的子空間，$\therefore W_1 \subseteq span(S_1 \cup S_2)$，$W_2 \subseteq span(S_1 \cup S_2)$，
$\therefore W_1 + W_2 \subseteq span(S_1 \cup S_2)$。

$(\supseteq)$：設 $u \in span(S_1 \cup S_2)$，
即存在向量 $v_1, \ldots, v_k \in S_1 \cup S_2$，純量 $\alpha_1, \ldots, \alpha_k$，使 $u = \alpha_1 v_1 + \ldots + \alpha_k v_k$，

(1) 若 $v_1, \ldots, v_k \in S_1$，則 $u \in span(S_1)$，則 $u = u + \mathbf{0} \in span(S_1) + span(S_2)$，

(2) 若 $v_1, \ldots, v_k \in S_2$，則 $u \in span(S_2)$，則 $u = \mathbf{0} + u \in span(S_1) + span(S_2)$，

(3) 設 $v_1, \ldots, v_j \in S_1$，$v_{j+1}, \ldots, v_k \in S_2$，則 $\sum_{i=1}^{j} \alpha_i v_i \in span(S_1)$，$\sum_{i=j+1}^{k} \alpha_i v_i \in span(S_2)$，

$\therefore u \in span(S_1) + span(S_2)$，
故 $span(S_1 \cup S_2) \subseteq span(S_1) + span(S_2)$。

> **Note**
>
> 由上述性質可得知，到劃 $W_1 + W_2$ 時，先個別取生成集，然後聯集即可。
>
> 例如：$V = \mathbb{R}^{2 \times 2}$，$W_1 = \left\{ \begin{bmatrix} x & 0 \\ 0 & x \end{bmatrix} \mid x \in \mathbb{R} \right\}$，$W_2 = \left\{ \begin{bmatrix} x & x+y \\ 0 & y \end{bmatrix} \mid x, y \in \mathbb{R} \right\}$，即可如下討論 $W_1 + W_2$：
>
> $$W_1 = span\left\{ \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} \right\}, \quad W_2 = span\left\{ \begin{bmatrix} 1 & 1 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 1 \\ 0 & 1 \end{bmatrix} \right\}$$
>
> $$\therefore W_1 + W_2 = span\left\{ \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}, \begin{bmatrix} 1 & 1 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 1 \\ 0 & 1 \end{bmatrix} \right\}$$
>
> $$= \left\{ a\begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} + b\begin{bmatrix} 1 & 1 \\ 0 & 0 \end{bmatrix} + c\begin{bmatrix} 0 & 1 \\ 0 & 1 \end{bmatrix} \mid a, b, c \in \mathbb{R} \right\}$$
>
> $$= \left\{ \begin{bmatrix} a+b & b+c \\ 0 & a+c \end{bmatrix} \mid a, b, c \in \mathbb{R} \right\} = \left\{ \begin{bmatrix} x & y \\ 0 & z \end{bmatrix} \mid x, y, z \in \mathbb{R} \right\}$$
