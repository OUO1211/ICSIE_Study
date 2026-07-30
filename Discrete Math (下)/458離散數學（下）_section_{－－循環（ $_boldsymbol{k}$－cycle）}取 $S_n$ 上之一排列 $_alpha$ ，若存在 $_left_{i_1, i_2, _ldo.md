458
離散數學（下）

\section*{－－循環（ $\boldsymbol{k}$－cycle）}

取 $S_n$ 上之一排列 $\alpha$ ，
若存在 $\left\{i_1, i_2, \ldots, i_k\right\} \subseteq\{1,2, \ldots, n\}$ ，使得 $\alpha\left(i_1\right)=i_2, \alpha\left(i_2\right)=i_3, \ldots, \alpha\left(i_k\right)=i_1$ ，
且 $\alpha(i)=i, \forall i \in\{1,2, \ldots, n\}-\left\{i_1, i_2, \ldots, i_k\right\}$ ，
則稱 $\alpha$ 為一種 $k$－循環（ $k$－cycle），記作 $\alpha=\left(\begin{array}{llll}i_1 & i_2 & \ldots & i_k\end{array}\right)$ 。
例如，
$$
\begin{aligned}
& p=\left(\begin{array}{llllll}
1 & 2 & 3 & 4 & 5 & 6 \\
4 & 3 & 5 & 2 & 1 & 6
\end{array}\right)=\left(\begin{array}{lllll}
1 & 4 & 2 & 3 & 5
\end{array}\right), \\
& q=\left(\begin{array}{lllllll}
1 & 2 & 3 & 4 & 5 & 6 \\
3 & 1 & 2 & 5 & 4 & 6
\end{array}\right)=\left(\begin{array}{lll}
1 & 3 & 2
\end{array}\right)\left(\begin{array}{ll}
4 & 5
\end{array}\right)(6)
\end{aligned}
$$

Note
\begin{itemize}
\item[（1）] 任何一個排列 $\alpha \in S_n-\{e\}, \alpha$ 可表成若干個互斥循環的乘積（互斥指的是任何一個數最多出現在一個循環中），此時的合成具交換性。
\item[（2）] 成為 cycle 後，表達法不唯一：$(a b c d)=(b c d a)=(c d a b) 。$
\item[（3）] 當 $k=2$ 時，2－循環又稱作換位或對調（transposition）。
\item[（4）] 任何循環（或排列）皆可表成若干個換位的乘積。
例如 ：
$$
\begin{aligned}
& (a b c d)=(a d) \circ(a c) \circ(a b)=(a b) \circ(b c) \circ(c d) . \\
& \left(\begin{array}{llllll}
1 & 2 & 3 & 4 & 5 & 6 \\
2 & 4 & 3 & 1 & 6 & 5
\end{array}\right)=(124) \circ(3) \circ(56)=(124) \circ(56)=(14) \circ(12) \circ(56) . \\
& \left(\begin{array}{llllllll}
1 & 2 & 3 & 4 & 5 & 6 & 7 & 8 \\
7 & 8 & 6 & 3 & 2 & 4 & 5 & 1
\end{array}\right)=(17528) \circ(364)=(17) \circ(75) \circ(52) \circ(28) \circ(36) \circ(64) .
\end{aligned}
$$
\item[（5）] 若任一排列 $\alpha \in S_n$ 表達成換位的個數為偶數時，稱 $\alpha$ 為一個偶排列（even permutation），否則為奇排列（odd permutation）。
\end{itemize}