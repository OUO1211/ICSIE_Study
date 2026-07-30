526
離散數學（下）

文法（grammar）
一個文法為 $G=(S, N, T, P)$ ，其中，
$N$ 為非終端符號集（set of non－terminals），
用來描述一個句子的中間符號，一般常以大寫符號表達。
$S$ 為開始符號（start symbol），用來指示生成一個句子的開頭，$S \in N$ 。
$T$ 為終端符號集（set of terminals），用來建立語言的符號，一般常以小寫符號表達。$P=\left\{\alpha \rightarrow \beta \mid \alpha, \beta \in(N \bigcup T)^*, \alpha \neq \lambda\right\}$ 為推論法則集（set of productions），
用來指示如何導出一個式子的法則，

生成語言
可由一文法 $G$ 所導出的字串所成的集合稱為 $G$ 所生成的語言，記做 $\boldsymbol{L}(\boldsymbol{G})$ 。

例題 4
有一個語言 $L$ 的文法為 $(T, N, S, P)$ ，其中 Terminal $T=\{a, b, c\}$ ，Non－terminal $N=\{S, A, B\}$ ， Starting symbol $S$ ，Production $P=\{S \rightarrow A B, A \rightarrow a b, A \rightarrow a A b, B \rightarrow c, B \rightarrow B c\}$ 。試問下列的句子 $a a b b, a a b b c, a a a b b b c c c, a b a b c c$ 是否符合 $L$ 語言的文法？試寫出你的推論過程。

解 所得語言 $L(G)=\left\{a^i b^i c^j \mid i, j \geq 1\right\}$ ．
\begin{itemize}
\item[（1）] No．
\item[（2）] Yes．$S \rightarrow A B \rightarrow a A b B \rightarrow a a b b B \rightarrow a a b b c$ ．
\item[（3）] Yes．
$$
S \rightarrow A B \rightarrow a A b B \rightarrow a a A b b B \rightarrow a a a b b b B \rightarrow a a a b b b B c \rightarrow a a a b b b B c c \rightarrow a a a b b b c c c .
$$
\item[（4）] No．
\end{itemize}

例如，下列文法可推得對應的語言，
\begin{itemize}
\item[（1）] $P=\{S \rightarrow 0 S, S \rightarrow \lambda\}, N=\{S\}, T=\{0\}, G=(N, T, P, S), L(G)=\left\{0^i \mid i \geq 0\right\}$ 。
\item[（2）] $P=\{S \rightarrow 0 S 1, S \rightarrow \lambda\}, N=\{S\}, T=\{0,1\}, G=(N, T, P, S), L(G)=\left\{0^i 1^i \mid i \geq 0\right\}$ 。
\item[（3）] $P=\{S \rightarrow 01 S, S \rightarrow 01\}, N=\{S\}, T=\{0,1\}, G=(N, T, P, S), L(G)=\left\{(01)^i \mid i \geq 1\right\}$ 。
\item[（4）] $P=\{S \rightarrow A B, A \rightarrow 0 A, A \rightarrow 0, B \rightarrow B 1, B \rightarrow \lambda\}, N=\{S, A, B\}, T=\{0,1\}, G=(N, T, P$ ． $S) \cdot L(G)=\left\{0^{\prime} 1^{\prime} \mid i \geq 1, j \geq 0\right\}$ ．
\end{itemize}