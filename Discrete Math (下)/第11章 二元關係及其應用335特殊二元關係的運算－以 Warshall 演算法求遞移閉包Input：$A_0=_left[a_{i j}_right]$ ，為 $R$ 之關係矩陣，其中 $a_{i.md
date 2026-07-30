第11章 二元關係及其應用
335

特殊二元關係的運算－以 Warshall 演算法求遞移閉包
Input：$A_0=\left[a_{i j}\right]$ ，為 $R$ 之關係矩陣，其中 $a_{i j}= \begin{cases}0 & \text { if }(i, j) \notin R \\ 1 & \text { if }(i, j) \in R\end{cases}$
Output：transitive closure of $R$
For $k=1$ to $n$ do
$$
A_k[i, j] \leftarrow\left(A_{k-1}[i, j] \vee\left(A_{k-1}[i, k] \wedge A_{k-1}[k, j]\right)\right), \quad \forall i, j
$$
Return $A_n$ ．
【重要】