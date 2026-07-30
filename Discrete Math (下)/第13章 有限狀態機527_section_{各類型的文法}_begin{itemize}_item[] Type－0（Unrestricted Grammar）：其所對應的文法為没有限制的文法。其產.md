第13章 有限狀態機
527

\section*{各類型的文法}
\begin{itemize}
\item[] Type－0（Unrestricted Grammar）：其所對應的文法為没有限制的文法。
其產生規則没有任何限制 $P=\left\{\alpha \rightarrow \beta \mid \alpha, \beta \in(N \bigcup T)^*, \alpha \neq \lambda\right\}$【90清大資應】相對應的機器：turning machine。
\item[] Type－1（Context－Sensitive Grammar）：其所對應的文法為與內容有關的文法。
限制產生規則之右邊符號的個數必須大於或等於左邊符號的個數。
$$
P=\left\{\alpha \rightarrow \beta \mid \alpha, \beta \in(N \bigcup T)^*, \alpha \neq \lambda,\|\alpha\| \leq\|\beta\| \text { or } \alpha \in N, \beta=\lambda\right\} .
$$
相對應的機器：linear bounded automata．
\item[] Type－2（Context－Free Grammar）：其所對應的文法為與內容無關的文法。
限制產生規則之左邊僅能有一個非終端符號。
$$
P=\left\{\alpha \rightarrow \beta \mid \alpha \in N, \beta \in(N \bigcup T)^*\right\} .
$$
【90清大資應】【94成大工科】
相對應的機器：pushdown automata．
\item[] Type－3（Regular－Sensitive Grammar）：其所對應的文法為正規文法。
限制產生規則之左邊與右邊最多只能有一個非終端符號，並且產生規則的右邊也僅能有一個終端符號。【94 成大工科】
$P=\{\alpha \rightarrow \beta \mid \alpha \in N, \beta=\lambda$ ，or $\beta=a$ ，or $\beta=a B$ ，or $\beta=B a, B \in N, a \in T\}$ ，
相對應的機器：finite automata（finite state machine）．
\end{itemize}

Note
若存在 $G$ 為Type－$i$ 的文法生成語言 $L$ ，但不存在Type－$(i+1)$ 的文法生成 $L$ ，則稱 $L$ 為 Type－$i$的語言，$i=0,1,2$ 。另外，可由 Type－3 之文法生成的語言，稱為 Type－3 的語言。