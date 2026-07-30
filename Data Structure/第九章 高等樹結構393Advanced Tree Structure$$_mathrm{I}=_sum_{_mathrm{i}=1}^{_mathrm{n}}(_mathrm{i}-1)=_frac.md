第九章 高等樹結構
393
Advanced Tree Structure
$$
\mathrm{I}=\sum_{\mathrm{i}=1}^{\mathrm{n}}(\mathrm{i}-1)=\frac{\mathrm{n}(\mathrm{n}-1)}{2}
$$
（二）當二元樹是 Complete Binary Tree 時，具有最小的 I。

\section*{9－4 Minimal Weighted External Path Length}

一．加權外部路徑長度
定義：
給定 n＋1組正加權值 $\mathrm{q}_1, \cdots, \mathrm{q}_{\mathrm{n}+1}$ 。每個加權值對應於二元樹的 n＋1個外部節點。此二元樹的加權外部路徑長度（Weighted External Path Length）定義為 ：
$$
\sum_{1 \leq i \leq n+1} q_i k_i
$$
其中 $\mathrm{k}_{\mathrm{i}}$ 是從根部到權值 $\mathrm{q}_{\mathrm{i}}$ 的外部節點之距離。
例如：
假設 $\mathrm{n}=3$ 同時我們給定4個權值： $\mathrm{q}_2=15, \mathrm{q}_2=2, \mathrm{q}_3=4, \mathrm{q}_4=5$下圖顯示出2種可能的樹。
它們的加權外部路徑長度分別為
$$
\text { 和 } \begin{aligned}
& 2 \times 3+4 \times 3+5 \times 2+15 \times 1=43 \\
& 2 \times 2+4 \times 2+2 \times 5+15 \times 2=52
\end{aligned}
$$