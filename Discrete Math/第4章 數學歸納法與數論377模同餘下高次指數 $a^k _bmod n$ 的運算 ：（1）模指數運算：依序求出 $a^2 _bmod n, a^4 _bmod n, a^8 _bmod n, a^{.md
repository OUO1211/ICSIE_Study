第4章 數學歸納法與數論
377

模同餘下高次指數 $a^k \bmod n$ 的運算 ：
（1）模指數運算：
依序求出 $a^2 \bmod n, a^4 \bmod n, a^8 \bmod n, a^{16} \bmod n, \cdots$ ，再把 $a^k$ 用 $a^2, a^4, a^8, a^{16}, \cdots$ 表示，而將對應的結果相乘。
例如，欲求 $7^{11} \bmod 5$ ：
$$
\begin{aligned}
& 7 \equiv 2 \bmod 5 \\
& 7^2 \equiv 2^2 \equiv 4 \bmod 5 \\
& 7^4 \equiv 4^2 \equiv 16 \equiv 1 \bmod 5 \\
& 7^8 \equiv 1^2 \equiv 1 \bmod 5 \\
& \therefore 7^{11} \bmod 5 \equiv 7 \cdot 7^2 \cdot 7^8 \bmod 5 \equiv 2 \cdot 4 \cdot 1 \equiv 8 \equiv 3 \bmod 5
\end{aligned}
$$
（2）尤拉定理（Euler Theorem）：
$m, n$ 為整數，$n>0$ ，且 $m, n$ 互質，則 $m^{\phi(n)} \equiv 1 \bmod n$ 。
（在第 12 章代數可給出證明）

【108中山資エ】

例如， $7^6 \equiv 1 \bmod 9$ 。
也因此可得 $7^5 \equiv(-2)^5 \equiv-32 \equiv 4 \bmod 9$ ，故 7 的乘法反元素為 4 。
（3）費瑪小定理（Fermat＇s Little Theorem）
【97宜蘭資エ】【97台北資エ】
$m$ 為整數，$p$ 為質數，且 $m, p$ 互質，則 $m^{p-1} \equiv 1 \bmod p$ 。
Note
可視為尤拉定理的一個特例，也可先證明下列性質而得證：
$m$ 為整數，且 $p$ 為質數，則 $m^p \equiv m \bmod p$ 。
【103 中央資エ】【88 清大資エ】【108 中山資エ】
【證明】
（1）$m$ 為正整數時，
由二項式定理 ：
$(x+y)^p=\binom{p}{0} x^0 y^p+\binom{p}{1} x^1 y^{p-1}+\ldots+\binom{p}{p} x^p y^0$ ，與質數 $p \|\binom{ p}{i}, 1 \leq i \leq p-1$ ，
可得 $(x+y)^p \equiv\binom{p}{0} y^p+\binom{p}{p} x^p \equiv x^p+y^p(\bmod p)$ ，
令 $x=1, ~ y=1$ 得 $2^p \equiv(1+1)^p \equiv 1^p+1^p \equiv 2(\bmod p)$ ，
令 $x=2$ ，$y=1$ 得 $3^p \equiv(2+1)^p \equiv 2^p+1^p \equiv 2+1 \equiv 3(\bmod p)$ ，
⋯ ，故得 $m^p \equiv m(\bmod p), ~ \forall m \in Z^{+}$。