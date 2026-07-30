第九章 高等樹結構
437
Advanced Tree Structure

而 17 的分攤成本等於 actual cost
$$
\Rightarrow 2+2+6+2+2+2+2+6+1=25=\text { 分攤成本加總 }=\text { actual cost 加總 }
$$
因此，若每一 Insert 的 amortized cost 不超過2
每一 Delete 的 amortized cost 不超過 6
則實際成本不會超過2i＋6d，i，d 分為在順序中 Insert 及 Delete min 之運算次數$\therefore \min \{2 \mathrm{i}+6 \mathrm{~d}, \mathrm{i}+\operatorname{cod}\}$ 為順序成本之上限

\section*{九．Binomial Heap 種類}

L＿Min－Binomial Heap ：最小樹之集合
Max－Binomial Heap：最大樹之集合
\begin{itemize}
\item[] 例：min－Binomial Heap
\item[（一）] 使用 Binomial Heap
Insertion 和 Combine 可以在 O（1）實際和分攤時間完成
Delete min element 則在 $O(\operatorname{logn})$ 分攤時間內完成
\item[（二）] Node structure
degree，child，left－link，right－link，data
degree：record 子點個數
child：pointer to any one child
left－link，right－link：用以維持在 sibiling nodes 之間的 double link circular list
此外，各樹之 Root 亦形成 Double link circular list
\end{itemize}