第七章 搜尋與排序 311
Search＆Sort

\section*{例題 7－1}

設 n＝5 且輸入之記錄順序為（5，4，3，2，1）則插入排序之過程如下所示：
初始順序

\begin{tabular}{|l|l|l|l|l|l|l|}
\hline $-\infty$ ， & 5， & 4， & 3， & 2， & 1 & $i=2$ \\
\hline $-\infty$ ， & 4， & 5， & 3， & 2， & 1 & $\mathrm{i}=3$ \\
\hline $-\infty$ ， & 3， & 4， & 5， & 2， & 1 & $\mathrm{i}=4$ \\
\hline $-\infty$ ， & 2， & 3， & 4， & 5， & 1 & $\mathrm{i}=5$ \\
\hline $-\infty$ ， & 1， & 2， & 3， & 4， & 5 & \\
\hline
\end{tabular}

\section*{例題 7－2}

設 n＝5 且輸入記錄順序為（2，3，4，5，1），那麼插入排序之過程如下：
初始順序

\begin{tabular}{|l|l|l|l|l|l|l|}
\hline $-\infty$ ， & 2， & 3， & 4， & 5， & 1 & $\mathrm{i}=2$ \\
\hline $-\infty$ ， & 2， & 3， & 4， & 5， & 1 & $\mathrm{i}=3$ \\
\hline $-\infty$ ， & 2， & 3， & 4， & 5， & 1 & $\mathrm{i}=4$ \\
\hline $-\infty$ ， & 2， & 3， & 4， & 5， & 1 & $\mathrm{i}=5$ \\
\hline $-\infty$ ， & 1， & 2， & 3， & 4， & 5 & \\
\hline
\end{tabular}
在執行插入排序中，首先視 $\mathrm{R}_0 、 \mathrm{R}_1$ 為排序好之記錄，然後將 $\mathrm{R}_2, \mathrm{R}_3, \cdots, \mathrm{R}_0$ 依順序地一個個插入。因為每次插入後之結果是排好序的，因此一個具有 $n$ 個記錄的檔案在做n－1 次插入後即可排序好。

\section*{－插入排序法的分析}
\begin{itemize}
\item[1．] 在最壞情況下，Insort（r，list，i）要做 i＋1 此比較才能完成插入的動作，因此其計算時級數為 O（i）。Insort 演算法則是由 $\mathrm{i}=1,2, \cdots, \mathrm{n}-1$ 每次呼叫 Insert 來完成排序之工作，因此在最壞的情況下，Insort 之計算時間級數為：
$$
\mathrm{O}\left(\sum_{\mathrm{r}=1}^{\mathrm{n}-1} \mathrm{i}\right)=\mathrm{O}\left(\mathrm{n}^2\right)
$$
\item[2．] 平均計算時間亦為 $0\left(\mathrm{n}^2\right)$ ，Best case（已照順序排序好者）為 $0(\mathrm{n})$（因為只需 $\mathrm{n}-1$ 次的比較）。
\item[3．] 插入排序法是穩定的。
\begin{itemize}
\item[e．] g．$\cdots 5 \cdots 5^{+} \cdots \cdots$
\end{itemize}
\end{itemize}