42
離散數學（下）

\section*{點覆蓋（Vertex cover）}

考虑無向圖 $G=(V, E)$ ，$S$ 為 $V$ 的一子集合，若 $G$ 中任一邊都有頂點在 $S$ 中，則稱 $S$ 為一點覆蓋。

例如，下圖中，$\{b, c, d, f, g\}$ 即為一vertex cover，且亦為 minimal。

Note
\begin{itemize}
\item[（1）] The vertex covering number $\beta(G): G$ 中具最少點的點覆蓋的點數。
\item[（2）] 若在一個 vertex cover 中再任拿掉一點，均會令其不為 vertex cover，則稱其為極小點覆蓋（minimal vertex cover）。
\item[（3）] $S$ 為 $G$ 中的獨立集 $\Leftrightarrow V-S$ 為 $G$ 的 vertex cover。【92暨南資工】【93中正資工】
【證明】
$S$ 為 $G$ 中的獨立集，
⇔ 任取邊 $e=(u, v), u, v$ 不會同時屬於 $S$（因為 $S$ 為獨立集），
$\Leftrightarrow u, v$ 必至少有一點屬於 $V-S$ ，即 $V-S$ 為 $G$ 的一組點覆蓋。
\item[（4）] $S$ 為 $G$ 中的 clique $\Leftrightarrow V-S$ 為 $\bar{G}$ 的 vertex cover
【證明】
$S$ 為 $G$ 的一 clique，
⇔ 任取邊 $e=(u, v) \in E(\bar{G})$ ，則 $u, v$ 不會同時屬於 $S$（因為 $S$ 為 clique），
⇔ 任取邊 $e=(u, v) \notin E(G)$ ，則 $u, v$ 不會同時屬於 $S$ ，
$\Leftrightarrow u, v$ 必至少有一點屬於 $V-S, \therefore V-S$ 為 $\bar{G}$ 的點覆蓋。
\item[（5）] $\alpha(G)+\beta(G)=|V(G)|$ 。
【證明】
設 $S$ 為 $G$ 中的一個最大獨立集，$|S|=\alpha$ ，$K$ 為 $G$ 中的一個最小點覆蓋，$|K|=\beta$ 。則因為 $V-S$ 為 $G$ 的一個點覆蓋，所以 $|V-S| \geq \beta$ ，即 $n-\alpha \geq \beta$ 。
又因為 $V-K$ 為 $G$ 的一個獨立集，所以 $|V-K| \leq \alpha$ ，即 $n-\beta \leq \alpha$ 。
$\therefore n \leq \alpha+\beta \leq n$ ，即 $n=\alpha+\beta$ 。
\end{itemize}