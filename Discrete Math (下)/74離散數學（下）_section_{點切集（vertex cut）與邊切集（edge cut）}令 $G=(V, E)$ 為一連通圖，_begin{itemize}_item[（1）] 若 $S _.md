74
離散數學（下）

\section*{點切集（vertex cut）與邊切集（edge cut）}

令 $G=(V, E)$ 為一連通圖，
\begin{itemize}
\item[（1）] 若 $S \subseteq V(G)$ ，且 $G$ 去掉 $S$ 中的點後成為不連通，則稱 $S$ 為點切集。若 $S$ 中只有一點$v$ ，則稱 $v$ 為 $G$ 之一切點（cut vertex）。
\item[（2）] 若 $T \subseteq E(G)$ ，且 $G$ 去掉 $T$ 中的邊後成為不連通，則稱 $T$ 為邊切集。若 $T$ 中只有一邊$e$ ，則稱 $e$ 為 $G$ 之一切邊（cut edge）或橋（bridge）。
\item[（3）] 若 $T$ 為邊切集且 $T$ 的真子集都不是邊切集，則稱 $T$ 為 $G$ 中之一切集（cut set）。
\end{itemize}

例如右圖中，
$f, d$ 均為切點；$\{b, c, d\},\{b, c\}$ 均為點切集；
$(d, f)$ 為切邊；$\{(b, d),(e, d),(f, d)\},\{(g, h),(g, f),(f, h)\}$
均為邊切集。
$\{(b, d),(e, d)\},\{(g, h),(g, f)\}$ 均為切集。

Note
\begin{itemize}
\item[（1）] 若去掉 $v$ 點後，$G$ 的分量圖變多了，則稱 $v$ 為一 articulation point。此與切點的差別是，某些書上的切點只在連通圖時討論。
\item[（2）] 不是每個圖都有切點，例如 $K_n$ 就沒有切點，這種圖也被稱為 nonseparable graph 。
\item[（3）] 點連通度（vertex connectivity）$\lambda(G)$ ：最少取出幾點可使 $G$ 成為不連通。
\item[（4）] $0 \leq \lambda(G) \leq|V(G)|-1$ ，且 $\lambda(G)=0$ 只在 $G$ 為不連通或 $G$ 為單點；$\lambda(G)=n-1$ 只在 $G=K_n$ 。若 $\lambda(G) \geq k$ ，則稱 $G$ 為 $k$－連通（ $k$－vertex－connected）。若連通圖 $G$ 至少三點且沒切點，則$G$ 又稱為 2－connected 或 biconnected．
【109 台大工科】
\item[（5）] 邊連通度（edge connectivity）$\lambda^{\prime}(G)$ ：最少取出幾邊可使 $G$ 成為不連通。
\item[（6）] $\lambda^{\prime}(G)=0$ 只在 $G$ 為不連通或 $G$ 為單點；$\lambda^{\prime}(G)=n-1$ 只在 $G=K_n$ 。
\item[（7）] 對任何連通圖 $G, 0 \leq \lambda(G) \leq \lambda^{\prime}(G) \leq \min \operatorname{deg}$ of $(G)$ 。
\item[（8）] $G$ 中不含有切點之連通的極大誘導子圖（maximal induced subgraph），稱為 $G$ 之一區塊（block），或雙連通分量圖（bi－connected component）．
【94台大工工】
\end{itemize}