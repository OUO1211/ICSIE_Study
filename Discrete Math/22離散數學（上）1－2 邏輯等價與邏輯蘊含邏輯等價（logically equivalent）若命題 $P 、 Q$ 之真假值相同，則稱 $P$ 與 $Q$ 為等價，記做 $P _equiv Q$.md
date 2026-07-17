22
離散數學（上）

1－2 邏輯等價與邏輯蘊含

邏輯等價（logically equivalent）
若命題 $P 、 Q$ 之真假值相同，則稱 $P$ 與 $Q$ 為等價，記做 $P \equiv Q$ 或 $P \Leftrightarrow Q$ 。
例如，
（1）請證明 $P:(A \vee B) \Rightarrow C$ 與 $Q:(C \Rightarrow B) \vee(\neg C \Rightarrow \neg A)$ 不等價。

【104 台大工科】

解

\begin{tabular}{|c|c|c|c|c|c|}
\hline$A$ & $B$ & $C$ & $(A \vee B)$ & $\Rightarrow$ & $C$ \\
\hline 0 & 0 & 0 & 0 & 1 & 0 \\
\hline 0 & 0 & 1 & 0 & 1 & 1 \\
\hline 0 & 1 & 0 & 1 & 0 & 0 \\
\hline 0 & 1 & 1 & 1 & 1 & 1 \\
\hline 1 & 0 & 0 & 1 & 0 & 0 \\
\hline 1 & 0 & 1 & 1 & 1 & 1 \\
\hline 1 & 1 & 0 & 1 & 0 & 0 \\
\hline 1 & 1 & 1 & 1 & 1 & 1 \\
\hline
\end{tabular}

\begin{tabular}{|c|c|c|c|c|c|}
\hline$A$ & $B$ & $C$ & $(C \Rightarrow B)$ & $\vee$ & $(\neg C \Rightarrow \neg A)$ \\
\hline 0 & 0 & 0 & 1 & 1 & 1 \\
\hline 0 & 0 & 1 & 0 & 1 & 1 \\
\hline 0 & 1 & 0 & 1 & 1 & 1 \\
\hline 0 & 1 & 1 & 1 & 1 & 1 \\
\hline 1 & 0 & 0 & 1 & 1 & 0 \\
\hline 1 & 0 & 1 & 0 & 1 & 1 \\
\hline 1 & 1 & 0 & 1 & 1 & 0 \\
\hline 1 & 1 & 1 & 1 & 1 & 1 \\
\hline
\end{tabular}

由上述真值表可知，$P$ 與 $Q$ 不等價。
（2）$(10 \%)$ 請證明 $[(r \leftrightarrow p) \wedge(p \leftrightarrow q) \wedge(q \leftrightarrow r)] \Leftrightarrow[(r \rightarrow p) \wedge(p \rightarrow q) \wedge(q \rightarrow r)]$ 。
【108中山資工】

\begin{tabular}{|l|l|l|l|l|}
\hline $p$ & $q$ & $r$ & $[(r \leftrightarrow p) \wedge(p \leftrightarrow q) \wedge(q \leftrightarrow r)]$ & $[(r \rightarrow p) \wedge(p \rightarrow q) \wedge(q \rightarrow r)]$ \\
\hline 0 & 0 & 0 & 1 & 1 \\
\hline 0 & 0 & 1 & 0 & 0 \\
\hline 0 & 1 & 0 & 0 & 0 \\
\hline 0 & 1 & 1 & 0 & 0 \\
\hline 1 & 0 & 0 & 0 & 0 \\
\hline 1 & 0 & 1 & 0 & 0 \\
\hline 1 & 1 & 0 & 0 & 0 \\
\hline 1 & 1 & 1 & 1 & 1 \\
\hline
\end{tabular}

因真值表相同，故得䌡。