第九章 高等樹結構
431

Advanced Tree Structure

⇒ 轉換成最小左傾樹
由（8）→（5）→（2）（root），check shortest（Leftchild）$\geqq$ shortest（Rightchild）
因為 union 為沿著兩個要 combine 之左傾樹最右邊路徑向下移動，∴ 合併全部元素個數為 n 的兩個左傾樹 time complexity 為 O（logn）

\section*{三．Skew Heap}
\begin{itemize}
\item[（一）] 為一具有 Heap 性質的 Binary Tree，但是不像 Leftist Heap 有結構上的限制
\item[（二）] 其右邊的路徑可以任意長
\item[（三）] Skew Heap 與 Leftist Heap 之關係有點類似於 Splay tree 與 AVL Tree 之關係
\item[（四）] Skew Heap 之 Merge 動作
\item[1．] Def：與前述 Leftist Heap 相同。只有一個地方不同，其左、右子點的交換是無條件的，除了在右邊路徑上的最大的節點之外，對於其它的 Node 一定作交換。
\end{itemize}