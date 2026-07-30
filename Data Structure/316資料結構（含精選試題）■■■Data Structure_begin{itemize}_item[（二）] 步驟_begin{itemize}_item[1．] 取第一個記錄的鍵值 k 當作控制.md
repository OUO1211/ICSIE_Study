316
資料結構（含精選試題）
■■■
Data Structure
\begin{itemize}
\item[（二）] 步驟
\begin{itemize}
\item[1．] 取第一個記錄的鍵值 k 當作控制鍵（Pivot key）。
\item[2．] 先由左向右找到第 1 個 $k_i \geq k, \quad i=1,2,3, \cdots, n$且由右向左找到第 1 個 $k_j \leq k, j=n, n-1, \cdots, 1$
\item[3．] 若 $\mathrm{i}<\mathrm{j}$ ，則將 $\mathrm{R}_{\mathrm{i}}$ 與 $\mathrm{R}_{\mathrm{j}}$ 的位置對調，並回到步驟二，否則 $\mathrm{R}_{\mathrm{k}}$ 與 $\mathrm{R}_{\mathrm{j}}$ 位置對調，將此檔案一分為二，即
$\left(\mathrm{R}_1, \mathrm{R}_2, \cdots, \mathrm{R}_{\mathrm{j}-1}\right) \mathrm{R}_{\mathrm{j}}\left(\mathrm{R}_{\mathrm{j}+1}, \mathrm{R}_{\mathrm{j}+2}, \cdots, \mathrm{R}_{\mathrm{n}}\right)$
而這兩部份可獨立進行快速排序，完成排序。
\item[] 例：設有一輸入檔案有 10 個記錄，其鍵值順序為：
26，5，37，1，61，11，59，15，48， 19
下表所示即為每次呼叫 Qsort 時檔案內容之狀態。以中括號所括住之部份檔案表示尚待排序者。

\begin{tabular}{|l|l|l|l|l|l|l|l|l|l|l|l|}
\hline $\mathrm{R}_1$ & $\mathrm{R}_2$ & $\mathrm{R}_3$ & $\mathrm{R}_4$ & $\mathrm{R}_5$ & $\mathrm{R}_6$ & $\mathrm{R}_7$ & $\mathrm{R}_8$ & $\mathrm{R}_9$ & $\mathrm{R}_{10}$ & m & n \\
\hline ［26 & 5 & 37 & 1 & 61 & 11 & 59 & 15 & 48 & 19］ & 1 & 10］ \\
\hline ［11 & 5 & 19 & 1 & 15］ & 26 & 59］ & 61 & 48 & 37］ & 1 & 5 \\
\hline ［ 1 & 5］ & 11 & ［19 & 15］ & 26 & ［59 & 61 & 48 & 37］ & 1 & 2 \\
\hline 1 & 5 & 11 & ［19 & 15］ & 26 & ［59 & 61 & 48 & 37］ & 4 & 5 \\
\hline 1 & 5 & 11 & 15 & 19 & 26 & ［59 & 61 & 48 & 37］ & 7 & 10 \\
\hline 1 & 5 & 11 & 15 & 19 & 26 & ［48 & 37］ & 59 & ［61］ & 7 & 8 \\
\hline 1 & 5 & 11 & 15 & 19 & 26 & 37 & 48 & 59 & ［61］ & 10 & 10 \\
\hline 1 & 5 & 11 & 15 & 19 & 26 & 37 & 48 & 59 & 61 & & \\
\hline
\end{tabular}
\item[4．] 快速排序之 algorithm
Procedure Qsort（Var list ：afile；m，n ：integer）；
｛Sort records list［m］，⋯，list［n］into nondecresing order on field key．
key $\mathrm{k}=$ list［m］．key is arbitrarily chosen as the control key．Pointers i and j are used to partition the subfile so that at any time list［1］．key $\leq \mathrm{k}, \mathrm{l}<\mathrm{i}$ and list［1］．key $\geq \mathrm{k}, 1>\mathrm{j}$ ．
It is assumed that list［m］．key $\leq$ list $[\mathrm{n}+1]$ ．key $\}$
\end{itemize}
\end{itemize}

\footnotetext{
Var i，j，k ：Integer；
Begin
If $\mathrm{m}<\mathrm{n}$ Then Begin
}