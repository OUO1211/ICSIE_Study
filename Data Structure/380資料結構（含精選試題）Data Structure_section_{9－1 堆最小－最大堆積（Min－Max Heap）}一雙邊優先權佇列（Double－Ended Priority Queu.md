380
資料結構（含精選試題）
Data Structure

\section*{9－1 堆最小－最大堆積（Min－Max Heap）}

一雙邊優先權佇列（Double－Ended Priority Queue）資料結構，能提供下列運算：
\begin{itemize}
\item[（一）] 插入任意鍵的元素。
\item[（二）] 刪除最大鍵的元素。
\item[（三）] 刪除最小鍵的元素。
\end{itemize}

Min－Max Heap 為製作雙邊優先權佇列的資結。
定義：最小－最大堆是一完整二元樹，若不為空，則此樹的交互階層（Alternating Levels）分別是最小階層和最大階層。樹根位於最小階層。假設 x 是最小－最大堆積的任一節點，如果 x 位於最小（最大）階層，那麼 x 在以 x 為根部的所有子樹元素中有最小（最大）鍵。位於最小（最大）階層上的節點，稱為最小（最大）節點（MinMode，Max Mode）。
\begin{itemize}
\item[] －例子：
\item[] Insert operation
例：假設我們想插入鍵為 5 的元素，先置於 last Node 中
\end{itemize}