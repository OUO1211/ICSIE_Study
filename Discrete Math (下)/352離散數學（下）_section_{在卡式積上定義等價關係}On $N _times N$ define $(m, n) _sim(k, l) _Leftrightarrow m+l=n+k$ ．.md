352
離散數學（下）

\section*{在卡式積上定義等價關係}

On $N \times N$ define $(m, n) \sim(k, l) \Leftrightarrow m+l=n+k$ ．
\begin{itemize}
\item[（1）] Let $N$ be the set of all nonnegative integers．Show that $\sim$ is an equivalence relation on $N \times N$ ， and draw a sketch of $N \times N$ that shows the equivalent classes．
\item[（2）] Let $N=\{1,2,3,4,5\}$ ．How many cells are there in the partition of $A$ induced by～？
【90成大資工】【101、104彰師資工】
\end{itemize}

解（1）反身性：$\forall(a, b) \in N \times N, \because a+b=b+a$ ，故 $(a, b) \sim(a, b)$ 。
對稱性：設 $(a, b) \sim(c, d)$ ，即 $a+d=b+c, \therefore c+b=d+a$ ，故 $(c, d) \sim(a, b)$ 。
遞移性：設 $(a, b) \sim(c, d)$ 且 $(c, d) \sim(e, f)$ ，
則由定義知 $a+d=b+c$ 且 $c+f=d+e$ ，$\therefore a+d+c+f=b+c+d+e$ ，
即 $a+f=b+e, \quad \therefore(a, b) \sim(e, f)$ 。
（2）此時，$N \times N=\left\{\begin{array}{lllll}(1,1) & (1,2) & (1,3) & (1,4) & (1,5) \\ (2,1) & (2,2) & (2,3) & (2,4) & (2,5) \\ (3,1) & (3,2) & (3,3) & (3,4) & (3,5) \\ (4,1) & (4,2) & (4,3) & (4,4) & (4,5) \\ (5,1) & (5,2) & (5,3) & (5,4) & (5,5)\end{array}\right\}$ ，
$\because(m, n) \sim(k, l) \Leftrightarrow m+l=n+k$ ，
每一條由左上至右下的對角線即為一等價類，共九種：
即 $A_1=\{(5,1)\}$ ，
$$
\begin{aligned}
& A_2=\{(4,1),(5,2)\}, \\
& A_3=\{(3,1),(4,2),(5,3)\}, \\
& A_4=\{(2,1),(3,2),(4,3),(5,4)\}, \\
& A_5=\{(1,1),(2,2),(3,3),(4,4),(5,5)\}, \\
& A_6=\{(1,2),(2,3),(3,4),(4,5)\}, \\
& A_7=\{(1,3),(2,4),(3,5)\}, \\
& A_8=\{(1,4),(2,5)\}, \\
& A_9=\{(1,5)\}
\end{aligned},
$$