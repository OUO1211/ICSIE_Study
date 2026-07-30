第10章 樹 221
\begin{itemize}
\item[] $$
\because d_1+d_2+\ldots+d_{k+1}=2 k,
$$
由鸽籠原理知必有某 $d_i=1$ ，令其為 $d_1$ ；且必有某 $d_j \geq 2$ ，令其為 $d_{k+1}$ ，
則因為 $d_2+d_3+\ldots+\left(d_{k+1}-1\right)=2(k-1)$ ，
由歸納假設知，必存在有一樹 $T$ 其度數序列為：$d_2, d_3, \ldots, d_{k+1}-1$ ，
則再把一點連到 $T$ 中度數為 $d_{k+1}-1$ 的點，就得到度數序列為 $d_1, d_2, \ldots, d_{k+1}$ 的樹了。
\item[（5）] Every tree with a vertex of degree $k$ has at least $k$ leaves．
【103 清大資工】
【證明】
對 $k$ 以歸納法討論如下：
$k=1$ 時即此樹有一個度數1的點，此即為一葉子，所以原樹至少一葉子，原命題成立。設原命題對 $k \geq 1$ 均成立，
則若樹 $T$ 有度數 $k+1$ 的點 $x$ ，去掉 $x$ 上的任一邊 $(x, y)$ ，得兩個樹，$T_1 、 T_2$ ，設 $x \in V\left(T_1\right), y \in V\left(T_2\right)$ ，且 $\operatorname{deg}_{T_1}(x)=k$ ，
根據歸納假設，$T_1$ 有至少 $k$ 個葉子，（而這 $k$ 個葉子也是 $T$ 的葉子）
另一方面，
若 $T_2$ 只有點 $y$ ，則 $y$ 亦為 $T$ 的葉子，所以 $T$ 有至少 $k+1$ 個葉子；
若 $T_2$ 不只有點 $y$ ，則 $\operatorname{deg}_{T_2}(y) \geq 1$ ，根據歸納假設，$T_2$ 有至少1個葉子（而這葉子也是 $T$的葉子），所以 $T$ 有至少 $k+1$ 個葉子。
\item[（6）] 非退化樹 $T$ 中有 $2+\sum_{\operatorname{deg}\left(v_i\right) \geq 3}\left(\operatorname{deg}\left(v_i\right)-2\right)$ 個葉子。
【94 政大資科】
【證明】
設度數為 $i$ 的點有 $n_i$ 個，則 $\sum_{i=1}^{\Delta} n_i=n$ 且 $\sum_{i=1}^{\Delta} i \cdot n_i=\sum_{i=1}^n \operatorname{deg} v_i$ ，其中 $\Delta$ 為最大度數。
$$
\begin{aligned}
& \text { 又 } \because \sum_{i=1}^n \operatorname{deg} v_i=2|E|=2 n-2, \\
& \therefore 1 \cdot n_1+2 \cdot n_2+3 \cdot n_3+\ldots+\Delta \cdot n_{\Delta}=2\left(n_1+n_2+\ldots+n_{\Delta}\right)-2, ~ \\
& \therefore n_1=2+(3-2) n_3+(4-2) n_4+\ldots+(\Delta-2) n_{\Delta} \\
& \quad=2+\sum_{k=3}^{\Delta}(k-2) n_k=2+\sum_{\operatorname{deg} v_i \geq 3}\left(\operatorname{deg} v_i-2\right) .
\end{aligned}
$$
\end{itemize}