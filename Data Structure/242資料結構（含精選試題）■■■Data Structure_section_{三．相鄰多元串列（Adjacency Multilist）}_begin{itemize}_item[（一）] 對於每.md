242
資料結構（含精選試題）
■■■

Data Structure

\section*{三．相鄰多元串列（Adjacency Multilist）}
\begin{itemize}
\item[（一）] 對於每個邊而言，均以一個節點表示，節點結構如下：

\begin{tabular}{|l|l|l|l|l|}
\hline M & $\mathrm{V}_1$ & $\mathrm{V}_2$ & Link for $\mathrm{V}_1$ & Link for $\mathrm{V}_2$ \\
\hline
\end{tabular}
其中 M ：為一 Mark，表示該邊是否搜尋過。
$V_1 、 V_2$ ：是該邊的兩個節點。
Link for $\mathrm{V}_1$ ：若有其他頂點與頂點 $\mathrm{V}_1$ 相連，則 Link for $\mathrm{V}_1$ 指向＂該頂點與頂點$\mathrm{V}_1$ 所形成的邊節點＂，否則指向 nil。
Link for $\mathrm{V}_2$ ：若有其他頂點與頂點 $\mathrm{V}_2$ 相連，則 Link for $\mathrm{V}_2$ 指向＂該頂點與頂點$V_2$ 所形成的邊節點＂，否則指向 nil。
\item[（二）] 圖形中的每一個節點依序所產生一個 Head Array，這些 Head 分別指向第一個包含該頂點的邊之節點。
\item[（三）] 所需的記憶體空間，除了多個單元 M 外，和一般的相鄰串列所需的空間相同。例：
\end{itemize}

\section*{四．索引表格表示法}
\begin{itemize}
\item[（一）] 以一個一維陣列循序儲存相鄰的頂點，
\item[（二）] 建立一個索引陣列，n 個頂點須建立 n 個項目於 Index Array 中，分別對應於陣列中的第一個與該頂點相鄰的頂點之位置。例如，以 G1 為例：
\end{itemize}

\begin{tabular}{|l|l|}
\hline \multicolumn{2}{|c|}{Vertex Position} \\
\hline 1 & 1 \\
\hline 2 & 4 \\
\hline 3 & 7 \\
\hline 4 & 10 \\
\hline
\end{tabular}