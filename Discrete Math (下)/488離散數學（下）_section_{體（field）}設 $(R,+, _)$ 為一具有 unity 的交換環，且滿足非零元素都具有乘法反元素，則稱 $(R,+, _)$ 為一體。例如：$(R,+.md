488
離散數學（下）

\section*{體（field）}

設 $(R,+, *)$ 為一具有 unity 的交換環，且滿足非零元素都具有乘法反元素，
則稱 $(R,+, *)$ 為一體。
例如：
$(R,+, *)$ 與 $(Q,+, *),\left(Z_5,+{ }_5,{ }^*{ }_5\right)$ 都為體，但 $(Z,+, *),\left(Z_6,+{ }_6,{ }^*{ }_6\right)$ 則否。

\section*{基礎類題}

1．Let $(R,+, *)$ be the commutative ring with unity given by the following tables．Is $R$ a field？
解 Yes．
乘法單位元素（unity）為 $u$ ，
$a$ 的乘法反為 $b$ ，
$b$ 的乘法反為 $a$ 。

\begin{tabular}{|l|l|l|l|l|l|l|l|l|l|l|}
\hline ＋ & $z$ & $u$ & $a$ & $b$ & & ＊ & $z$ & $u$ & $a$ & $b$ \\
\hline $z$ & $z$ & $u$ & $a$ & $b$ & & $z$ & $z$ & $z$ & $z$ & $z$ \\
\hline $u$ & $u$ & $z$ & $b$ & $a$ & ； & $u$ & $z$ & $u$ & $a$ & $b$ \\
\hline $a$ & a & $b$ & $z$ & $u$ & & $a$ & $z$ & $a$ & $b$ & $u$ \\
\hline $b$ & $b$ & $a$ & $u$ & $z$ & & $b$ & $z$ & $b$ & $u$ & $a$ \\
\hline
\end{tabular}