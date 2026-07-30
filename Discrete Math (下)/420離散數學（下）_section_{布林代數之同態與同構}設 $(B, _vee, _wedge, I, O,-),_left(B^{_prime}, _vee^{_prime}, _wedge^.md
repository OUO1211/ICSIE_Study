420
離散數學（下）

\section*{布林代數之同態與同構}

設 $(B, \vee, \wedge, I, O,-),\left(B^{\prime}, \vee^{\prime}, \wedge^{\prime}, I^{\prime}, O^{\prime},-^{\prime}\right)$ 為二個布林代數，
若存在一函数 $f: B \rightarrow B^{\prime}$ 滿足：
$\forall a, b \in B, \quad f(a \vee b)=f(a) \vee^{\prime} f(b) ; \quad f(a \wedge b)=f(a) \wedge^{\prime} f(b) ; \quad f(\bar{a})=\overline{f(a)}$ ．
則稱 $f$ 為由 $B$ 至 $B^{\prime}$ 之布林代數同態函數。
若 $f$ 亦為 1－1 且 onto 時，
則稱 $f$ 為由 $B$ 至 $B^{\prime}$ 之布林代數同構函數，且稱 $B$ 與 $B^{\prime}$ 同構，記做 $B \cong B^{\prime}$ 。
Note
令 $B_n$ 為一具有 $n$ 個原子 $m_1, \ldots, m_n$ 的布林代數，令 $M=\left\{m_1, \ldots, m_n\right\}$ ，則 $\left(B_n, \vee, \wedge, I, O,-\right) \cong\left(P(M), \cup, \cap M, \varnothing,^c\right)$,
其中符號對應如下 ：$\vee \leftrightarrow \cup, \wedge \leftrightarrow \cap, I \leftrightarrow M, O \leftrightarrow \varnothing,-\leftrightarrow^c, \leq \leftrightarrow \subseteq$ ；且可得：$\left|B_n\right|=2^n$ 。
【證明提示】
定義函數 $f: B_n \rightarrow P(M)$ ，by $\forall a \in B_n, f(a)=\{m \in M \mid m \leq a\}$ ，再證明以下各項即可：
\begin{itemize}
\item[（1）] $f(a \vee b)=f(a) \cup f(b)$ ．
\item[（2）] $f(a \wedge b)=f(a) \cap f(b)$ ．
\item[（3）] $f(\bar{a})=f(a)^c$ ．
\item[（4）] $f$ 為 1－1．
\item[（5）] $f$ 為 onto．
\end{itemize}