第 8 章 圖論1
31

\section*{8－3 完全與獨立}

\section*{完全圖（complete graph）}

對正整數 $n$ ，定義完全圖 $K_n$ 為一 $n$ 點無向圖且滿足任兩點恰一邊相連。

Note
\begin{itemize}
\item[（1）] $\left|E\left(K_n\right)\right|=\binom{n}{2}$ ，且 $\forall x \in V\left(K_n\right), \operatorname{deg}(x)=n-1$ 。【96 宜蘭資工】【102中央資工】
\item[（2）] 若對 $K_n$ 的每邊任給方向，即得有向完全圖（或稱完全競賽圖、directed complete graph、complete tournament）$K_n^*$ 。例如下列兩圖都是 5 點的有向完全圖 $K_5^*$ 。
\item[（3）] 因為有 $\binom{n}{2}$ 邊，且每邊有兩種方向可以任給，故有 $2^{\binom{n}{2}}$ 種不同的 $K_n^*$ 。
【90 政大資科】【98 中山電機】
\item[（4）] $K_n^*$ 中，$\forall x \in V\left(K_n^*\right), \operatorname{deg}(x)=\operatorname{indeg}(x)+\operatorname{outdeg}(x)=n-1$ 。【90政大資科】
\end{itemize}