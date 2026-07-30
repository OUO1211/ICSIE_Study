194
資料結構（含精選試題）
■■

Data Structure
4． $\mathrm{T}_1 \neq 0, \mathrm{~T}_2 \neq 0$
$$
\begin{array}{ll}
\text { Preorder } & : \mathrm{NT}_1^{\prime}{ }^{\prime} \mathrm{T}_2^{\prime} \\
\text { Postorder } & : \mathrm{T}_1 * \mathrm{~T}_2 * \mathrm{~N}
\end{array}
$$
考慮2及3，若 $\mathrm{T}_2{ }^{\prime}=\mathrm{T}_2{ }^{\prime}$ 且 $\mathrm{T}_2 *-\mathrm{T}_1 *$ ，則無法區分是2或3的狀況，因此，無法決定一個唯一的二元樹。

\section*{5－13 二元樹的計數}
（一）n 個節點所能排出的二元樹種類為 ：
$$
\frac{1}{n+1}\binom{2 n}{n}
$$
證明：設 $\mathrm{b}_{\mathrm{n}}$ 表示含有 n 個節點的相異二元樹的總數，則我們可以取其中的一個節點為樹根，餘分成兩個子樹，分別具有 i 個及 n－i－1 個節點。
$$
\begin{aligned}
\therefore \quad b_n & =b_0 b_{n-1}+b_1 b_{n-2}+\ldots+b_{n-1} b_0, \text { 且 } b_0=1 \\
& =\sum_{i=0}^{n-1} b_i b_{n-i-1} \quad n \geq 1
\end{aligned}
$$
$$
\text { 令 } B(x)=b_0+b_1 x+b_2 x^2+\ldots=\sum_{n=0}^{\infty} b_n x^n
$$
則 $\sum_{n=1}^{\infty} b_n x^n=\sum_{n=1}^{\infty}\left(b_0 b_{n-1}+b_1 b_{n-2}+\ldots+b_{n-1} b_0\right) x^n$
$$
\begin{aligned}
& \rightarrow \quad \sum_{n=1}^{\infty} b_n x^n-b_0=\sum_{n=1}^{\infty}\left(b_0 b_{n-1}+b_1 b_{n-2}+\ldots+b_{n-1} b_0\right) x^n \\
& \rightarrow \quad B(x)-1=x \sum_{n=1}^{\infty}\left(b_0 b_{n-1}+b_1 b_{n-2}+\ldots+b_{n-1} b_0\right) x^{n-1}
\end{aligned}
$$
令 $m=n-1$ 代入上式，得：
$$
\rightarrow \quad B(x)-1=x \sum_{n=0}^{\infty}\left(b_0 b_n+b_1 b_{n-1}+\ldots+b_n b_0\right) x^n
$$
令 $n=m$ 代入上式，得：