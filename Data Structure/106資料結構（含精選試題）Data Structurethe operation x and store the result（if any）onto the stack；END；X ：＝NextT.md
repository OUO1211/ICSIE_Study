106
資料結構（含精選試題）
Data Structure

the operation x and store the result（if any）onto the stack；
END；
X ：＝NextToken（e）；
END；｛ of while\}
END；｛of eval\}
例題 3－3
43－15＊＋

例題 3－4
$\mathrm{AB} / \mathrm{C}-\mathrm{DE}^*+\mathrm{AC}^*-$

\begin{tabular}{|l|l|}
\hline Operation & postfix \\
\hline T1：＝A／B & T1－DE＊＋AC＊－ \\
\hline $\mathrm{T} 2:=\mathrm{T} 1-1$ & T2DE＊＋AC＊－ \\
\hline T3：＝D＊E & T2T＿3＋AC＊－ \\
\hline T4：＝T2＋T3 & T4AC＊－ \\
\hline T5：＝A＊C & T4T5－ \\
\hline T6：＝T4－T5 & T6 \\
\hline POP→T6 結果。 & \\
\hline
\end{tabular}

四．多重堆叠（multiple stacks）
假設將多重堆疊以循序對應（sequential mapping）的方式表示在單一維的陣列 U（1．．m）中
\begin{itemize}
\item[（一）] Two stacks Solution
利用 U［1］當作堆疊 1 的最底端（bottommost）元素，而以 U［m］表示另一個堆疊的最底端元素；然後堆疊 1 向 $[\mathrm{U}] \mathrm{m}$ 的方向成長，而堆疊 2 則向 $\mathrm{U}[1]$ 的方向成長。因此譡樣的表示方式能夠很有效地利用整個全部的空間。
\end{itemize}