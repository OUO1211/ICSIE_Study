176 資料結構（含精選試題）
Data Structure

例：

\begin{tabular}{|l|l|l|}
\hline Level 1 & 1 & A \\
\hline \multirow[t]{2}{*}{Level 2} & 2 & B \\
\hline & 3 & C \\
\hline \multirow[t]{4}{*}{Level 3} & 4 & \\
\hline & 5 & E \\
\hline & 6 & \\
\hline & 7 & \\
\hline \multirow[t]{6}{*}{Level 4} & 8 & \\
\hline & 9 & \\
\hline & 10 & F \\
\hline & 11 & \\
\hline & ： & \\
\hline & ： & \\
\hline
\end{tabular}

優點：處理簡單，對於 Full Bynary Tree 而言，此方式相當節省空間（無空間上的浪費）。
缺點：1．若遇到 Skewed Binary Tree，則很浪費空間。說明：深度為 k 的斜曲二元樹需要 $2^k-1$ 個空間，但真正使用空間只有k 個，故浪費 $2^{\mathrm{k}}-1-\mathrm{k}$ 個。
\begin{itemize}
\item[2．] 在樹中插入或刪除一個節點，都需要大量搬動資料以反映改變之後的樹結構。
\end{itemize}

\section*{二．鏈結串列（Linked List）表示法}

作法：節點結構如下

\begin{tabular}{|l|l|l|}
\hline Lchild & DATA & Rchild \\
\hline
\end{tabular}

其中 DATA：存放節點資料值。
Lchild：指向其左子樹的指標。
Rchild：指向其右子樹的指標。