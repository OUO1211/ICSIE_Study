第11章 二元關係及其應用
421

\section*{布林表示式（Boolean expression）}

設 $(B, \vee, \wedge, I, O,-)$ 為布林代數，一個布林表示式 $E\left(x_1, x_2, \ldots, x_n\right)$ 可遞迴的定義為：
\begin{itemize}
\item[（1）] $B$ 中任何元素皆為布林表示式。
\item[（2）] 任何變數 $x_1, x_2, \ldots, x_n$ 皆為布林表示式。
\item[（3）] 若 $E_1, E_2$ 為布林表示式，則 $\overline{E_1}, E_1 \vee E_2, E_1 \wedge E_2$ 亦為布林表示式。
\end{itemize}

\section*{極小項與極大項（mini－term and max－term），分離正規型與連接正規型（Disjunctive normal form and Conjunctive normal form）}

設 $E\left(x_1, x_2, \ldots, x_n\right)$ 為具 $n$ 個變數 $x_1, x_2, \ldots, x_n$ 的布林表示式，
\begin{itemize}
\item[（1）] 稱 $E\left(x_1, x_2, \ldots, x_n\right)=\tilde{x}_1 \wedge \tilde{x}_2 \wedge \ldots \wedge \tilde{x}_n$ 為極小項，其中 $\tilde{x}_i \in\left\{x_i, \overline{x_i}\right\}$ 。
\item[（2）] 稱 $E\left(x_1, x_2, \ldots, x_n\right)=\tilde{x}_1 \vee \tilde{x}_2 \vee \ldots \vee \tilde{x}_n$ 為極大項，其中 $\tilde{x}_i \in\left\{x_i, \overline{x_i}\right\}$ 。
\item[（3）] 若 $E\left(x_1, x_2, \ldots, x_n\right)$ 為若干個極小項之和（join），則稱其為一種分離正規型；
\item[（4）] 若 $E\left(x_1, x_2, \ldots, x_n\right)$ 為若干個極大項之積（meet），則稱其為一種連接正規型。
\end{itemize}

例如 ：
\begin{itemize}
\item[（1）] $E_1\left(x_1, x_2, x_3\right)=x_1 \overline{x_2} x_3+\overline{x_1} \overline{x_2} x_3+x_1 \overline{x_2} \overline{x_3}+x_1 x_2 x_3$ 為一分離型。
\item[（2）] $E_2\left(x_1, x_2, x_3\right)=\left(x_1+x_2+x_3\right)\left(\overline{x_1}+x_2+x_3\right)\left(x_1+\overline{x_2}+\overline{x_3}\right)$ 為一連接型。
\item[（3）] $E_3\left(x_1, x_2, x_3\right)=\bar{x}_1 x_2+x_1 \bar{x}_2$ 不為分離型，亦不為連接型。
\end{itemize}

Note
\begin{itemize}
\item[（1）] 有時會以＋表示 $\vee$ ；以 • 表示＾。
\item[（2）] 在 $n$ 個變數的布林表示式，極小項有 $2^n$ 種，極大項也有 $2^n$ 種。
\item[（3）] 分離型又稱 sum of product $(S O P)$ ；連接型又稱 product of sum（POS），都是標準型，且每一種分離型都可唯一轉換成一種連接型。
\item[（4）] $n$ 個變數的標準布林表示式有 $2^{2^n}$ 種。
\item[（5）] 任一布林表示式均可化成一標準的布林表示式（ $C N F$ 或 $D N F$ ）。以下介紹兩種化為布林表示式的方法：例題1與例題2使用代數運算；例題3使用真值表。
\end{itemize}