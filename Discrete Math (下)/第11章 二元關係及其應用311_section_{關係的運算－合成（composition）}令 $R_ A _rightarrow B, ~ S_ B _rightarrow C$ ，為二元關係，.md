第11章 二元關係及其應用
311

\section*{關係的運算－合成（composition）}

令 $R: A \rightarrow B, ~ S: B \rightarrow C$ ，為二元關係，則 $R \circ S: A \rightarrow C$ 為 $R, S$ 之合成，
其中 $R \circ S=\{(a, c) \mid$ 存在 $b \in B$ ，使得 $(a, b) \in R$ 且 $(b, c) \in S\}$ 。
例如 ：令 $A=\{1,2,3,4\}, B=\{a, b, c\}, C=\{x, y, z\}$ ，
取 $R=\{(1, a),(1, b),(2, a),(3, a)\}: A \rightarrow B$ ，
取 $S=\{(a, x),(a, y),(c, x)\}: B \rightarrow C$ ，
則 $R \circ S=\{(1, x),(2, x),(3, x),(1, y),(2, y),(3, y)\}: A \rightarrow C$ 。

Note
\begin{itemize}
\item[（1）] 關係的合成一般採用左運算，而可得 $M_{R \circ S}=M_R M_S$ 。本書所使用的合成，也以右運算為主。Rosen 用書則使用右運算，與函數合成也用右運算比較一致。
\item[（2）] 關係的合成滿足結合性：
令 $R: A \rightarrow B, ~ S: B \rightarrow C, ~ T: C \rightarrow D$ ，為三關係，則 $(R \circ S) \circ T=R \circ(S \circ T) \circ$
\item[（3）] 當 $R$ 為 $A$ 上的二元關係，則 $R$ 與 $R$ 的合成 $R \circ R$ ，也記成 $R^2$ 。且可一般化成 $R^{n+1}=R^n \circ R$ ，$n \geq 1$ 。
\end{itemize}