第12章 代數結構
479

\section*{$12-4$ 環與體}

環（ring）
若代數系統 $(S,+, *)$ 滿足 ：
\begin{itemize}
\item[（1）] （ $S,+$ ）為一交換群，
\item[（2）] $(S, *)$ 為一半群，
\item[（3）] ＊對＋具有分配性，即 $\forall a, b, c \in S,\left\{\begin{array}{l}a *(b+c)=a * b+a * c \\ (b+c)^* a=b^* a+c * a\end{array}\right.$ ，
\end{itemize}

則稱（ $S,+, *$ ）為一個環。
又若（ $S, *$ ）具交換性，則稱（ $S,+, *$ ）為交換環（commutative ring）。
Note
\begin{itemize}
\item[（1）] 此時，$(S,+)$ 中之單位元素習慣稱為加法單位元素（additive identity），記做 $\underline{0}$（zero）；$a$ 之加法反元素稱為負元素（negative）記做 $\underline{a}$ 。
\item[（2）] $(S, *)$ 中，若有單位元素，習慣稱為乘法單位元素（multiple identity），記做 1 （unity）；$a$ 之乘法反元素若存在（則稱 $a$ 為一個 unit），並稱 $a$ 的乘法反為 inverse，記做 $a^{-1}$ 。
\item[（3）] $(Z,+, \times) 、(R,+, \times) 、\left(Z_n,+{ }_n,{ }_n\right)$ 均為交換環，且均有乘法單位元素。
\item[（4）] $(P(A), \oplus, \cap)$ 為交換環，$P(A)$ 為某給定集合 $A$ 的幂集合。
\end{itemize}

【91暨南資工】
\begin{itemize}
\item[（5）] 矩陣環：（ $\left.R^{n \times n},+, \cdot\right)$ 為一非交換環。
\item[（6）] 多項式環：（ $R[x],+, \times$ ），其中 $R[x]=\{f(x) \mid f(x)$ 為佈於 $R$ 之多項式\}, 且 $(R,+, *)$ 為某環。【96 雲科資工】
\item[（7）] 環的運算性質：$(S,+, *)$ 為一環，則
\begin{itemize}
\item[（1）] $\forall a \in S, a * 0=0=0 * a$ 。
\item[（2）] If $a$ is a unit in ring $S$ ，then $-a$ is also a unit in $S$ ．
【87 台科資工】
\end{itemize}
\end{itemize}

【證明】
\begin{itemize}
\begin{itemize}
\item[（1）] $\because a^* 0+0=a^* 0=a^*(0+0)=a^* 0+a^* 0, ~ \therefore a^* 0=0$ 。
\item[（2）] $\because a$ 有乘法反元素，設為 $b$ ，滿足 $a * b=b * a=1$ ，則 $(-a) *(-b)=(-b) *(-a)=a * b =1, \therefore-b$ 為 $-a$ 的乘法反元素，$-a$ 是一個 unit。
\end{itemize}
\end{itemize}