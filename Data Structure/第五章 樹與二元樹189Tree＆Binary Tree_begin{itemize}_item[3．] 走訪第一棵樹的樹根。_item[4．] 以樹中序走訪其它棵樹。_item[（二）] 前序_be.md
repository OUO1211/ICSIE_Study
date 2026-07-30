第五章 樹與二元樹
189
Tree＆Binary Tree
\begin{itemize}
\item[3．] 走訪第一棵樹的樹根。
\item[4．] 以樹中序走訪其它棵樹。
\item[（二）] 前序
\begin{itemize}
\item[1．] 如果 F 為空的，那就直接返回。
\item[2．] 走訪 F 第一棵樹的樹根。
\item[3．] 依樹前序走訪第一棵的子樹。
\item[4．] 依樹前序走訪 F 的其他棵樹。
\end{itemize}
\item[（三）] 後序
\begin{itemize}
\item[1．] 如果 F 為空的，那就直接返回。
\item[2．] 以樹後序走訪第一棵的子樹。
\item[3．] 以樹後序的走訪 F 的其他棵樹。
\item[4．] 走訪 F 第一棵樹的樹根。
\item[] 例：
\end{itemize}
\end{itemize}

中序：EBCDAGHFI
前序：ABECDFGHI
後序：EBCDGHIFA
【註】亦可化為二元樹再追蹤，但後序無自然對應，即森林的中序、前序與化成二元樹後的中序、前序相同。

例：化成 Binary Tree 後如下所示：

中序：EBCDAGHFI
前序：ABECDFGHI
後序：EDCBHGIFA