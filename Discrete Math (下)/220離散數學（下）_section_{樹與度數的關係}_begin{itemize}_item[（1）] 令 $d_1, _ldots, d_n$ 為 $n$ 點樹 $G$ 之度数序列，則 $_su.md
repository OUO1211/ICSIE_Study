220
離散數學（下）

\section*{樹與度數的關係}
\begin{itemize}
\item[（1）] 令 $d_1, \ldots, d_n$ 為 $n$ 點樹 $G$ 之度数序列，則 $\sum_{i=1}^n d_i=2(n-1)$ 。
【85、87台大資工】【90交大應數】【99政大資科】
\item[（2）] 設 $G$ 為非退化樹，則 $G$ 中至少含2個度数為1的點。
【94暨南資工】【89、100中山資工】
\end{itemize}

【證明】
\begin{itemize}
\item[（1）] $\sum_{i=1}^n d_i=2|E(G)|=2(n-1)$ 。
\item[（2）] 令 $P$ 為 $G$ 之最長路徑（path）：$v_1-v_2-\ldots-v_k$ ，
則 $\operatorname{deg} v_1=1$（不然設 $v_t$ 與 $v_1$ 相鄰，若 $t \in\{3, \ldots, k\}$ ，則表示 $G$ 中存在一 cycle，矛盾；若$t \notin\{3, \ldots, k\}$ ，則表示 $v_t-v_1-v_2 \ldots-v_k$ 為 $G$ 之更長路徑，矛盾），
同理亦可得 $\operatorname{deg} v_k=1$ ，故 $G$ 中至少兩點度數為1。
\end{itemize}

Note
\begin{itemize}
\item[（1）] 若 $n$ 點圖 $G$ 是恰含 $k$ 棵樹的森林，則 $\sum_{i=1}^n d_i=2(n-k)$ 。【85、87台大資工】
【證明】
因為有 $k$ 樹，所以 $|E|=n-k$ ，再由 $\sum_{v \in V} \operatorname{deg}(v)=2|E|$ 即得證。
\item[（2）] 度數為1的點又稱懸吊點（pendant vertex）或葉子（leaf）。
\item[（3）] 若 $T$ 中恰含2個度數為1的點，則 $T$ 為一path。
\item[（4）] 若 $\sum_{i=1}^n d_i=2(n-1)$ 且 $d_i \geq 1, \forall i$ ，則 $\left\{d_i\right\}_{i=1}^n$ 必為某樹之度數序列。
【 92 成大電機】【 102 台大電機】【 $90 、 103$ 交大應數】
\end{itemize}

【證明】
對 $n$ 以歸納法討論如下：
$n=2$ ，此時即只 $d_1, d_2$ ，且 $d_1=d_2=1$ ，的確存在一樹度數序列為1，1。
設 $n=k \geq 2$ 時，命題成立，
即若 $\sum_{i=1}^k d_i=2(k-1)$ ，則 $d_1, d_2, \ldots, d_k$ 必為某樹之度數序列。
則 $n=k+1$ 時，