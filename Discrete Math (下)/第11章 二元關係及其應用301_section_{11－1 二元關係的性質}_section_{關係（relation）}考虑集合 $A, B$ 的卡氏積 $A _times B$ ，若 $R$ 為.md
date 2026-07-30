第11章 二元關係及其應用
301

\section*{11－1 二元關係的性質}

\section*{關係（relation）}

考虑集合 $A, B$ 的卡氏積 $A \times B$ ，
若 $R$ 為 $A \times B$ 的一子集，則稱 $R$ 為一種 $A$ 到 $B$ 的二元關係，也記做 $R: A \rightarrow B$ ，此時，若 $(a, b) \in R$ ，則稱 $a$ 與 $b$ 有 $R$ 關係，或記做 $a R b$ 。

Note
\begin{itemize}
\item[（1）] 本書討論的二元關係，除非特別指明，否則都是 $A 、 B$ 為非空集合。
\item[（2）] 當 $A=B$ 時，稱 $R \subseteq A \times A=A^2$ 為 $A$ 上之一二元關係。
\end{itemize}

【100 中山電機】
\begin{itemize}
\item[（2）] 若 $R=\varnothing$ ，則稱 $R$ 為 $A$ 到 $B$ 上的空關係。
\item[（3）] 若 $R=A \times B$ ，則稱 $R$ 為 $A$ 到 $B$ 上的全關係。
\item[（4）] 一般表示關係的方法，除了用集合表達外，還有以下方式：
設集合 $A=\left\{a_1, a_2, \ldots, a_m\right\}, B=\left\{b_1, b_2, \ldots, b_n\right\}, R$ 為 $A \rightarrow B$ 之一關係，
\begin{itemize}
\item[（1）] $R$ 之關係矩陣 $M_R=\left[m_{i j}\right]_{m \times n}$ ，定義為 $m_{i j}=\left\{\begin{array}{ll}1 & \text { if }\left(a_i, b_j\right) \in R \\ 0 & \text { if }\left(a_i, b_j\right) \notin R\end{array}\right.$ 。
\item[（2）] $R$ 之關係圖形為一有向圖 ：$G=(V, E)$ ，點集合 $V=\left\{a_1, a_2, \ldots, a_m, b_1, b_2, \ldots, b_n\right\}$ ，且 $a_i$ 有一指向 $b_j$ 的邊 $\Leftrightarrow\left(a_i, b_j\right) \in R$ 。
\end{itemize}
\end{itemize}

例如：
令 $A=\{1,2,3,4\}, B=\{a, b, c\}$ ，取 $R=\{(1, a),(1, b),(2, a),(3, a)\}$