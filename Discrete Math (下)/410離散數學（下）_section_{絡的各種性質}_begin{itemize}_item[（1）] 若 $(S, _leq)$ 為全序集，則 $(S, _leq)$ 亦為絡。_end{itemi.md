410
離散數學（下）

\section*{絡的各種性質}
\begin{itemize}
\item[（1）] 若 $(S, \leq)$ 為全序集，則 $(S, \leq)$ 亦為絡。
\end{itemize}

【92暨南資工】
\begin{itemize}
\item[（2）] 絡（ $S, \vee, \wedge$ ）滿足下列性質 ：$\forall a, b, c \in S$ ，
\begin{itemize}
\item[（1）] 交換率（commutative law）：$a \vee b=b \vee a, a \wedge b=b \wedge a$ ．
\item[（2）] 一致律（consistent law）：$a \leq b \Leftrightarrow a \vee b=b \Leftrightarrow a \wedge b=a$ ．
\item[（3）] 結合律（associative law）：$a \vee(b \vee c)=(a \vee b) \vee c, a \wedge(b \wedge c)=(a \wedge b) \wedge c$ ．
\item[（4）] 等效律（idempotent law）：$a \vee a=a, a \wedge a=a, \forall a \in S$ ．
\item[（5）] 吸收律（absorptive law）：$a \vee(a \wedge b)=a, a \wedge(a \vee b)=a, \forall a, b \in S$ ．
\end{itemize}
\end{itemize}

【證明】
\begin{itemize}
\item[（1）] ∵ $(A, \leq)$ 為全序 $\therefore \forall a, b \in A, a \leq b$ or $b \leq a$ ，
if $a \leq b$ then $a \vee b=b, a \wedge b=a$ ；
if $b \leq a$ then $a \vee b=a, a \wedge b=b$ ；
再加上 $(A, \leq)$ 本為偏序，故知 $(A, \leq)$ 為絡。
\item[（2）] ①～③請讀者自行練習。
\begin{itemize}
\item[（4）] $\because a \leq a, a \leq a, \therefore a \leq a \wedge a$ ，又 $\because a \wedge a \leq a$ ，∴ 由反對稱性，得 $a \wedge a=a$ 。
$\because a \leq a, a \leq a, \therefore a \vee a \leq a$ ，又 $\because a \leq a \vee a$ ，∴ 由反對稱性，得 $a \vee a=a$ 。
\item[（5）] $\because a \leq a, a \wedge b \leq a, \therefore a \vee(a \wedge b) \leq a$ ，又 $\because a \leq a \vee(a \wedge b)$ ，
∴ 由反對稱性，得 $a \vee(a \wedge b)=a$ 。
$\because a \leq a, a \leq a \vee b, \therefore a \leq a \wedge(a \vee b)$ ，又 $\because a \wedge(a \vee b) \leq a$ ，
∴ 由反對稱性，得 $a \wedge(a \vee b)=a$ 。
\end{itemize}
\end{itemize}

Note
\begin{itemize}
\item[（1）] 之逆敘述不真。
\end{itemize}