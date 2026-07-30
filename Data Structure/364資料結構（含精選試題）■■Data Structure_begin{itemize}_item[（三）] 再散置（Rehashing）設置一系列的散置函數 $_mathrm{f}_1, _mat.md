364
資料結構（含精選試題）
■■
Data Structure
\begin{itemize}
\item[（三）] 再散置（Rehashing）
設置一系列的散置函數 $\mathrm{f}_1, \mathrm{f}_2, \cdots, \mathrm{f}_{\mathrm{n}}$ 。當使用 $\mathrm{f}_1$ 產生溢位時，則改用 $\mathrm{f}_2$ ，若 $\mathrm{f}_2$ 又發生溢位時，則改用 $\mathrm{f}_3$ ，直到沒有溢位發生為止。
\item[（四）] 鏈結（Chain 或叫 Link list）
首先將所有的散置空間建立 b 個串列，起初只有 b 個串列首，之後若有相同位址的識別字則將其鏈結其後，成為鏈結串列，直到所有的可用空間都用完為止。例：識別字 GA，D，A，G，L，A2，A1，A3，A4，Z，ZA 及 E 以鏈結串列法存放於散置表中。
\end{itemize}