408
資料結構（含精選試題）
■■■

Data Structure

（xii）SEPTEMBER
（六）Time Complexity for Array，linked list 及 AVL Tree

\begin{tabular}{|l|l|l|l|}
\hline Operation & Array & Linked List & AVL－Tree \\
\hline Search for X & $0(\log \mathrm{n})$ & 0（n） & $0(\log \mathrm{n})$ \\
\hline Search for k＇th item & 0（1） & 0（k） & $0(\log \mathrm{n})$ \\
\hline Delete X & 0（n） & 0（1） & $0(\log \mathrm{n})$ \\
\hline Delete k＇th item & $0(\mathrm{n}-\mathrm{k})$ & 0（k） & $0(\log \mathrm{n})$ \\
\hline Insert X & 0（n） & 0（1） & $0(\log \mathrm{n})$ \\
\hline Output in order & 0（n） & 0（n） & 0（n） \\
\hline
\end{tabular}

9－7 2－3 樹
\begin{itemize}
\item[（一）] 為一特殊情況的 B Tree ：B－tree of order 3
\item[（二）] 因每個 2－3 樹的內部節點的 Degree 為 2 或 3 而來。Degree 為 2 的節點稱為2－節點，而 Degree 為 3 的節點稱為3－節點。
\item[（三）] 定義：2－3 樹為一空樹或滿足下列特性的搜尋樹：
\begin{itemize}
\item[1．] 每個內部點為：2－節點或3－節點。其中2－節點有一個元素，3－節點有 2 個元素。
\item[2．] 假設 LeftChild 和 MiddleChild 代表 2－節點的兒子，又設 dataL 為此節點的元素，且 dataL．key 為它的鍵。所有 LeftChild 為根部的2－3 子樹的元素其鍵必小於dataL．key，而以 MiddleChild 為根部的2－3子樹的元素其鍵必大於 data．key。
\item[3．] 假設 LeffChild • MiddIChild 和 RightChild 代表 3－節點的兒子又設 dataL 和 dataR
\end{itemize}
\end{itemize}