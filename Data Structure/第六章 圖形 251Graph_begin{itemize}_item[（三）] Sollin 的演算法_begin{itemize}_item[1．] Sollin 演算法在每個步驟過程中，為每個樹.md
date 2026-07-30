第六章 圖形 251
Graph
\begin{itemize}
\item[（三）] Sollin 的演算法
\begin{itemize}
\item[1．] Sollin 演算法在每個步驟過程中，為每個樹選擇一最小成本，由於對於樹林中的二個樹選擇同樣的邊是可能的。因此，重覆的相同邊將於每個 step 中剔除。而所選擇的邊，則加入展開樹中。此演算法在只有一個樹或者沒有剩下邊可供選擇的時候停止。
\item[2．] 例子
頂點 $1,2, \cdots, 7$ 所選擇的邊分別是：
（1，6），（2，7），（3，4），（4，3），（5，4），（6，1），$(9,2)$
\end{itemize}
\end{itemize}
此選擇中的不同邊，則為：
$(1,6),(2,7),(3,4)$ 和 $(5,4)$
把這些加入到所選擇邊的集合將形成下圖（a）的形狀。在下個步驟中，頂點集合為 $\{1,6\}$ 的樹選擇邊（6，5）而剩下的二個選擇邊（2，3）。把這二個邊加入到所選擇的邊之集合後，展開樹的建立的過程即完成。

（a）

（b）

\section*{6－5 圖形的最短路徑（Shortest Path of Graph）}
\begin{itemize}
\item[一．] 求 Single Source to All Destination 的最短路徑問題。
\item[（一）] 問題敘述
若存在一有向圖形 $\mathrm{G}=(\mathrm{V}, \mathrm{E})$ ，假設每一邊上皆附有其對應的加權數（Weight，W）或成本（Cost），欲求從某一頂點 $\mathrm{V}_0$ 到 G 中其他頂點的最短路徑的問題，稱之。
\end{itemize}