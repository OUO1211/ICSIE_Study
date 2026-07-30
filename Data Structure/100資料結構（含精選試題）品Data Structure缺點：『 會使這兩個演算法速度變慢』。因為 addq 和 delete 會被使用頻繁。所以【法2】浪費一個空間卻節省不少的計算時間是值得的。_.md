100
資料結構（含精選試題）
品

Data Structure
缺點：『 會使這兩個演算法速度變慢』。因為 addq 和 delete 會被使用頻繁。所以【法2】浪費一個空間卻節省不少的計算時間是值得的。
\begin{itemize}
\item[四．] Queue 的應用
\begin{itemize}
\item[（一）] 在作業系統中的 job scheduling，在相同的 Priority 之下，利用 queue，來完成先到先做的原則。
\item[（二）] 有許多 I／O 同時要求處理，即 I／O device Queue 將所有的 I／O 要求，利用 queue 來使之先到先做。
\item[（三）] Priority queue，為一不遵守 FIFO 的特性，而是最高優先權者先出（Highest Priorityout First）。
\item[（四）] 用於模擬（simulation）方面，例：佇列理論。模擬是一種將現實情況建立出一種抽象模式，以便瞭解在各種因素下的影響，以來改善實際的情況。在模擬系統中，經常有 time－driven 或者 event－driven 的輸入訊號，這些訊號到達時間不一，需要使用 queue 來 simulation。
\item[（五）] 作為輸出入工作的 buffer，也是採用先到先作的佇列。
\item[（六）] 日常生活中排隊的行為也是 queue。
\end{itemize}
\item[五．] Deque（Double－Ended Queue）雙向佇列
\item[（一）] 一個 queue 兩端同時都可以加入與刪除
\end{itemize}

【註】常用的 deque 有二種型式：
Input－Restricted Deque 限制在一端加入，而兩端均可刪除。
Output－Restricted Deque 限制在一端刪除，而兩端均可加入。
\begin{itemize}
\begin{itemize}
\item[（二）] 動作製作：ADD 與 Delete。
$$
\begin{aligned}
\text { 初值 } \rightarrow \text { rear } 1 & =\text { front } 1=0 \\
& \text { rear } 2=\text { front } 2=\mathrm{n}-1
\end{aligned}
$$
\item[1．] Procedure ADD（item，leftin，q）
BEGIN
\end{itemize}
\end{itemize}