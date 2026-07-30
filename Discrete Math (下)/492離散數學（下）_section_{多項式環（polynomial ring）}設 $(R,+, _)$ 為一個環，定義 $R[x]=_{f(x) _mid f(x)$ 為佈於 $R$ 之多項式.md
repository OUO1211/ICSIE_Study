492
離散數學（下）

\section*{多項式環（polynomial ring）}

設 $(R,+, *)$ 為一個環，定義 $R[x]=\{f(x) \mid f(x)$ 為佈於 $R$ 之多項式 $\}, ~ R[x]$ 上的加法及乘法運算為一般多項式的運算，則稱 $(R[x],+, *)$ 為多項式環。

Note
\begin{itemize}
\item[（1）] $(R,+, *)$ 為一交換環 $\Leftrightarrow(R[x],+, *)$ 為一交換環。
\item[（2）] $(R,+, *)$ 具 unity $1 \Leftrightarrow(R[x],+, *)$ 具 unity 1 。
\item[（3）] $(R,+, *)$ 為體，則 $(R[x],+, *)$ 不一定為體。
\item[（4）] 可約（reducible）與不可約（irreducible）：
若存在佈於體 $F$ 的多項式 $g(x), h(x)$ ，使得 $f(x)=g(x) h(x)$ ，其中 $g(x)$ 與 $h(x)$ 次數均至少一次，則稱 $f(x)$ 為一可約多項式，否則稱為不可約多項式。
\item[（5）] 例如：$x^2+1$ 佈於實數 $R$ 時不可約，但佈於複數 $C$ 時可約 $\left(\because x^2+1=(x+i)(x-i)\right)$ ．
\item[（6）] 設 $f(x) \in F[x]$ ，其中 $F$ 為一個體。
\begin{itemize}
\item[（1）] 若 $\operatorname{deg}(f)=1$ ，則 $f(x)$ 為不可約的。
\item[（2）] 若 $\operatorname{deg}(f)=2$ 或3，則 $f(x)$ 為可約的 ⇔ $f(x)$ 在 $F$ 中有一根。
\end{itemize}
\item[（7）] 若 $f(x), g(x)$ 互質，則不存在 $a$ 使 $f(a)=0$ 與 $g(a)=0$ 。
\end{itemize}

【92 暨南資工】