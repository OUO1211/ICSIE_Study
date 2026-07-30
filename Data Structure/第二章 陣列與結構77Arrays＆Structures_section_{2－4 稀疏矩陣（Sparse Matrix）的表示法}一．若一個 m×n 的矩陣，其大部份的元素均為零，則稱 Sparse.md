第二章 陣列與結構
77

Arrays＆Structures

\section*{2－4 稀疏矩陣（Sparse Matrix）的表示法}

一．若一個 m×n 的矩陣，其大部份的元素均為零，則稱 Sparse Matrix。
二．為避免空間上的浪費，其解決方法是採用3－Tuple 結構來儲存每個非零項次【作法】每一個非零項是（i，j，Value），其中：
$\left\{\begin{array}{l}\mathrm{i}: \text { 列數，} \mathrm{j}: \text { 行數 } \\ \text { Value：儲存元素值 }\end{array}\right.$
假設有 t 個非零項，則需一個二維陣列 $\mathrm{A}(0 \cdots \mathrm{t}, 1 \cdots 3)$ 來儲存，其中$\mathrm{A}(0,1)$ ：存陣列的總列數。
$A(0,2)$ ：存陣列的總行數。
$\mathrm{A}(0,3)$ ：存非零項次的數目 t。
例題 2－13

\begin{tabular}{|l|l|l|l|l|l|l|}
\hline & 1 & 2 & 3 & 4 & 5 & 6 \\
\hline 1 & 15 & 0 & 0 & 22 & 0 & －15 \\
\hline 2 & 0 & 11 & 3 & 0 & 0 & 0 \\
\hline 3 & 0 & 0 & 0 & －6 & 0 & 0 \\
\hline 4 & 0 & 0 & 0 & 0 & 0 & 0 \\
\hline 5 & 91 & 0 & 0 & 0 & 0 & 0 \\
\hline 6 & 0 & 0 & 28 & 0 & 0 & 0 \\
\hline
\end{tabular}

\begin{tabular}{|l|l|l|l|l|l|}
\hline \multirow[b]{2}{*}{→} & \multirow{10}{*}{A} & & 1 & 2 & 3 \\
\hline & & 0 & 6 & 6 & 8 \\
\hline & & 1 & 1 & 1 & 15 \\
\hline & & 2 & 1 & 4 & 22 \\
\hline & & 3 & 1 & 6 & －15 \\
\hline & & 4 & 2 & 2 & 11 \\
\hline & & 5 & 2 & 3 & 3 \\
\hline & & 6 & 3 & 4 & －6 \\
\hline & & 7 & 5 & 1 & 91 \\
\hline & & 8 & 6 & 3 & 28 \\
\hline
\end{tabular}