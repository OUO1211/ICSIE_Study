第 8 章 圖論1
13

\section*{度數（degree）}

考慮圖 $G=(V, E)$ ，$v$ 為 $G$ 上一點，
$G$ 為無向圖時，與點 $v$ 相連的邊數稱為點 $v$ 的度數，記為 $\operatorname{deg}(v)$ ；
$G$ 為有向圖時，連向點 $v$ 的邊數稱為 $v$ 的入度數（indegree），記為 $i d(v)$ 或 $\operatorname{indeg}(v)$ ；由 $v$ 連出去的邊數稱為 $v$ 的出度數（outdegree），記為 $\operatorname{od}(v)$ 或 $\operatorname{outdeg}(v)$ ；入度數與出度數的和稱為 $v$ 的度數。

Note
（1）無向圖中，若點 $v$ 多了一個 loop，則 $\operatorname{deg}(v)$ 增加2（有的書是寫增加1）。
（2）$G$ 中最小的度數記成 $\delta(G)$ ；最大的度數記成 $\Delta(G)$ 。
例如：圖 $G$ 中， $\operatorname{deg}(a)=0, \operatorname{deg}(b)=3, \operatorname{deg}(c)=1, \Delta(G)=3, \delta(G)=0$ ；
圖 $H$ 中， $\operatorname{id}(a)=1, \operatorname{od}(a)=0, \operatorname{id}(b)=1, \operatorname{od}(b)=2$ 。
\begin{itemize}
\item[（3）] 若 $G$ 為 $n$ 點簡單無向圖，則 $\forall x, \operatorname{deg}_G(x)+\operatorname{deg}_{\bar{G}}(x)=n-1$ 。
\item[（4）] 若每點度數都是 $k$ ，則稱 $G$ 為一 $k$－正則圖（ $k$－regular graph）。

2－regular

3－regular
\end{itemize}