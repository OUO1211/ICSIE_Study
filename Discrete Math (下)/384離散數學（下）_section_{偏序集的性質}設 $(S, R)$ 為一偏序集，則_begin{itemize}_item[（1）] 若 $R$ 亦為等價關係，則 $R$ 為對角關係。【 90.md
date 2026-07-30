384
離散數學（下）

\section*{偏序集的性質}

設 $(S, R)$ 為一偏序集，則
\begin{itemize}
\item[（1）] 若 $R$ 亦為等價關係，則 $R$ 為對角關係。
【 90 成大工科】【94 暨南資工】【95 交大資訊】
\item[（2）] $\left(S, R^{-1}\right)$ 亦為一偏序集。
\item[（3）] 若 $S^{\prime}$ 為 $S$ 之子集合，則 $\left(S^{\prime}, R\right)$ 亦為一偏序集。
\end{itemize}

【94 交大資訊】
\begin{itemize}
\item[（4）] $R$ 之關係圖形中，不存在有長度大於等於2的迴路（cycle）。
\end{itemize}

【證明】
\begin{itemize}
\item[（1）] ∵ $R$ 為等價關係及偏序關係，所以 $R$ 具有反身性、對稱性、反對稱性、遞移性，因為 $R$ 有反身性，故 $(a, a) \in R, \forall a \in S$ ，
又 if $(a, b) \in R$ ，for some $a \neq b$ ，則因為 $R$ 有對稱性，$\therefore(b, a) \in R$ ，
又因為 $R$ 有反對稱性 $\therefore a=b$ ，不合，故知 $R=\{(a, a) \mid a \in S\}$ ，即 $R$ 為對角關係。
\item[（2）] $\because R$ 為偏序關係，所以 $R$ 具有反身性、反對稱性、遞移性，
另外，之前證明過：$R$ 有反身性 $\Leftrightarrow R^{-1}$ 有反身性；
$R$ 有反對稱性 $\Leftrightarrow R^{-1}$ 有反對稱性；$R$ 有遞移性 $\Leftrightarrow R^{-1}$ 有遞移性；
$\therefore R^{-1}$ 為偏序關係。
\item[（3）] $\forall x \in S^{\prime}, \because x \in S, \therefore x R x$ ，所以 $R$ 在 $S^{\prime}$ 上有反身性；
$\forall x, y \in S^{\prime}, \because x, y \in S$ ，且 $R$ 在 $S$ 上有反對稱性 $\therefore x R y \wedge y R x \Rightarrow x=y$ ，
所以 $R$ 在 $S^{\prime}$ 上亦有反對稱性；
$\forall x, y, z \in S^{\prime}, \because x, y, z \in S$ ，且 $R$ 在 $S$ 上有遞移性 $\therefore x R y, y R z \Rightarrow x R z$ ，
所以 $R$ 在 $S^{\prime}$ 上亦有遞移性，
$\therefore\left(S^{\prime}, R\right)$ 為偏序集。
\item[（4）] 設存在有一 cycle：$a_1-a_2-\ldots-a_k-a_1, k \geq 2, \forall i, a_i \in S$ ，
即 $a_1 R a_2, a_2 R a_3, \ldots, a_{k-1} R a_k, a_k R a_1$ ，
但 $R$ 有遞移性，∴ 由前 $k-1$ 項可知 $a_1 R a_k$ ，而此再與 $a_k R a_1$ ，由反對稱性得 $a_1=a_k$ ，為一矛盾。
\end{itemize}