第12章 代數結構
445

\section*{關於群上的運算的交換性}

考虑群 $(G, *)$ ，且單位元素為 $e$ ，
\begin{itemize}
\item[（1）] If $x^* x=e, \forall x \in G$ ，then $(G, *)$ is an abelian group．
\item[（2）] If $(a * b)^2=a^2 * b^2, \forall a, b \in G$ then $(G, *)$ is an abelian group．
\item[（3）] If $|G| \leq 4$ ，then $(G, *)$ is an abelian group．
\end{itemize}

【證明】
\begin{itemize}
\item[（1）] 由題意，$\forall a, b \in G, a^* a=e, b^* b=e,\left(a^* b\right)^*\left(a^* b\right)=e$ ，
$$
\begin{aligned}
& \therefore a^{-1}=a, b^{-1}=b,\left(a^* b\right)^{-1}=\left(a^* b\right), \\
& \therefore a^* b=\left(a^* b\right)^{-1}=b^{-1} * a^{-1}=b^* a, \text { 所以此為交換群。 }
\end{aligned}
$$
\item[（2）] 由題意，$\forall a, b \in G,\left(a^* b\right)^*\left(a^* b\right)=\left(a^* b\right)^2=(a * a)^*\left(b^* b\right)$ ，
$$
\begin{aligned}
& \therefore a^{-1}\left(a^* b\right) *\left(a^* b\right)=a^{-1} *\left(a^* a\right)^*\left(b^* b\right), \\
& \therefore b^*\left(a^* b\right)=a^*\left(b^* b\right), \\
& \therefore b^*\left(a^* b\right) * b^{-1}=a^*\left(b^* b\right)^* b^{-1}, \\
& \therefore b^* a=a^* b, \text { 所以此為交換群。 }
\end{aligned}
$$
\item[（3）] 可如下一一列出其二元運算表，檢查得均為交換群，或用循環群那裡更簡單的方法。

\begin{tabular}{|l|l|l|l|l|l|l|l|l|}
\hline & & ＊ & $e$ & $a$ & ＊ & $e$ & $a$ & $b$ \\
\hline ＊ & $e$ & $e$ & & & $e$ & $e$ & $a$ & b \\
\hline $e$ & $e$ & a & $e$ & a & $a$ & $a$ & $b$ & $e$ \\
\hline & & & $a$ & $e$ & $b$ & $b$ & $e$ & $a$ \\
\hline
\end{tabular}

\begin{tabular}{|l|l|l|l|l|l|l|l|l|l|l|l|l|l|l|l|l|l|l|l|}
\hline ＊ & $e$ & $a$ & $b$ & $c$ & ＊ & $e$ & $a$ & $b$ & $c$ & ＊ & $e$ & $a$ & $b$ & $c$ & ＊ & $e$ & $a$ & $b$ & $c$ \\
\hline $e$ & $e$ & $a$ & $b$ & $c$ & $e$ & $e$ & $a$ & $b$ & $c$ & $e$ & $e$ & $a$ & $b$ & $c$ & $e$ & $e$ & $a$ & $b$ & $c$ \\
\hline $a$ & a & e & $c$ & $b$ & $a$ & a & $e$ & $c$ & $b$ & $a$ & $a$ & $c$ & $e$ & $b$ & $a$ & $a$ & $b$ & $c$ & $e$ \\
\hline $b$ & b & $c$ & $e$ & $a$ & $b$ & b & $c$ & a & $e$ & $b$ & b & $e$ & $c$ & $a$ & $b$ & $b$ & $c$ & e & $a$ \\
\hline $c$ & $c$ & $b$ & a & $e$ & $c$ & $c$ & $b$ & $e$ & $a$ & $c$ & c & $b$ & $a$ & $e$ & $c$ & c & e & $a$ & $b$ \\
\hline
\end{tabular}
Note
但後3個彼此同構（其實就是 $\left(Z_4,+{ }_4\right)$ ），而與第1個不同構。
\end{itemize}