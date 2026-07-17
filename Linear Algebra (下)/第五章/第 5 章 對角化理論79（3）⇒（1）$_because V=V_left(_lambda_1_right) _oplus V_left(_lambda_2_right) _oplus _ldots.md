第 5 章 對角化理論
79

（3）⇒（1）
$\because V=V\left(\lambda_1\right) \oplus V\left(\lambda_2\right) \oplus \ldots \oplus V\left(\lambda_r\right)$ ，且 $V\left(\lambda_i\right)$ 為 $T-$ 不變子空間，$\forall i=1,2, \ldots, r$ ，故取 $V\left(\lambda_i\right)$ 的一組基底 $\beta_i$ ，
則 $\beta=\beta_1 \cup \beta_2 \cup \cdots \cup \beta_r$ 為 $V$ 的一組基底且使 $[T]_\beta=\left[\begin{array}{llll}A_1 & & & O \\ & A_2 & & \\ & & \ddots & \\ O & & & A_r\end{array}\right]$ ，
其中 $A_i=\left[T_{V\left(\lambda_i\right)}\right]_{\beta_i}=\left[\begin{array}{llll}\lambda_i & & & O \\ & \lambda_i & & \\ & & \ddots & \\ O & & & \lambda_i\end{array}\right]=\lambda_i I_{m_i}, \operatorname{dim}\left(V\left(\lambda_i\right)\right)=m_i, i=1,2, \ldots, r$,
故 $[T]_\beta$ 為對角方陣，所以 $T$ 可以對角化．

Note
（1）此處對線性算子所討論的定義與性質，對方陣討論時亦可成立。
（2）若 $A \in F^{n \times n}$（或 $T \in L(V, V), \operatorname{dim}(V)=n$ ）有 $n$ 個相異的特徵根，則 $A$（或 $T$ ）可對角化．
【證明】
【重要】
設 $\lambda_1, \lambda_2, \ldots, \lambda_n$ 為 $A$ 的相異特徵根，
則 $m\left(\lambda_i\right)=1, \forall i=1,2, \ldots, n$ ，
$$
\because 1 \leq g m\left(\lambda_i\right) \leq m\left(\lambda_i\right) \leq n, \forall i=1,2, \ldots, n,
$$

故得 $g m\left(\lambda_i\right)=1, \forall i=1,2, \ldots, n$ ，
故 $A$ 可對角化．
（3）$\left[\begin{array}{ll}1 & 0 \\ 1 & 1\end{array}\right],\left[\begin{array}{ll}0 & 0 \\ 1 & 0\end{array}\right]$ 都不可對角化．
【重要】
（4）若 $A$ 的獨立特徵向量個數不到 $n$ 個（也即為 $A$ 不可對角化），稱 $n$ 階方陣 $A$ 為 defective。