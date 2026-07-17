368
離散數學（上）

模同餘運算性質：
$\forall a, b, c, n \in Z, n \geq 2$ ，
（1）若 $a \equiv b \bmod n, c \equiv d \bmod n$, 則 $(a+c) \equiv(b+d) \bmod n \circ$

【101師大資工】

（2）若 $a \equiv b \bmod n, c \equiv d \bmod n$, 則 $a c \equiv b d \bmod n$ 。【100北科資工】【101彰師資工】
（3）若 $a \equiv b \bmod n, ~$ 則 $a^2 \equiv b^2 \bmod n$ 。
（4）若 $a c \equiv b c \bmod n$ 且 $\operatorname{gcd}(c, n)=1$ 則 $a \equiv b \bmod n$ 。

【97台北資工】

（5）若 $\operatorname{gcd}(m, n)=1$ ，則 $a \equiv b \bmod m n \Leftrightarrow\left\{\begin{array}{l}a \equiv b \bmod m \\ a \equiv b \bmod n\end{array}\right.$
【證明】
（1）
$$
\begin{align*}
& \because a \equiv b \bmod n, \therefore n \mid a-b \ldots \ldots\left({ }^*\right)  \tag{**}\\
& \because c \equiv d \bmod n, \therefore n \mid c-d \ldots \ldots\left(^{* *}\right)  \tag{*}\\
& \left({ }^*\right)+\left({ }^{* *}\right), \therefore n \mid a+c-(b+d), \therefore(a+c) \equiv(b+d) \bmod n \tag{......}
\end{align*}
$$
（2）由 $(*)$ 可得 $n \mid(a-b) \times c$ $\_\_\_\_$

由 $(* *)$ 可得 $n \mid(c-d) \times b$ $\_\_\_\_$
$$
\begin{equation*}
(i)+(i i), \quad \therefore n \mid a c-b d, \quad \therefore a c \equiv b d \bmod n \text { 。 } \tag{ii}
\end{equation*}
$$
（3）由 $(*)$ 可得 $n \mid(a-b)(a+b)$ ，即 $n \mid a^2-b^2, \therefore a^2 \equiv b^2 \bmod n$ 。
（4）$\because a c \equiv b c \bmod n, \therefore n \mid a c-b c$ ，即 $n \mid(a-b) c$ ，
又 $\operatorname{gcd}(c, n)=1$ 所以 $n \mid a-b, \therefore a \equiv b \bmod n$ 。
（5）$\Rightarrow \because m n|(a-b), \therefore m|(a-b)$ 且 $n \mid(a-b)$ ，所以 $\left\{\begin{array}{l}a \equiv b \bmod m \\ a \equiv b \bmod n\end{array}\right.$ 。
$\Leftarrow \because m \mid(a-b)$ 且 $n \mid(a-b), \therefore a-b$ 為 $m$ 與 $n$ 的公倍數，
但 $\operatorname{gcd}(m, n)=1, \therefore m, n$ 的最小公倍數為 $m n, \therefore m n \mid a-b$ ，即 $a \equiv b \bmod m n$ 。
Note
（1）敘述（3）可推廣成：若 $a \equiv b \bmod n$ ，則 $a^k \equiv b^k \bmod n, \forall k \in N$ 。
（2）敘述（4）中，$c, n$ 一定要互質，否則不見得成立。例如 $10 \equiv 100 \bmod 5$ ，但 $1 \not \equiv 10 \bmod 5$ ，
（3）敘述（5）中，$m, n$ 一定要互質，否則不見得成立，例如 $31 \equiv 1 \bmod 10$ ，但 $31 \not \equiv 1 \bmod 20^{\circ}$
（4）$\left\{\begin{array}{l}a \equiv b \bmod m \\ a \equiv b \bmod n\end{array}\right.$ 有解，若且唯若 $\operatorname{gcd}(m, n) \mid a-b$ 。

【95 台科資工】