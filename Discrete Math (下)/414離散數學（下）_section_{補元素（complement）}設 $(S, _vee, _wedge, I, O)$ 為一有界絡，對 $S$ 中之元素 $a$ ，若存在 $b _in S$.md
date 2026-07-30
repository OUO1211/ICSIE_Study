414
離散數學（下）

\section*{補元素（complement）}

設 $(S, \vee, \wedge, I, O)$ 為一有界絡，對 $S$ 中之元素 $a$ ，
若存在 $b \in S$ ，使得 $\left\{\begin{array}{l}a \vee b=I \\ a \wedge b=O\end{array}\right.$ ，則稱 $b$ 為 $a$ 之補元素，並記為 $b=\bar{a}$ 。
例如圖中，6的補元素是 5 ； 10 的補元素是 3 。

Note
\begin{itemize}
\item[（1）] 在 $(S, \vee, \wedge, I, O)$ 為一有界且分配絡時，對 $S$ 中之元素 $a$ ，若 $a$ 之補元素存在，則唯一。
\item[（2）] $\forall a \in S, \overline{\bar{a}}=a$ ．
\end{itemize}

【97台大資工】

\section*{互補絡（complement lattice）}

在有界絡（ $S, \vee, \wedge, I, O$ ）中，若 $S$ 中的任意元素其補元素均存在，則稱其為互補絡。

\section*{Note}
\begin{itemize}
\item[（1）] $(P(A), \cup, \cap, A, \varnothing)$ 為一互補絡，每個集合的補元素即為其補集。
\item[（2）] （ $D_m, \mathrm{lcm}, \mathrm{gcd}, m, 1$ ）未必為互補絡：例如 $m=30$ 時為互補絡；$m=12$ 時則不是。
判別法：$\left(D_m, \mathrm{lcm}, \operatorname{gcd}, m, 1\right)$ 為互補絡 $\Leftrightarrow m=$ 相異質數相乘。
【91 交大資科】
\end{itemize}

【證明】
⇐ 令 $m=p^2 q$ ，則因為 $p \mid m$ ，故 $p \in D_m$ ，令 $p^{\prime}=p^{-1}$ ，
則 $\left\{\begin{array}{c}p \vee p^{\prime}=m \\ p \wedge p^{\prime}=1\end{array}\right.$ ，得 $\left\{\begin{array}{l}\operatorname{lcm}\left(p, p^{\prime}\right)=m \\ \operatorname{gcd}\left(p, p^{\prime}\right)=1\end{array}\right.$ ，
$\therefore p p^{\prime}=\operatorname{lcm}\left(p, p^{\prime}\right) \times \operatorname{gcd}\left(p, p^{\prime}\right)=m \times 1=p^2 q$ ，
$\therefore p^{\prime}=p q \ldots \ldots$ 與 $\operatorname{gcd}\left(p, p^{\prime}\right)=1$ 矛盾。
故 $p$ 在 $D_m$ 中沒有補元素，故 $D_m$ 不為互補絡。
⇒ 令 $m=p_1 \times \cdots \times p_k$ ：相異質數相乘，
任取 $a \in D_m, ~ a$ 亦為相異質數相乘，則 $\frac{m}{a}$ 即為 $a$ 的補元素。