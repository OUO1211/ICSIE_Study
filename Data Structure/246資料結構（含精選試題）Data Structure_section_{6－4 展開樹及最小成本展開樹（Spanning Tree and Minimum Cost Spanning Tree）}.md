246
資料結構（含精選試題）
Data Structure

\section*{6－4 展開樹及最小成本展開樹（Spanning Tree and Minimum Cost Spanning Tree）}

一．展開樹（Spanning Tree）
【定義】
當圖形 G 是連通時，以任何一個頂點為起始點所做的縱向優先搜尋或橫向優先搜尋時，都會走過 G 中的所有頂點。在這種情況下，G 中的所有邊可分成為二個集合T（樹邊）及 B（稱邊）；其中 T 是搜尋時所經過的所有邊所成的集合，而 B 是其他的邊所成的集合。T 中的所有邊構成了一個包含 G 中所有頂點的樹。任何一個只由 G 的邊所構成，且包含 G 中所有頂點的樹，稱為一個展開樹。呼叫 DFS 而得到的展開樹稱為縱向優先開樹；使用 BFS 而得到的展開樹稱為橫向優先展開樹。
特質：
若 $\mathrm{G}=(\mathrm{V}, \mathrm{E})$ 為一圖形時， $\mathrm{S}=(\mathrm{V}, \mathrm{T})$ 為 G 中的一個 Spanning Tree，則具有以下三項性質：
\begin{itemize}
\item[（一）] $\mathrm{E}=\mathrm{T}+\mathrm{B}$
\item[（二）] 若加入 B 中的任何一個邊到 S 中，會產生 Cycle。
\item[（三）] 任何兩頂點 $V_i, V_j$ 在 $S$ 中，存在唯一的一條 Simple Path。
例 ： $\mathrm{G}=$
\end{itemize}