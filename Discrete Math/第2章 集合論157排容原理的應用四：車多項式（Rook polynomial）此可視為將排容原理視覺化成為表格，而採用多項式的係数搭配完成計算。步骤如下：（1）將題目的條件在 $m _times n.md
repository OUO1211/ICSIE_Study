第2章 集合論
157

排容原理的應用四：車多項式（Rook polynomial）
此可視為將排容原理視覺化成為表格，而採用多項式的係数搭配完成計算。步骤如下：
（1）將題目的條件在 $m \times n$ 表格內打叉。
（2）盡量把表格列交換行交換成可＂完整分隔的数個子表格＂
（3）列出各互斥子表格的車多項式 $1+a_1 x+a_2 x^2+\ldots$ ，
其中，$a_i$ 代表在那些打叉的位置放車，共放 $i$ 個，使不在同列同行出現的方法数。
（4）答案為 $\frac{n!}{(n-m)!}-a_1 \cdot \frac{(n-1)!}{(n-m)!}+a_2 \cdot \frac{(n-2)!}{(n-m)!}-\ldots$ 。
（5）另外，如題目無法拆成互斥的子表格，則可能造成求算各係数時的運算量太大，此時也可参考使用車多項式的遞迴：
方法－挑選一處可使去掉此位置的叉後，剩狳是互斥的子表格（如下表的（ $i_1, 3$ ）），接著去掉此處的叉形成表格 2 ；也去掉這叉所在列與行的所有叉成表格 3 ，則表格 1 的車多項式 $=$ 表格 2 的車多項式 + 表格 3 的車多項式乘上 $x$ 。

\begin{table}
\captionsetup{labelformat=empty}
\caption{表格1}
\begin{tabular}{|c|c|c|c|c|c|c|}
\hline & 4 & 2 & 3 & 1 & 5 & 6 \\
\hline$i_4$ & $\times$ & & & & & \\
\hline$i_3$ & & $\times$ & $\times$ & & & \\
\hline$i_1$ & & & {$[\times]$} & $\times$ & $\times$ & \\
\hline$i_6$ & & & & & $\times$ & $\times$ \\
\hline$i_2$ & & & & & & \\
\hline$i_5$ & & & & & & \\
\hline
\end{tabular}
\end{table}

\begin{table}
\captionsetup{labelformat=empty}
\caption{表格2}
\begin{tabular}{|c|c|c|c|c|c|c|}
\hline & 4 & 2 & 3 & 1 & 5 & 6 \\
\hline$i_4$ & $\times$ & & & & & \\
\hline$i_3$ & & $\times$ & $\times$ & & & \\
\hline$i_1$ & & & & $\times$ & $\times$ & \\
\hline$i_6$ & & & & & $\times$ & $\times$ \\
\hline$i_2$ & & & & & & \\
\hline$i_5$ & & & & & & \\
\hline
\end{tabular}
\end{table}

\begin{table}
\captionsetup{labelformat=empty}
\caption{表格3}
\begin{tabular}{|l|l|l|l|l|l|l|}
\hline & 4 & 2 & 3 & 1 & 5 & 6 \\
\hline$i_4$ & $\times$ & & & & & \\
\hline$i_3$ & & $\times$ & & & & \\
\hline$i_1$ & & & & & & \\
\hline$i_6$ & & & & & $\times$ & $\times$ \\
\hline$i_2$ & & & & & & \\
\hline$i_5$ & & & & & & \\
\hline
\end{tabular}
\end{table}