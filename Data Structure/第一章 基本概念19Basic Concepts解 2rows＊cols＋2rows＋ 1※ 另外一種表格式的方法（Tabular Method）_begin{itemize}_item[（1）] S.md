第一章 基本概念
19
Basic Concepts

解 2rows＊cols＋2rows＋ 1
※ 另外一種表格式的方法（Tabular Method）
\begin{itemize}
\item[（1）] Steps／Execution（S／E）
Step count for each statement．
\item[（2）] Frequency
The number of times that each statement is executed．
Total steps $=(1) *(2) \quad$（For each step）
\end{itemize}

例題 1－18
Permutations

\begin{tabular}{|l|l|l|l|}
\hline Statement & S／E & Frequency & Total steps \\
\hline Float sum（float list［ ］，int n） & 0 & 0 & 0 \\
\hline ｛ & 0 & 0 & 0 \\
\hline float tempsum＝0； & 1 & 1 & 1 \\
\hline int i； & 0 & 0 & 0 \\
\hline for $(\mathrm{i}=0 ; \mathrm{i}<\mathrm{n} ; \mathrm{i}++)$ & 1 & $\mathrm{n}+1$ & $\mathrm{n}+1$ \\
\hline tempsum＋＝list［i］ & 1 & n & n \\
\hline return tempsum； & 1 & 1 & 1 \\
\hline \} & 0 & 0 & 0 \\
\hline Total & \multicolumn{3}{|r|}{$2 \mathrm{n}+3$} \\
\hline
\end{tabular}

\begin{tabular}{|l|l|l|l|}
\hline Statement & S／E & Frequency & Total steps \\
\hline Float sum（float list［ ］，int n） & 0 & 0 & 0 \\
\hline ｛ & 0 & 0 & 0 \\
\hline if（n） & 1 & $\mathrm{n}+1$ & $\mathrm{n}+1$ \\
\hline return rsum（list，n－1）＋list［n－1］； & 1 & n & n \\
\hline return list［0］； & 1 & 1 & 1 \\
\hline \} & 0 & 0 & 0 \\
\hline Total & \multicolumn{3}{|r|}{$2 \mathrm{n}+2$} \\
\hline
\end{tabular}