第七章 搜尋與排序
319
Search＆Sort
$$
\begin{aligned}
\frac{T(n)}{n} & =c\left(\frac{1}{n}+\frac{1}{n-1}+\cdots+\frac{1}{2}\right)+c\left(\frac{1}{n-1}+\frac{1}{n-2}+\cdots+1\right) \\
& =c\left(H_n-1\right)+c H_{n-1} \\
& =c\left(H_n+H_{n-1}-1\right) \\
& =c\left(2 H_e-1 / n-1\right) \\
& =c\left(2 H_n-(n+1) / n\right) \\
T(n) & =2 H_n c n-c(n+1) \\
& \fallingdotseq 2 c n \log n-c(n+1) \\
& =O(n \log n)
\end{aligned}
$$
\begin{itemize}
\item[（四）] 快速排序不是一個穩定的排序（Unstable Method）
\item[（五）] 在額外的空間需求方面。它需要有一些空間當作堆疊來完成遞迴的特性。如果每次檔案都是平均分割，那遞迴叫之最高深度是 $\log _2 \mathrm{n}$ ，因此所需之堆疊空間是$0(\operatorname{logn})$ 。最壞的情況下，是每次分割出來的兩個部份檔案中右邊的大小為零而左邊的則為原來的大小減1，此種情形下遞迴呼叫的深度將等於 n，因此所需之空間是 0（n）。
\item[] —補充：排序能達多快？
如果將此問題限制在只能做比較與對調的演算法，那可以證明一個定理顯示可能之最佳時間是 $0\left(n \log _2 n\right)$ 。
將利用決策樹（Decision Tree）來描述排序的過程，其中每一個節點代表一次鍵的比較，而分支則代表比較之結果。決策樹中的一條路徑即代表演算法所可能產生的一串比較順序。
下圖所示就是 3 個資料排序的結果，其中樹葉節點編號成（1）到（6），只有在到達這些樹葉節點時演算法才會停止。從下圖中，我們可以看出此樹的最高深度是4。
\end{itemize}

\begin{tabular}{|l|l|l|}
\hline 樹葉 & 排 列 & 產生此得排列之鍵 \\
\hline ① & 123 & （7，9，10） \\
\hline （2） & 132 & （7，10，9） \\
\hline （3） & 312 & （9，10，7） \\
\hline （4） & 213 & （9，7，10） \\
\hline （5） & 231 & （10，7，9） \\
\hline ⑥ & 321 & （10，9，7） \\
\hline
\end{tabular}