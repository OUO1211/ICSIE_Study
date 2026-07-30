第九章 高等樹結構
429

Advanced Tree Structure

\begin{tabular}{|l|l|l|}
\hline Operations & Deap／Min－Max Heap & Leftist Heap \\
\hline Insert element & O（logN） & O（logN） \\
\hline Delete min／max element & O（logN） & $\mathrm{O}(\log \mathrm{N})$ \\
\hline Combine two queues & O（N） & $\mathrm{O}(\log \mathrm{N})$ \\
\hline
\end{tabular}
\begin{itemize}
\item[（二）] Shortest（X）定義
\begin{itemize}
\item[1．] Def：Shortest（X）為x到外部節點的最短路徑長度。
令 x 為 Extended Binary Tree 的 Node，令 leftchild（x）以及 rightchild（x）為x的左右子點。則
shortest $(\mathrm{X})=\left\{\begin{array}{l}0, \text { if } \mathrm{X} \text { is an external node } \\ 1+\min \{\text { shortest }(\text { leftchild }(\mathrm{x})), \text { shortest }(\text { rightchild }(\mathrm{x}))\}\end{array}\right.$
\item[2．] 例子：
\item[（三）] Leftist Tree
Def：若不為空，則對每一個內部節點 x，其 shortest（leftchild（x）$\geqq s h o r t e s t$ （rightchild（x））。
例如：上圖左邊不是，右邊才是 Leftist tree
\end{itemize}
\item[（四）] Min－Leftist Tree（or Max－Leftist Tree）
Def：為一 Leftist Tree，且其中每一個節點之鍵值小於（大於）等其子點的鍵值。例如 ：Min Leftist Tree
\end{itemize}