第七章 搜尋與排序 329
Search＆Sort
\begin{itemize}
\item[（五）] 評估
\begin{itemize}
\item[1．] Heap sort 之 Best，Average，Worst Case 均為 $0(\mathrm{n} \log \mathrm{n})$ 。假設 $2^{\mathrm{k}-1} \leq \mathrm{n} \leq 2^{\mathrm{k}}$ ，因此二元樹之階度為 k 且第 i 階段之節點數是 $2^{\mathrm{i}-1}$ 在第一個 for 迴圈中，對於每一個有兒子的節點都要呼叫 Adjust 一次，因此此迴圈之費時是將每一階度中節點數與該階度中之節點可能移動之最長距離的乘積累加起來，即：
$$
\sum_{1 \leq i \leq k} 2^{i-1}(k-i)=O(n)
$$
在第二 for 迴圈中，呼叫了 Adjust 程序 n－1 次，且呼叫最高深度為：$\mathrm{k}=\left[\log _2(\mathrm{n}+1)\right]$ ，因此此迴圈之費時為 $0(\mathrm{n} \log \mathrm{n})$ 。因此，總共之計算時間$0(n+n \log n)=0(n \log n)$ 。
\item[2．] Unstable Sorting Method
\item[3．] Space complexity： $\mathrm{O}(1)$
\end{itemize}
\item[四．] 基數排序法（Radix Sort Method）
\begin{itemize}
\item[] －此排序法又稱為 Bin Sort 或 Bucket Sort，它是屬於分配模式的排序技巧。
\end{itemize}
\end{itemize}