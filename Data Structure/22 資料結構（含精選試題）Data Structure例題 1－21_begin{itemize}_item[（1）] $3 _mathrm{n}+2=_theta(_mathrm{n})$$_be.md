22 資料結構（含精選試題）
Data Structure

例題 1－21
\begin{itemize}
\item[（1）] $3 \mathrm{n}+2=\theta(\mathrm{n})$
$\because 3 n+2 \geqq 3 n$ for all $n \geqq 2$ 且 $3 n+2 \leqq 4 n$ for all $n \geqq 2$
\item[（2）] $10 \mathrm{n}^2+4 \mathrm{n}+2=\theta\left(\mathrm{n}^2\right)$
\item[（3）] $10 \log \mathrm{n}+4=\theta(\log \mathrm{n})$
\item[但] $62^{\mathrm{n}}+\mathrm{n}^2 \neq \theta(1), 3 \mathrm{n}+3 \neq \theta\left(\mathrm{n}^2\right), 10 \mathrm{n}^2+4 \mathrm{n}+3 \neq \theta(\mathrm{n})$
\end{itemize}
※ The theta notation is more precise than both the＂big oh＂and＂omega＂notations．

1－6 Time Complexity 之考型
1－6－1［型一］求指令執行次數
例題 1－22
给予下列程式片段，求 $\mathrm{x}=\mathrm{x}+1$ 之執行次數
$$
\left\{\begin{array}{l}
\text { For } \mathrm{i}=1 \text { to } \mathrm{n} \text { do } \\
{\left[\begin{array}{l}
\text { For } \mathrm{j}=1 \text { to } \mathrm{i} \text { do } \\
\mathrm{x}=\mathrm{x}+1
\end{array}\right.} \\
\text { end; }
\end{array}\right.
$$

解 共執行
$$
1+2+3+\cdots+n=\frac{n(n+1)}{2} \text { 次 }
$$
Note：Time Complexity $=\mathrm{O}\left(\mathrm{n}^2\right)$