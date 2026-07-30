362
資料結構（含精選試題）
■

Data Structure
\begin{itemize}
\item[3．] 折疊相加（Folding Addition）
在此法中，識別字首先被分割成數段，其中除了最後一段之外，其餘各段均等長，然後將此各段相加而得到雜湊位址。在做各段相加時，有兩種方法。第一種方法是將各段完全切開，各段的最小位元與最後一段之最小位元對齊，然後各段之值相加起來。此法稱為位移折疊（Shift Folding）（如圖（a））。
另一為邊界折疊（Folding at Boundaries），各段之邊界並不切斷，而是以邊界為折疊支點，將各斷折疊後再將位相同位置之各位數相加起來（如圖（b））。

\begin{tabular}{|l|l|l|l|l|}
\hline P1 & P2 & P3 & P4 & P5 \\
\hline
\end{tabular}

\begin{table}
\begin{tabular}{|l|l|}
\hline P1 & 123 \\
\hline P2 & 203 \\
\hline P3 & 241 \\
\hline P4 & \multirow[t]{2}{*}{112} \\
\hline P5 & \\
\hline
\end{tabular}
\captionsetup{labelformat=empty}
\caption{（a）位移折疊}
\end{table}

\begin{tabular}{|l|l|l|l|l|}
\hline $\mathrm{P} 1=123$ & $\mathrm{P} 2=203$ & $\mathrm{P} 3=241$ & $\mathbf{P 4}=112$ & $\mathrm{P} 5=20$ \\
\hline
\end{tabular}

\begin{table}
\begin{tabular}{|l|l|}
\hline P1 & 123 \\
\hline P2 & 302 \\
\hline P3 & 241 \\
\hline P4 & \multirow[t]{2}{*}{211} \\
\hline P5 & \\
\hline
\end{tabular}
\captionsetup{labelformat=empty}
\caption{（b）邊界折疊}
\end{table}
\item[4．] 位數值分析（Digital Analysis）
此法適用於符號表中的識別字均已事先已知。此方法中，任一識別字 X 均被視為以一個 r 為基底（Radix）之數，然後可以來檢視各識別字之一位數。分析每一位數時，若該位數之值太集中就捨去該位，最後所剩下的位數只要能達到雜湊表之範圍即可。
例如：

\begin{tabular}{|l|l|l|l|l|l|l|l|l|l|l|l|}
\hline & 電 & 話 & & 碼 & & 鍵 & 值 & & 位 & 址 & \\
\hline 0 & 2 & － & 9 & 4 & 7 & 5 & 8 & 6 & 4 & 5 & 6 \\
\hline 0 & 2 & － & 9 & 8 & 7 & 8 & 6 & 4 & 8 & 8 & 4 \\
\hline 0 & 2 & － & 7 & 7 & 6 & 7 & 8 & 5 & 7 & 7 & 5 \\
\hline 0 & 2 & － & 8 & 2 & 1 & 6 & 4 & 3 & 2 & 6 & 3 \\
\hline 0 & 2 & － & 9 & 6 & 7 & 5 & 8 & 7 & 6 & 5 & 7 \\
\hline 0 & 2 & － & 8 & 3 & 7 & 4 & 8 & 2 & 3 & 4 & 2 \\
\hline 0 & 2 & － & 7 & 4 & 7 & 3 & 8 & 1 & 4 & 3 & 1 \\
\hline
\end{tabular}
\end{itemize}