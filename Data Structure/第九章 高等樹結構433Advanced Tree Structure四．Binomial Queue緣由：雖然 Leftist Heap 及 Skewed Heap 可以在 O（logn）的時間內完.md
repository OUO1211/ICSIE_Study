第九章 高等樹結構
433
Advanced Tree Structure

四．Binomial Queue
緣由：雖然 Leftist Heap 及 Skewed Heap 可以在 O（logn）的時間內完成 Merge，Insert 及Delete Min 的運作。而 Binomial Queue 雖在此三個 operation 的 worst time 為O（logn），但對於 Insert 之平均操作為 O（1）時間
\begin{itemize}
\item[] Def：①Binomial Queue 為許多Heap－orderd Tree 的集合（i．e．Forest）每個 Heap tree 都是一個二項式樹
\begin{itemize}
\item[（2）] 高度為 $\phi$ 的二項式樹是只有一個 Node 的樹高度為 k 的二項式樹 $\mathrm{B}_{\mathrm{k}}$ ，由二個 $\mathrm{B}_{\mathrm{k}-1}$ 的二項式樹構成，且 $\mathrm{B}_{\mathrm{k}-1}$ Tree 指向另一個 $\mathrm{B}_{\mathrm{k}-1}$ 樹之樹根
\item[e．] g．
\end{itemize}
\item[] Note ：（1）高度為 k 的二項式樹之節點數為 $2^{\mathrm{k}}$ 個
\item[（2）] 深度為 d 的節點個數為 $\binom{\mathrm{k}}{\mathrm{d}}$（root Level 為 $\phi$ ）
\begin{itemize}
\item[（3）] 13 個元素的 priority Queue 可以用 $\mathrm{B}_3, \mathrm{~B}_2, \mathrm{~B}_0$ 表示
\item[（4）] e．g． 6 個元素的 priority Queue 以 Binomial Queue 表示如下：
\end{itemize}
\end{itemize}

五．Binomial Queue 之 Merge 動作
例：