20
資料結構（含精選試題）
Data Structure

\begin{tabular}{|l|l|l|l|}
\hline Statement & S／E & Frequency & Total steps \\
\hline Float sum（int a［ ］［MAX＿SIZE．．］ & 0 & 0 & 0 \\
\hline ｛ & 0 & 0 & 0 \\
\hline int i，j； & 0 & 0 & 0 \\
\hline for（i＝0；i＜rows；i＋＋） & 1 & rows＋1 & rows＋1 \\
\hline for $(\mathrm{j}=0 ; \mathrm{j}<\operatorname{cols} ; \mathrm{j}++)$ & 1 & rows •（cols＋1） & rows •（cols＋1） \\
\hline $\mathrm{c}[\mathrm{i}][\mathrm{j}]=\mathrm{a}[\mathrm{i}][\mathrm{j}]+\mathrm{b}[\mathrm{i}][\mathrm{j}] ;$ & 1 & rows • cols & rows • cols \\
\hline \} & 0 & 0 & 0 \\
\hline Total & \multicolumn{3}{|r|}{2rows＊cols＋2rows＋1} \\
\hline
\end{tabular}

\section*{1－5 Asymptotic Notation $(\mathrm{O}, \Omega, \theta)$}

\section*{1－5－1 Bigoh：O}
\begin{itemize}
\item[（一）] Definition：［Big＂oh＂］ $\mathrm{f}(\mathrm{n})=0(\mathrm{~g}(\mathrm{n}))$
（讀作 ：＂f of n is big oh of g of n＂）
if f there exist two positive constants c and $\mathrm{n}_0$ such that
$\mathrm{f}(\mathrm{n}) \leqq \mathrm{cg}(\mathrm{n})$ for all $\mathrm{n}, \mathrm{n} \geqq \mathrm{n}_0$.
\item[（二）] $f(n)=0(g(n))$ only states that $g(n)$ is an upper bound on the value of $f(n)$ for all $n, n \geqq n_0$ ．
\end{itemize}

\section*{例題 1－19}
\begin{itemize}
\item[（1）] $3 n+2=O(n)$
\begin{itemize}
\item[] $\because 2 n+2 \leqq 4 n$ ，for all $n \geqq 2$（即 $c-4, n_0=2$ ）
\end{itemize}
（2） $100 \mathrm{n}+6=\mathrm{O}(\mathrm{n})$
\begin{itemize}
\item[] $\because 100 \mathrm{n}+6 \leqq 101 \mathrm{n}$ ，for $\mathrm{n} \geqq 10\left(\mathrm{c}=101, \mathrm{n}_0=10\right)$
\end{itemize}
（3） $10 n^2+4 n+2=O\left(n^2\right)$
\begin{itemize}
\item[] $\because 10 \mathrm{n}^2+4 \mathrm{n}+2 \leqq 11 \mathrm{n}^2$ ，for $\mathrm{n} \geqq 5$
\end{itemize}
【 Summary 】
$O(1)=$ Computing time is constant
O（n）＝Linear
\end{itemize}