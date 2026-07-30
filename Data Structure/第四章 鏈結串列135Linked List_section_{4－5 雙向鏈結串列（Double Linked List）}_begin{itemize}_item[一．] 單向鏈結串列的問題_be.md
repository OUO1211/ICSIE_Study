第四章 鏈結串列
135
Linked List

\section*{4－5 雙向鏈結串列（Double Linked List）}
\begin{itemize}
\item[一．] 單向鏈結串列的問題
\begin{itemize}
\item[（一）] 我們只能單方向的來找尋串列中的 Node，若要刪除一個節點時，必須事先知道前一個節點的位置。
\item[（二）] 若其中一個鏈結指標脫落時，則此 Linked List 將一分為二，無法再恢復原狀，可靠度差。
\end{itemize}
\item[二．] 雙向鏈結串列的資料結構
\begin{itemize}
\item[（一）] 每個 Node 表示如下：

\begin{tabular}{|l|l|l|}
\hline LLINK & DATA & RLINK \\
\hline
\end{tabular}
LLINK：指向前一個節點
RLINK：指向下一個節點
\item[（二）] 通常在雙向 Linked List 中，加上一個串列首，使用起來更加方便。串列首的資料欄不存任何資料。圖示如下：
\item[（三）] 特性
\begin{itemize}
\item[1．] 假設 P 是指向串列任何一個節點的指標，則 P 可以等於
$$
(\mathrm{P} \uparrow . \mathrm{L} \text { Link }) \uparrow . \mathrm{R} \text { Link }=(\mathrm{P} \uparrow . \mathrm{R} \text { Link }) \uparrow . \mathrm{L} \text { Link }
$$
\end{itemize}
\item[（四）] Double Linked List 的加入／刪除動作
\begin{itemize}
\item[1．] 加入動作：需要改變四個指標。
\end{itemize}
\end{itemize}
\end{itemize}