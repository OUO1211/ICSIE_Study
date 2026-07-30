第五章 樹與二元樹
187
Tree＆Binary Tree

\section*{5－8 一般樹的二元樹表示法（Using Link List）}
\begin{itemize}
\item[（一）] 將節點的大小固定為 k 個兒子欄，其中 k 為 tree degree。

\begin{tabular}{|l|l|l|l|}
\hline \multicolumn{4}{|c|}{DATA} \\
\hline Child 1 & Child 2 & ⋯ & Child k \\
\hline
\end{tabular}
\item[（二）] 極浪費 Link 空間 ：如果 t 為一 k 元樹，節點個數為 n，而則 nk 個鏈結欄中將有$n(k-1)+1$ 個為 nil，且 $n \geq 1$ 。
證明：因為在 n 個節點中非 nil 之鏈結數等於 n－1，而在 n 節點的 k 的元樹中，其鏈結數共為 nk，因此鏈結等於 nil 之個數 nk－$(n-1)=n(k-1)+1$ 。
hence，為了節省空間，通常將樹化為二元樹來表示。
\item[（三）] 將一般樹化為二元樹的方法
步骤：一般是採用＂Leftmost－Child－Next－Right－Sibling＂的方式。
\begin{itemize}
\item[1．] 將節點的所有兄弟（Sibling）用平行線連接起來。
\item[2．] 刪除掉父點與所有子節點間的鏈結，只保留與最左子點間的鏈結。
\item[3．] 順時針轉 45°
\end{itemize}
例：
\end{itemize}