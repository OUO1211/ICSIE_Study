第13章 有限狀態機
515

\section*{13－2 語言與文法}

\section*{語言（language）}

設 $\Sigma$ 為一符號集（symbol set），
\begin{itemize}
\item[（1）] 定義集合 $\Sigma^n=\left\{w \mid w=x_1 x_2 \ldots x_n, x_i \in \Sigma\right.$ ，for all $\left.i\right\}$ ，即收集長度為 $n$ 之字串的集合，且記成 $\|w\|=n$ 。
\item[（2）] $\Sigma^0=\{\lambda\}, \lambda$ 稱為空字串（empty string，null string），不包含任何符號的字串。
\item[（3）] $\Sigma^{+}=\bigcup_{i=1}^{\infty} \Sigma^i$ 為任意長度之字串集；$\Sigma^*=\Sigma^{+} \bigcup \Sigma^0=\bigcup_{i=0}^{\infty} \Sigma^i$ 。
\item[（4）] 對 $\Sigma^*$ 之任意子集 $A$ ，稱 $A$ 為佈於 $\Sigma$ 之語言。設 $A, B$ 為佈於 $\Sigma$ 的語言，
\item[（5）] $A B=\{a b \mid a \in A, b \in B\}$ ，稱為 $A, B$ 的串連（concatenation）。
\item[（6）] $A^0=\{\lambda\}, A^1=A, A^{n+1}=\left\{a b \mid a \in A, b \in A^n\right\}, n \in Z^{+}$。
\item[（7）] $A^{+}=\bigcup_{n \in Z^{+}} A^n:$ 稱為 $A$ 的正閉包（positive closure）。
\item[（8）] $A^*=A^{+} \bigcup\{\lambda\}$ ：稱為 $A$ 的 Kleene 閉包（Kleene closure）。
\end{itemize}

例如 ：
設 $\Sigma=\{a, b\}$ ，則 $\Sigma^0=\{\lambda\}, ~ \Sigma^2=\{a a, a b, b a, b b\}$ ，
$$
\Sigma^3=\{a a a, a a b, a b a, a b b, b a a, b a b, b b a, b b b\},
$$
⋯
$$
\begin{aligned}
& \Sigma^{+}=\{a, b, a a, a b, b a, b b, a a a, a a b, a b a, a b b, \ldots\} \\
& \Sigma^*=\{\lambda, a, b, a a, a b, b a, b b, a a a, a a b, a b a, a b b, \ldots\}
\end{aligned}
$$

令 $A=\{a, b, a a\}, B=\{\lambda, b b\}$ ，則
$A B=\{a, b, a a, a b b, b b b, a a b b\}, B A=\{a, b, a a, b b a, b b b, b b a a\}$ ，
$A^0=\{\lambda\}, \quad A^2=\{a a, a b, a a a, b a, b b, b a a, a a b, a a a a\} ; \quad B^0=\{\lambda\}, \quad B^2=\{\lambda, b b, b b b b\} 。$
Note
學字事也被記成 $\varepsilon$ 。