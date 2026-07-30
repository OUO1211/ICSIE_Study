256
資料結構（含精選試題）
■■

Data Structure

\begin{tabular}{|l|l|l|l|}
\hline A ${ }^2$ & 1 & 2 & 3 \\
\hline 1 & 0 & 4 & 6 \\
\hline 2 & 6 & 0 & 2 \\
\hline 3 & 3 & 7 & 0 \\
\hline
\end{tabular}

\begin{tabular}{|l|l|l|l|}
\hline A ${ }^3$ & 1 & 2 & 3 \\
\hline 1 & 0 & 4 & 6 \\
\hline 2 & 5 & 0 & 2 \\
\hline 3 & 3 & 7 & 0 \\
\hline
\end{tabular}

\section*{三．遞移封閉性（Transitive Closure）}

決定 G 中的每個頂點對（i，j）是否存在從 i 到 j 的路徑。
以下定義兩個相關的矩陣：
\begin{itemize}
\item[（一）] 若 A 為 G 的相鄰矩陣，則矩陣 A ${ }^{+}$稱為 G 的遞移封閉矩陣（Transitive Closure Matrix），其特性是若從 i 到 j 有路徑可通且長度大於零，則 $\mathrm{A}^{+}(\mathrm{i}, \mathrm{j})=1$ ，否則為 0 。
\item[（二）] 矩陣 A＊稱為 G 的反身遞移封閉矩陣（Reflexive Transitive Closure Matrix），若從 i到 j 有路徑可通且長度 $\geq 0$ ，則 $\mathrm{A}^*(\mathrm{i}, \mathrm{j})=1$ ，否則為 0 。
\end{itemize}

下圖顯示了一個向圖 G 的 A，A ${ }^{+}$和 A＊。可以發現 A＋和 A＊的差異只有對角線項次不同。

（a）有向圖 G

（b）G相鄰矩陣A

（c） $\mathrm{A}^{+}$

（d）A＊

以下是計算遞移閉矩陣 $\mathrm{A}^{+}$的演算法：
Procedure TRAN＿CLOSURE（G）
$$
\begin{aligned}
& \text { for } \mathrm{i} \leftarrow 1 \text { to } \mathrm{n} \text { do } \\
& \text { for } \mathrm{j} \leftarrow \mathrm{i} \text { to } \mathrm{n} \text { do }
\end{aligned}
$$