第13章 有限狀態機
555

\section*{13－4 決定性與非決定性}

決定性／非決定性有限狀態機
（Deterministic／Nondeterministic Finite State Machine）
一個有限狀態機
\begin{itemize}
\item[（1）] 若滿足對每一個輸入符號皆有唯一的下個狀態，則稱為決定性有限狀態機。
\item[（2）] 若滿足對某個輸入符號可有任意個下個狀態，則稱為非決定性有限狀態機。
\end{itemize}

Note
\begin{itemize}
\item[（1）] 同理可定義決定性有限自動機（D．F．S．A．）與非決定性有限自動機（N．F．S．A．）
\item[（2）] 設 M 為一 N．F．S．A．認知語言 $L$ ，則存在一 D．F．S．A．$M^{\prime}$ 認知 $L$ ．
【91 北科資工】
\end{itemize}

例題 1
\begin{itemize}
\item[（1）] （10％）Find the state diagram for the nondeterministic finite－state automaton with the following state table．The final state are $s_2$ and $s_3$.
【98政大資科】
\item[（2）] Find the language recognized by the given non－deterministic finite－state automaton．
\item[（3）] Find a deterministic automaton that recognizes the same language in（2）．
\end{itemize}

解（1）如右圖。
\begin{itemize}
\item[（2）] $\{\lambda\} \cup\left\{01^i \mid i \geq 0\right\} \cup\left\{0^i 1^j \mid i, j \geq 1\right\}$ ．
\item[（3）]

\begin{tabular}{|l|l|l|l|}
\hline \multirow{2}{*}{State} & \multicolumn{2}{|r|}{Input} & \multirow[t]{2}{*}{Output} \\
\hline & 0 & 1 & \\
\hline $\rightarrow\{A\}$ & ｛ $B C$ \} & $\varnothing$ & 1 \\
\hline ｛B\} & ｛B\} & $\{C\}$ & 0 \\
\hline ｛C\} & $\varnothing$ & $\{C\}$ & 1 \\
\hline （BC） & ｛B\} & ｛C\} & 1 \\
\hline $\varnothing$ & $\varnothing$ & $\varnothing$ & 0 \\
\hline
\end{tabular}
\end{itemize}