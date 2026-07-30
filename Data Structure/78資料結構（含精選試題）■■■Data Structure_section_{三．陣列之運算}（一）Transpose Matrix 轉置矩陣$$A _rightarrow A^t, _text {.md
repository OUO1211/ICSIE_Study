78
資料結構（含精選試題）
■■■
Data Structure

\section*{三．陣列之運算}
（一）Transpose Matrix 轉置矩陣
$$
A \rightarrow A^t, \text { 即 } a_{i j} \rightarrow a_{j i}
$$

【演算法一】
for each row i do
$$
\begin{aligned}
& \text { take element(i, j, Value) from A } \\
& \text { and store it in (j, I, Value) of the At }
\end{aligned}
$$
end；
此法行不通，因為如 $(1,6,-15) \rightarrow(6,1,-15)$ 還未掃完整個陣列，不曉得 $(6,1,-15)$的位址在何處！所以，改用以行（Column）的順序來考慮。

【演算法二】
for all elements in column j do
place element(i, j, Value) and store it in
position(j, i, Value)
end；
上述演算法之 Complexity 分析
第15－21列上迴圈每執行一次，第17列就要執行 t 次。
而 $15-21$ 列要重複 $n$ 次，因此第 17 列執行 nt次。
第10—14列執行 time 為常數 → O（nt）。
當 t 的級數為 nm 時 $\rightarrow \mathrm{O}\left(\mathrm{n}^2 \mathrm{~m}\right)$ ，會比二維陣列的 $\mathrm{O}(\mathrm{nm})$ 差可用 Fast Transpose
【演算法三】Fast Transpose
\begin{itemize}
\item[] －Time Complexity →O（n＋t）
\end{itemize}
$\because 4$ 個迴圈分別作 $\mathrm{n} 、 \mathrm{t} 、 \mathrm{n}-1$ 及 t 次
當 $\mathrm{t}=\mathrm{mn}$ 時 →O（mn）與一維陣列相同。
Void fast＿transpose（term a［ ］，term b［ ］）
$$
\{
$$
／＊the transpose of a is placed in b ＊／
int row_terms [MAX_Col], starting_pos [MAX_COL];
$$
\text { int } \mathrm{i}, \mathrm{j} \text {, num_cols }=\mathrm{a}[0] . \mathrm{col}, \text { num _terms }=\mathrm{a}[0] . \text { value } ;
$$
$$
\mathrm{b}[0] . \text { row }=\text { num_cols; } \mathrm{b}[0] . \mathrm{col}=\mathrm{a}[0] . \text { row; }
$$
$$
\mathrm{b}[0] \text {.value }=\text { num_terms } ;
$$
$$
\text { if (num_terms }>0 \text { ) \{/* nonzero matrix } * /
$$