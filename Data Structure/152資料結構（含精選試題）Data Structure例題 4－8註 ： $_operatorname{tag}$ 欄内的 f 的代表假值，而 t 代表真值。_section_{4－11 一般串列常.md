152
資料結構（含精選試題）
Data Structure

例題 4－8

註 ： $\operatorname{tag}$ 欄内的 f 的代表假值，而 t 代表真值。

\section*{4－11 一般串列常見的遞迴式運算}

假設 node 的定義如前所述：

\begin{tabular}{|l|l|l|}
\hline tag & data & link \\
\hline t & or & \\
\hline f & dlink & \\
\hline
\end{tabular}

\section*{一．拷貝一個串列}
```
function copy(p : listpointer) : listpointer;
    {copy the nonrecursive list with no shared sublists pointed
    at by p}
var q : listpointer;
BEGIN
    q := nil
    if p<>nil the Begin
        new(q);
    q ↑ .tag : = p ↑ .tag;
    if not p ↑ .tag
        then q ↑ .data := p ↑ .data
```