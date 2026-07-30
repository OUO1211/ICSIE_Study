142
資料結構（含精選試題）
Data Structure

【圖示】稀疏矩陣的鏈結表示方式下圖省略了 Head 欄標示。
$$
\begin{aligned}
\text { Head } & =\text { true 開頭節點 } \\
& =\text { false 非開頭節點 }
\end{aligned}
$$

\section*{4－7 鏈結串列之基本運算}
－．Length of link list
分為 Circular link list 及 single link list 兩種類型，底下為 circular list 長度。
【程式】 Procedure Length（A）
$$
\begin{aligned}
& \text { begin } \\
& \mathrm{i}=\phi ; \\
& \text { if } \mathrm{A} \neq \text { nil then Begin }
\end{aligned}
$$
$$
\begin{aligned}
& \text { ptr=A; } \\
& \text { repeat } \\
& \mathrm{i}=\mathrm{i}+1 ; \\
& \text { ptr }=\text { ptr } \uparrow . \text { Link; } \\
& \text { until ptr }=\mathrm{A} ;
\end{aligned}
$$