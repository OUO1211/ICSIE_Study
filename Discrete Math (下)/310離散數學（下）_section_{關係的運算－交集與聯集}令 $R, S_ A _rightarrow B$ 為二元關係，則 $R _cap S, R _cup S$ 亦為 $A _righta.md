310
離散數學（下）

\section*{關係的運算－交集與聯集}

令 $R, S: A \rightarrow B$ 為二元關係，
則 $R \cap S, R \cup S$ 亦為 $A \rightarrow B$ 的二元關係，其中，
$$
\begin{aligned}
& R \cap S=\{(a, b) \mid(a, b) \in R \text { and }(a, b) \in S\}, \\
& R \cup S=\{(a, b) \mid(a, b) \in R \text { or }(a, b) \in S\} .
\end{aligned}
$$

例如 ：
令 $A=\{1,2,3,4\}, B=\{a, b, c\}$ ，
取 $R=\{(1, a),(1, b),(2, a),(3, a)\}: A \rightarrow B$ ；取 $S=\{(1, a),(1, c)\}: A \rightarrow B$ ，
則 $R \cap S=\{(1, a)\}$ ；
$$
R \bigcup S=\{(1, a),(1, b),(1, c),(2, a),(3, a)\} \circ
$$

Note
\begin{itemize}
\item[（1）] $\overline{R \bigcap S}=\bar{R} \bigcup \bar{S} ; \overline{R \bigcup S}=\bar{R} \cap \bar{S}$ ．（De Morgan＇s law 的應用定理）
\item[（2）] $(R \cap S)^{-1}=R^{-1} \cap S^{-1} ;(R \cup S)^{-1}=R^{-1} \cup S^{-1}$ ．
\end{itemize}