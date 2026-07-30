第12章 代數結構
481

子環（subring）
設 $(R,+, *)$ 為一環，$S \subseteq R$ 滿足 $(S,+, *)$ 亦為一環，則稱 $(S,+, *)$ 為 $(R,+, *)$ 的一個子環。
Note
\begin{itemize}
\item[（1）] 例如：偶整數 $\left(Z_e,+, \times\right)$ 為正整數 $(Z+, \times)$ 之子環；正整數 $(Z,+, \times)$ 為實數 $(R,+, \times)$ 之子環。
\item[（2）] $(S,+, *)$ 為 $(R,+, *)$ 的一個子環時，$R$ 之加法單位元素必為 $S$ 之加法單位元素，但 $R$ 之乘法單位元素未必為 $S$ 之乘法單位元素，$S$ 也未必會有乘法單位元素。
例如，（ $\left.\left\{\left.\left[\begin{array}{ll}a & 0 \\ 0 & 0\end{array}\right] \right\rvert\, a \in R\right\},+, *\right)$ 為實矩陣環 $\left(R^{2 \times 2},+, *\right)$ 的一子環，$\left(R^{2 \times 2},+, *\right)$ 有乘法單位元素 $\left[\begin{array}{ll}1 & 0 \\ 0 & 1\end{array}\right]$ ，但 $\left(\left\{\left.\left[\begin{array}{ll}a & 0 \\ 0 & 0\end{array}\right] \right\rvert\, a \in R\right\},+, *\right)$ 的乘法單位元素是 $\left[\begin{array}{ll}1 & 0 \\ 0 & 0\end{array}\right]$ 。
\item[（3）] 判斷子環的充要條件：設 $(R,+, *)$ 為一環，$S \subseteq R, S \neq \varnothing$ ，則
【97、99台大資工】
\begin{itemize}
\item[（1）] $S$ 為 $R$ 的子環 $\Leftrightarrow \forall a, b \in S, a+b \in S, a b \in S,-a \in S$ ．
\item[（2）] $S$ 為 $R$ 的子環 $\Leftrightarrow \forall a, b \in S, a-b \in S, a b \in S$ ．
\end{itemize}
\item[（3）] 有限集 $S$ 為 $R$ 的子環 $\Leftrightarrow \forall a, b \in S, a+b \in S, a b \in S$ 。
\end{itemize}

【101台大資工】
【證明】
⇒ 由定義明顯得知成立。
⇐ 由定義明顯得知，只需再補上加法單與加法反元素性質即可。任取 $a \in S$ ，
$\because(S,+)$ 的運算具封閉性 $\therefore a, a^2, a^3, \ldots$ 均為 $S$ 中之元素，（ $a^2$ 代表 $a+a$ ），
若 $a=a^2=a^3=\ldots$ ，則 $a$ 為加法單位元素。
否則，$\because|S|<\infty, \therefore$ 存在 $m>n>0$ ，使 $a^m=a^n$ ，得 $a^{m-n}$ 即為加法單位元素，
且 $a$ 的加法反元素為 $a^{m-n-1}$（ $\because a+a^{m-n-1}=a^{m-n}=$ 加法單位元素），故 $-a \in S$ 。得證。
（4）若 $S, T$ 為 $(R,+, *)$ 的子環，則 $S \cap T$ 也是。
【93 嘉義資工】