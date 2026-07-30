第一章 基本概念
29
Basic Concepts

\section*{1—8 常用的對數數學公式}

Logarithms：

\begin{tabular}{|l|l|}
\hline \begin{itemize}
\item[] － $\log ^{\mathrm{k}} \mathrm{n}=(\log \mathrm{n})^{\mathrm{k}}$
\item[] － $\log \log \mathrm{n}=\log (\log \mathrm{n})$
\item[] － $\mathrm{a}=\mathrm{b}^{\log _{\mathrm{b}} \mathrm{a}}$
\item[] － $\log _{\mathrm{c}}(\mathrm{ab})=\log _{\mathrm{c}} \mathrm{a}+\log _{\mathrm{c}} \mathrm{b}$
\item[] － $\log _{\mathrm{b}} \mathrm{a}^{\mathrm{n}}=\mathrm{n} \log _{\mathrm{b}} \mathrm{a}$
\end{itemize} & \begin{itemize}
\item[] － $\log _{\mathrm{b}}{ }^{\mathrm{a}}=\frac{\log _{\mathrm{c}}{ }^{\mathrm{a}}}{\log _{\mathrm{c}}{ }^{\mathrm{b}}}$
\item[] － $\log _{\mathrm{b}}{ }^{(1 / \mathrm{a})}=-\log _{\mathrm{b}}{ }^{\mathrm{a}}$
\item[] － $\log _{\mathrm{b}}{ }^{\mathrm{a}}=\frac{1}{\log _{\mathrm{a}}{ }^{\mathrm{b}}}$
\item[] －$a^{\log _b c}=c^{\log _b a}$
\end{itemize} \\
\hline
\end{tabular}

例題 1－39
Evaluate $\sum_{\mathrm{k}=0}^{\log \mathrm{n}} \mathrm{k} 2^{\mathrm{k}}$
解 $\sum_{\mathrm{k}=0}^{\mathrm{n}} \mathrm{x}^{\mathrm{k}}=\frac{\mathrm{x}^{\mathrm{n}+1}-1}{\mathrm{x}-1}$（等比數列）
$$
\sum_{k=1}^n k x^{k-1}=\frac{n x^{n+1}-n x^n-x^n+1}{(x-1)^2}
$$
Multiply by x：
$$
\begin{aligned}
\sum_{k=1}^n k x^k= & \frac{n x^{n+2}-n x^{n+1}-x^{n+1}+x}{(x-1)^2} \\
\Rightarrow \sum_{k=0}^{\log n} k 2^k & =\phi+\sum_{k=1}^{\log n} k 2^k \\
& =(\log n)\left(2^{\log n+2}\right)-(\log n)\left(2^{\log n+1}\right)-2^{\log n+1}+2 \\
& =4 n \log n-2 n \log n-2 n+2 \\
& =2 n \log n-2 n+2
\end{aligned}
$$