240
離散數學（下）

\section*{生成樹個數－其他計算法－硬算}

例如：
How many nonisomorphic spanning trees are there for $K_{2,3}$ ？
【86 交大應數】
解 由題意知，此時點是不具編號的，故只剩下這兩個不同構的生成樹。

\section*{進階類題}
\begin{itemize}
\item[1．] $K_5$ 有多少不同構的 spanning tree？
解 如右圖3種，相當於問有多少種5點 unrooted tree。
\item[2．] How many spanning tree does $K_{2,9}$ have？
解 設 $V\left(K_{2,9}\right)=\left\{x_1, x_2, y_1, \cdots, y_9\right\}$ ，其中，$x_i$ 連到 $y_j, \forall i, \forall j$ ，
因為所形成的生成樹中，必有某個 $y_j$ 同時連到 $x_1, x_2$ ，
而且剩下的那些 $y_i$ ，for $i \neq j$ ，必恰連到 $x_1$ 或 $x_2$ ，
故形成的生成樹有 $\binom{9}{1} \cdot 2^8=9 \times 2^8$ 。
\end{itemize}