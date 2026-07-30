第四章 鏈結串列
131
Linked List
\begin{itemize}
\begin{itemize}
\item[] 【程式】 Procedure GetNode（x）
Begin
if AV＝nil then Call No More＿Node
else
$\mathrm{x}=\mathrm{AV} ;$
$\mathrm{AV}=\mathrm{AV} \uparrow$. Link；
End；
\end{itemize}
\item[（三）] Ret（x）
將一個節點 x 歸還給可用空間。
\begin{itemize}
\item[] 【程式】 Procedure Ret（x）
Begin
\item[（1）]
$$
\mathrm{x} \uparrow . \text { Link }=\mathrm{AV} ;
$$
\item[②]
$$
\mathrm{AV}=\mathrm{x} ;
$$
End；
\end{itemize}
\item[] 【圖示】
\end{itemize}

\section*{4－3 鏈結堆疊與鏈結佇列}
\begin{itemize}
\item[（一）] 使用 Link List 製作的優點有二：
\begin{itemize}
\item[1．] 方便插入／刪除元素。
\item[2．] Stack 與 Queue 的大小是可變動的。
\end{itemize}
\item[（二）] Linked Stack 與 Linked Queue 的圖示法
\end{itemize}