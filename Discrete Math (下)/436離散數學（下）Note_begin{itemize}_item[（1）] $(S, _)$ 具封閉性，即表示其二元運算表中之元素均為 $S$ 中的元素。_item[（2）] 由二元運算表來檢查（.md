436
離散數學（下）

Note
\begin{itemize}
\item[（1）] $(S, *)$ 具封閉性，即表示其二元運算表中之元素均為 $S$ 中的元素。
\item[（2）] 由二元運算表來檢查（ $S, *$ ）是否具結合性：
設 $S=\{a, b, c\}$ ，其二元運算表為：

\begin{tabular}{|l|l|l|l|l|}
\hline ＊ & $a$ & $b$ & $c$ & \\
\hline $a$ & $x_1$ & $x_2$ & $x_3$ & $x_i \in\{a, b, c\}$ ，則再造出： \\
\hline $b$ & $x_4$ & $x_5$ & $x_6$ & \\
\hline $c$ & $x_7$ & $x_8$ & $x_9$ & \\
\hline
\end{tabular}

\begin{tabular}{|l|l|l|l|l|l|l|l|l|l|l|}
\hline ＊ & $x_1$ & $x_2$ & $x_3$ & $x_4$ & $x_5$ & $x_6$ & $x_7$ & $x_8$ & $x_9$ & \multirow{4}{*}{與} \\
\hline $a$ & $z_1$ & $z_2$ & $z_3$ & $z_4$ & $z_5$ & $z_6$ & $z_7$ & $z_8$ & $z_9$ & \\
\hline $b$ & $z_{10}$ & $z_{11}$ & $z_{12}$ & $z_{13}$ & $z_{14}$ & $z_{15}$ & $z_{16}$ & $z_{17}$ & $z_{18}$ & \\
\hline $c$ & $z_{19}$ & $z_{20}$ & $z_{21}$ & $z_{22}$ & $z_{23}$ & $z_{24}$ & $z_{25}$ & $z_{26}$ & $z_{27}$ & \\
\hline
\end{tabular}

\begin{tabular}{|l|l|l|l|}
\hline ＊ & $a$ & $b$ & $c$ \\
\hline $x_1$ & $y_1$ & $y_2$ & $y_3$ \\
\hline $x_2$ & $y_4$ & $y_5$ & $y_6$ \\
\hline $x_3$ & $y_7$ & $y_8$ & $y_9$ \\
\hline $x_4$ & $y_{10}$ & $y_{11}$ & $y_{12}, y_i, z_j \in\{a, b, c\}$ ， \\
\hline $x_5$ & $y_{13}$ & $y_{14}$ & $y_{15}$ \\
\hline $x_6$ & $y_{16}$ & $y_{17}$ & $y_{18}$ \\
\hline $x_7$ & $y_{19}$ & $y_{20}$ & $y_{21}$ \\
\hline $x_8$ & $y_{22}$ & $y_{23}$ & $y_{24}$ \\
\hline $x_9$ & $y_{25}$ & $y_{26}$ & $y_{27}$ \\
\hline
\end{tabular}
則 $(S, *)$ 具結合性 $\Leftrightarrow y_i=z_i \forall i$ 。
\item[（3）] $(S, *)$ 具單位元素，即表示其二元運算表中某列之元素與標題相同，某行的元素與標題相同。例如下表中的 $x$ ，即為一單位元素。

\begin{tabular}{|l|l|l|l|}
\hline ＊ & $a$ & $b$ & $x$ \\
\hline $a$ & $a$ & $a$ & $a$ \\
\hline $b$ & $a$ & $x$ & $b$ \\
\hline $x$ & a & $b$ & $x$ \\
\hline
\end{tabular}
\item[（4）] $(S, *)$ 具交換性，即表示其二元運算表中之元素對稱於主對角線。
\end{itemize}