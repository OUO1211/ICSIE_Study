第九章 高等樹結構
425
Advanced Tree Structure
\begin{itemize}
\item[（1）] 刪除 $X=58$ 之結果
\item[（2）] 刪除 $X=65$ 之結果
\end{itemize}

\section*{9－12 補充}
\begin{itemize}
\item[] －．Splay Tree
\item[（一）] 緣由：AVL Tree，2－3 tree，2－3－4 tree and Red－Black Tree 可以在 $\mathrm{O}(\log N)$ 的時間內完成 Insert，Delete and Delete 的運算。但若以分攤成本的角度來看，我們可以利用一個簡單的 splay operations，使得 search tree 的所有運算成本可以在 $O(\log N)$ 的分攤時間成本內完成。
\item[（二）] 定義 ：Splay Tree is a Binary Search Tree，其 Insert，Delete，and Search 運算皆與Binary search Tree 相同。但是每一個運算之後，會接著一個 Splay 運算。Splay 運算由一連串的旋轉所組成。
\item[（三）] Splay 運算的起始節點：
\begin{itemize}
\item[1．] Search ：由包含所搜尋的元素之節點作為 Splay 運算起點
\item[2．] Insert ：由新插入的節點作為 Splay 運算起點
\item[3．] Delete：由被刪除節點的父親節點作為 Splay 運算起點。如果刪除節點為 Root，則以 NULL 作為 Splay 運算起點。
\end{itemize}
\end{itemize}