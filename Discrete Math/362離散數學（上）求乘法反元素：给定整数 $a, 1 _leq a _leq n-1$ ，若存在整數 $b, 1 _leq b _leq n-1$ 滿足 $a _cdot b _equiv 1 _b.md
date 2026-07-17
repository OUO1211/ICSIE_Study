362
離散數學（上）

求乘法反元素：
给定整数 $a, 1 \leq a \leq n-1$ ，
若存在整數 $b, 1 \leq b \leq n-1$ 滿足 $a \cdot b \equiv 1 \bmod n$ ，
則稱 $b$ 為 $a$ 在模 $n$ 下的乘法反元素，記做 $b=a^{-1}$ 。
例如：
$\bmod 10$ 時， 3 與 7 互為彼此的乘法反元素； 9 的乘法反元素是 9 。
$\bmod 9$ 時， $2^{-1}=5, ~ 4^{-1}=7, ~ 8^{-1}=8$ 。

Note
（1）有時也直接稱 $a$ 的乘法反元素為 $a$ 的反元素（inverse）。
（2）若 $a$ 有乘法反元素，則稱 $a$ 為一unit。
（3） $1 \leq a \leq n, a$ 有乘法反元素 $\Leftrightarrow a$ 與 $n$ 互質。

【92台科資工】

【證明】
$a$ 有乘法反 ⇔ 存在 $b, a \cdot b \equiv 1 \bmod n$
$$
\begin{aligned}
& \Leftrightarrow \text { 存在 } b, n \mid 1-a b \\
& \Leftrightarrow \text { 存在 } b, k, \text { 使 } a b+n k=1 \\
& \Leftrightarrow \operatorname{gcd}(a, n)=1 \text { 。 }
\end{aligned}
$$
（4）$Z_n=\{0,1, \ldots, n-1\}$ 中有 $\phi(n)$ 個元素有乘法反元素。【94 台大資工】【99 中山資工】
（5）給定整數 $a, 0 \leq a \leq n-1$ ，若存在整數 $b, 0 \leq b \leq n-1$ 滿足 $(a+b) \equiv 0 \bmod n$ ，則稱 $b$ 為 $a$ 在模 $n$ 下的加法反元素。
例如： $\bmod 10$ 時， 3 與 7 互為彼此的加法反元素； 2 與 8 互為彼此的加法反元素。