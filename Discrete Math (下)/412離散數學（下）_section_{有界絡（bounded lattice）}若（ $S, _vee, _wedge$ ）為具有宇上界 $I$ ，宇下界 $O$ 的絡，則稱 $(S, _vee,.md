412
離散數學（下）

\section*{有界絡（bounded lattice）}

若（ $S, \vee, \wedge$ ）為具有宇上界 $I$ ，宇下界 $O$ 的絡，
則稱 $(S, \vee, \wedge)$ 為一有界絡，並記成 $(S, \vee, \wedge, I, O)$ 。
例如
（ $N, \max , \min$ ）中，宇下界為 1 ，沒有宇上界。
$(P(A), \bigcup, \bigcap)$ 中，宇下界為 $\varnothing$ ，宇上界為 $A$ ，記成 $(P(A), \cup, \cap A, \varnothing)$ 。
$\left(D_m, \mathrm{lcm}, \mathrm{gcd}\right)$ 中，宇下界為 1 ，宇上界為 $m$ ，記成 $\left(D_m, \mathrm{lcm}, \mathrm{gcd}, m, 1\right)$ 。

Note
\begin{itemize}
\item[（1）] 設 $(S, \leq)$ 為一有限的偏序集，則
\begin{itemize}
\item[（1）] $\forall a, b \in S, \operatorname{lub}(a, b)$ 存在 $\Leftrightarrow(S, \leq)$ 具有宇上界 $I$ 。
\item[（2）] $\forall a, b \in S, \operatorname{glb}(a, b)$ 存在 $\Leftrightarrow(S, \leq)$ 具有宇下界 $O$ 。
\end{itemize}
\item[（2）] 若 $(S, \leq)$ 為一有限絡，則 $(S, \leq)$ 具有宇上界 $I$ 及宇下界 $O$ ，但反之不成立。
\item[（3）] 令 $(S, \vee, \wedge, I, O)$ 為一有界絡，則
$\forall a \in S, a \vee I=I, a \wedge I=a ; a \vee O=a, a \wedge O=O$ ．
\item[（4）] 設 $(S, \vee, \wedge, I, O)$ 為一有界絡，$a, b \in S$ ，
\begin{itemize}
\item[（1）] 若 $a \leq b$ 且不存在 $c \in S$ 使得 $a \leq c, c \leq b$ ，則稱 $b$ 覆蓋（cover）$a 。$
\item[（2）] 若 $a$ 覆蓋 $O$ ，則稱 $a$ 為一原子（atom）。
\item[（3）] 若 $I$ 覆蓋 $a$ ，則稱 $a$ 為一對偶原子（dual atom）。
\end{itemize}
\end{itemize}