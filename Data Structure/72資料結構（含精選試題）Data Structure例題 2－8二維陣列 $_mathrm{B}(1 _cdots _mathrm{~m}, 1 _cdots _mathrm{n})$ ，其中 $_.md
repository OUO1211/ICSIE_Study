72
資料結構（含精選試題）
Data Structure

例題 2－8
二維陣列 $\mathrm{B}(1 \cdots \mathrm{~m}, 1 \cdots \mathrm{n})$ ，其中 $\mathrm{B}(2,3)$ 之 Location 為 $18, \mathrm{~B}(3,2)$ 之 Location 為 $28, \mathrm{~A}(1,1)$之 Location 為 2 ，則 B（4，5）之 Location 為？

解 判斷為 Row－major，假設 n 為行數，d 為元素大小。
則 $\mathrm{B}(2,3)=\mathrm{B}(1,1)+[(2-1) * \mathrm{n}+(3-1)] * \mathrm{~d}$
$$
\begin{align*}
& 18=2+\mathrm{nd}+2 \mathrm{~d}  \tag{1}\\
& \mathrm{~B}(3,2)=\mathrm{B}(1,1)+[(3-1) * \mathrm{n}+(2-1)] * \mathrm{~d} \\
& 28=2+2 \mathrm{nd}+\mathrm{d} \tag{2}
\end{align*}
$$
（1）$* 2$－（2）
$$
\begin{aligned}
& 8=2+3 d \quad \therefore d=2 \text { 代回 }(1 \\
& 18=2+2 n+4 \quad \therefore n=6 \\
& \therefore B(4,5)=B(1,1)+[(4-1) * 6+(5-1)] * 2 \\
& \quad=2+36+8=46
\end{aligned}
$$

例題 2－9
二維陣列 x ，其中 $\mathrm{x}[0,0], \mathrm{x}(0,1)$ 及 $\mathrm{x}(1,0)$ 之位址分為 $100,102,106$ ，求 $\mathrm{x}(4,5)$ 之位址為？
解 x（4，5）之位址為174。
例題 2－10
Array 於某些應用相當方便，問：
\begin{itemize}
\item[（1）] 說明它在何種狀況下不適用？
\item[（2）] 若原有 n 筆資料，以 Array 存放，試計算插入一新的資料，平均需移動幾筆資料？【高考類似題】
\end{itemize}

解（1）當加入／刪除很多時，須移動其它元素，非常不便。
\begin{itemize}
\item[（2）]
$$
\begin{aligned}
& (n+(n-1)+\cdots 3+2+1) \times 1 / n \\
& =\frac{n(n+1)}{2} \cdot 1 / n=\frac{n+1}{2}
\end{aligned}
$$
\end{itemize}

三 ．三維陣列
宣告方式：陣列 $\mathrm{A}\left(1: \mu_1, 1: \mu_2, 1: \mu_3\right)$