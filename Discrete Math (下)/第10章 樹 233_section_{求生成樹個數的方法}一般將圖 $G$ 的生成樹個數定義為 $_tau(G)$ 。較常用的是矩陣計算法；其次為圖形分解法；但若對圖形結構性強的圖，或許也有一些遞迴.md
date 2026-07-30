第10章 樹 233

\section*{求生成樹個數的方法}

一般將圖 $G$ 的生成樹個數定義為 $\tau(G)$ 。較常用的是矩陣計算法；其次為圖形分解法；但若對圖形結構性強的圖，或許也有一些遞迴關係式，或特殊编碼的方式可導出再求解；而對一些簡易的圖，或者就暴力法直接硬算了。

\section*{矩陣計算法（Matrix－Tree theorem 、Kirchhoff Theorem）}

考虑 $n$ 點連通圖 $G$ ，其 Laplace 矩陣 $M=\left[m_{i j}\right]_{n \times n}, m_{i j}= \begin{cases}\operatorname{deg}\left(v_{i j}\right) & i=j \\ 0 & i \neq j, v_i, v_j \text { 不相鄰 } \\ -1 & i \neq j, v_i, v_j \text { 相鄰 }\end{cases}$則 $M$ 的所有元素之餘因子（cofactor）皆相同，且其值即 $\tau(G)$ 。

Note
設 $a_{i j} \in M_{n \times n}$ ，則 $a_{i j}$ 之餘因子： $\operatorname{cofactor}\left(a_{i j}\right)=(-1)^{i+j} \cdot \operatorname{det}\left(M_{i j}\right)$ ，
其中，$M_{i j}$ 為將 $M$ 去掉第 $i$ 列，第 $j$ 行所得之 $(n-1) \times(n-1)$ 矩陣。

例如：欲求 $K_{3,3}$ 中有多少相異的生成樹？
$K_{3,3}$ 之 Laplace 矩陣為 $\left[\begin{array}{cccccc}3 & 0 & 0 & -1 & -1 & -1 \\ 0 & 3 & 0 & -1 & -1 & -1 \\ 0 & 0 & 3 & -1 & -1 & -1 \\ -1 & -1 & -1 & 3 & 0 & 0 \\ -1 & -1 & -1 & 0 & 3 & 0 \\ -1 & -1 & -1 & 0 & 0 & 3\end{array}\right]$ ，
cofactor $\left(a_{11}\right)=(-1)^{1+1} \cdot\left|\begin{array}{ccccc}3 & 0 & -1 & -1 & -1 \\ 0 & 3 & -1 & -1 & -1 \\ -1 & -1 & 3 & 0 & 0 \\ -1 & -1 & 0 & 3 & 0 \\ -1 & -1 & 0 & 0 & 3\end{array}\right|=81$ ，
所以共有 81 個相異的 spanning tree．