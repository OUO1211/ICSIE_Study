第四章 鏈結串列
141

Linked List

【註】不用抄寫剩下的項次指令，所以時間較省。

\section*{三．稀疏矩陣之表示}

稀疏矩陣的節點結構設計如下：
\begin{itemize}
\item[1．] 開頭節點（Head Node）

\begin{tabular}{|l|l|l|}
\hline Down & Head & Right \\
\hline \multicolumn{3}{|c|}{Next} \\
\hline
\end{tabular}
\item[2．] 元素節點（element Node）

\begin{tabular}{|l|l|l|l|l|}
\hline Down & Head & Row & Col & Right \\
\hline \multicolumn{5}{|c|}{Value} \\
\hline
\end{tabular}
\end{itemize}

每一節點將有一個 Head 欄，此欄被用來區別開頭節點與代表非零矩陣元素的節點。每一個開頭節點還有另外三欄：Down、Right 與 Next。開頭節點的總數等等於 $\operatorname{Max}\{$ 列數，行數 $\} 。$ 第 $i$ 列的開頭節點也是第 $i$ 行的開頭節點。開頭節點的 Down 欄是用來鏈結到行串列（Column List），而 Right 欄是用來鏈結至列串列（Row List）。Next 欄把開頭節點鏈結在一起。

元素節點則含有另外五欄：Row、Col、Down、Right 與 Value。Down 欄用來鏈結到同一行中的下一個非零項：而 Right 欄則用來鏈結到同一列中的下一個非零項。因此，如果 $\mathrm{a}_{\mathrm{ij}} \neq 0$ 那將會有一個節點，其 Head＝false，Value＝ $\mathrm{a}_{\mathrm{ij}}$ 、Row＝i、Col＝j，此節點同時鏈結到第 i 列與第 j 行的兩個環狀鏈結串列中；因此它必然同時屬於兩個不同的串列。

此外，開頭節點的串列本身含有一個相同於六個欄的元素節點之開頭節點，此節點的 Row 與 Col 欄是用來儲存矩陣的列數及行數。

例如：
$$
\left[\begin{array}{rrrrrrr}
0, & 0, & 11, & 0, & 0, & 13, & 0, \\
12, & 0, & 0, & 0, & 0, & 0, & 14, \\
0, & -1, & 0, & 0, & 0, & -8, & 0, \\
0, & 0, & 0, & 0, & 0, & 0, & 0, \\
0, & 0, & 0, & 0, & 0, & 0, & 0, \\
0, & -9, & 0, & 0, & 0, & 0, & 0,
\end{array}\right]
$$