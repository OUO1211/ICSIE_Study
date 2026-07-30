148
資料結構（含精選試題）
＂

Data Structure
\begin{itemize}
\item[（三）] 第二階段中每一節點最多被放到鏈結堆疊中一次，而因總共只有 2 m 個節點及 forloop 最多執行 $n$ 次，因此時間為 $0(m+n)$ 。
\item[（四）] Space Complexity： $0(\mathrm{~m}+\mathrm{n})$
\end{itemize}

\section*{4－9 Buddy 系統配置及回收法}
\begin{itemize}
\item[一．] Buddy system for memory management 是以＂2的冪次方大小＂作為記憶體配置及回收區塊之大小。
\item[二．] 若系統的 Memory size 為 2 m ，則 Available list 會有（ $\mathrm{m}+1$ ）條串列，以 AV $[\Psi$ ．．m］ofpointer 表示，其中 AV［i］表示大小為2i 的可用空間串列系統初始的 AV lists 如下 ：
\end{itemize}

\section*{三．配置方式}

假設 Process 要求大小為 n 的可用空間，則（一）先計算出 $\mathrm{k}, \mathrm{k}$ 為 $\left\lceil\log _2 \mathrm{n}\right\rceil$
\begin{itemize}
\item[（二）] 令 $\mathrm{j}=\mathrm{k}$ ；
$$
\left\{\begin{array}{c}
\text { while }(\mathrm{j}<=\mathrm{m} \text { and AV }[\mathrm{j}]=\text { nil }) \text { do } \\
\quad \mathrm{j}=\mathrm{j}+1 ;
\end{array}\right.
$$
\item[（三）] while $(\mathrm{j}>\mathrm{k})$ do
begin
\item[] －將 $2^{\mathrm{j}}$ 區塊（起始位址若為p）切割成兩等份
\end{itemize}