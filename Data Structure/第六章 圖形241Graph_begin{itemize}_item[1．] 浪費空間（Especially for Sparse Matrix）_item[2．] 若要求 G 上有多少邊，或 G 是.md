第六章 圖形
241

Graph
\begin{itemize}
\item[1．] 浪費空間（Especially for Sparse Matrix）
\item[2．] 若要求 G 上有多少邊，或 G 是否為連通等等；使用相鄰矩陣表示方式，則無論使用何種演算法，在最壞的情況時，所需的時間為 $O\left(n^2\right), n$ 為頂點個數。
\end{itemize}

\section*{二．相数串列（Adjacency List）}
\begin{itemize}
\item[（一）] G 中的每一個頂點都有頂點 i 個相鄰串列開頭節點陣列表示，串列 i 上的每一個節點表示一個相鄰的頂點。每個節點至少有兩欄：Vertex 和 Link。Vertex 欄存放與頂點i相鄰之頂點。
\item[（二）] 例子
\item[1．] $\mathrm{G}_1$ 之相鄰串列
\item[2．] $\mathrm{G}_2$ 之相鄰串列
\item[（三）] 對於有 n 個頂點以及 e 個邊的無向圖形，這種表示需要 n 個 Head 節點及 2e 個節點。
\item[（四）] 在無向圖形中，任一個頂點的分支度，就是其相鄰串列上的節點數目；因此圖形$G$ 中邊的個數，可以在 $0(n+e)$ 時間求得。
\item[（五）] 對有向圖形而言，串列節點的數目只有 e 個，任一個頂點的出支可以從其相数串列的節點數得到；因此，$G$ 上的邊數，可以在 $0(n+e)$ 時間內求出。若是求一個頂點的入支度就比較複雜一點。因為需要重複地找尋和某個頂點相鄰的所有頂點時，此時可再記錄另一組的串列，稱為反鄰串列（Inverse Adjacency List）。每個頂點有一個反鄰串列，串列上的每一個節點代表一個相鄰至該頂點的頂點（如下圖所示），以利求出 indegree of a vartex。

\begin{tabular}{|l|l|l|}
\hline Vertex 1 & & nil \\
\hline Vertex 2 & & nil \\
\hline Vertex 3 & & nil \\
\hline
\end{tabular}
\end{itemize}