82
資料結構（含精選試題）
Data Structure

假設 band matrix 將最下的對角線元素依序储存到 B 一維陣列當中，如下所示：
\begin{itemize}
\item[] B：

\begin{tabular}{|l|l|l|l|l|l|l|l|l|l|l|l|}
\hline ［1］ & ［2］ & ［3］ & ．． & ．． & ．． & ．． & ．． & ．． & ．． & ．． & ［12］ \\
\hline 9 & 7 & 8 & 3 & 6 & 0 & 0 & 2 & 1 & 3 & 4 & 9 \\
\hline
\end{tabular}
\end{itemize}

Please answer the following questions：
\begin{itemize}
\item[（1）] How many elements are there in the band of $\mathrm{A}_{\mathrm{n}, \mathrm{a}, \mathrm{b}}$ ？
\item[（2）] How many elements of the band are there in the i－th row of $\mathrm{A}_{\mathrm{n}, \mathrm{a}, \mathrm{b}}$ ？
\item[（3）] Considering B ，the sequential representation of the band matrix $\mathrm{A}_{100,20,30}$ What is $\operatorname{LOC}\left(\mathrm{A}_{60,65}\right)$ in B？
\item[（4）] Let $\mathrm{a}_{\mathrm{i}, \mathrm{j}}$ be the element of $\mathrm{A}_{100,20,30}$ located in B（150）．
\end{itemize}

What are the values of $i$ and $j$ respectively？
\begin{itemize}
\item[] 解（1） $\mathrm{n}+\frac{(\mathrm{a}-1)(2 \mathrm{n}-\mathrm{a})}{2}+\frac{(\mathrm{b}-1)(2 \mathrm{n}-\mathrm{b})}{2}$
\begin{itemize}
\item[（2）] $(\mathrm{a}+\mathrm{b}-1)-\mathrm{O}_{\mathrm{a}}-\mathrm{O}_{\mathrm{b}}$
其中，$O_{\mathrm{a}}=\left\{\begin{array}{l}\varnothing, \mathrm{i} \geq \mathrm{a} \\ \mathrm{a}-\mathrm{i}, \mathrm{i}<\mathrm{a}\end{array}\right.$
$$
O_b=\left\{\begin{array}{l}
\varnothing, i \leq n-b+1 \\
i-(n-b+1), i>n-b+1
\end{array}\right.
$$
\item[（3）] 2260
\item[（4）] $i=87, j=69$
\end{itemize}
\end{itemize}