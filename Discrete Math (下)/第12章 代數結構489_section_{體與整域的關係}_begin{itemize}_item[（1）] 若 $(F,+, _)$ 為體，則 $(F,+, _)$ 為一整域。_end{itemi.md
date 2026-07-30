第12章 代數結構
489

\section*{體與整域的關係}
\begin{itemize}
\item[（1）] 若 $(F,+, *)$ 為體，則 $(F,+, *)$ 為一整域。
\end{itemize}

【85、90、99台大資工】【94中山資工】
\begin{itemize}
\item[（2）] $F$ 元素個數有限時，若 $(F,+, *)$ 為整域，則 $(F,+, *)$ 為一體。
【90台大資工】【104中山資工】
\end{itemize}

【證明】
\begin{itemize}
\item[（1）] 只需證明 $F$ 中沒有零除元：
設存在 $a \neq 0$ ，且 $a$ 為 $F$ 之一零除元，即存在 $b \neq 0$ ，使得 $a * b=0$ ，
但 $F$ 為體，$\therefore a^{-1} \in F, a^{-1} * a * b=a^{-1} * 0, \therefore b=0 \ldots \ldots$ 得矛盾，故知 $F$ 中沒有零除元。
\item[（2）] 只需證出：$\forall a \in F-\{0\}, a^{-1} \in F$ 即可，
令 $F=\left\{x_1, x_2, \ldots, x_n\right\}$ ，取 $a \in x_i \in F$ ，for some $i$ ．
考慮 $X=\left\{a^* x_1, a^* x_2, \ldots, a^* x_n\right\}$ ，則
\begin{itemize}
\item[（1）] $X$ 中之元素彼此相異，否則設 $a^* x_t=a^* x_s$ ，則利用整域的消去性，可得 $x_s=x_t \ldots$ 矛盾。
\item[（2）] $X=F \ldots \ldots \ldots$ ．因為 $X \subseteq F$ ，且由（1）得 $|X|=n=|F|$ ．
\end{itemize}
\end{itemize}
再由（2）知 $X$ 中之元素等於 $F$ 中之元素，所以存在 $x_k, a * x_k=1$ ，即找到了 $a$ 的右反元素，同理可證 $a$ 的左反元素的存在性，所以 $a$ 的反元素存在，即 $a^{-1} \in F$ ．

Note
\begin{itemize}
\item[（1）] （1）之逆敘述不為真；例如 $(Z,+, *)$ 為一整域，但不為體。
\end{itemize}

【94 中山資工】
\begin{itemize}
\item[（2）] 所以 $\left(Z_n,+, \cdot\right)$ 為體 $\Leftrightarrow\left(Z_n,+{ }_n,{ }_n\right)$ 為整域。
\end{itemize}