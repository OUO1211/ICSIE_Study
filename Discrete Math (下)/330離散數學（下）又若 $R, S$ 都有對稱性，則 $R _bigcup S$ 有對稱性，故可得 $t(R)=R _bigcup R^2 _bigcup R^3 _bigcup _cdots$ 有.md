330
離散數學（下）

又若 $R, S$ 都有對稱性，則 $R \bigcup S$ 有對稱性，故可得 $t(R)=R \bigcup R^2 \bigcup R^3 \bigcup \cdots$ 有對稱性。
\begin{itemize}
\item[（8）] 考慮集合 $A$ 上的關係 $R$ 與 $S$ ，則 $s(R \bigcup S)=s(R) \bigcup s(S)$ 。
【92 台科資工】
\end{itemize}

【證明】
$$
s(R \bigcup S)=(R \bigcup S) \bigcup(R \bigcup S)^{-1}=(R \bigcup S) \bigcup\left(R^{-1} \bigcup S^{-1}\right)=\left(R \bigcup R^{-1}\right) \bigcup\left(S \bigcup S^{-1}\right)=s(R) \bigcup s(S) .
$$