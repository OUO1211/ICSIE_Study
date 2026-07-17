第 5 章 組合計數
579

題型五

由多項式定理：$\left(x_1+x_2+\ldots+x_t\right)^n=\sum_{n_1+\ldots+n_t=n} \frac{n!}{n_{1}!n_{2}!\ldots n_{t}!} x_1^{n_1} x_2^{n_2} \ldots x_t^{n_t}$ 知，
展開後的項数即為 $n_1+\ldots+n_t=n \quad$ 之非負整数解個数。

例題 11
Please find the number of the terms in the expansion of each expression．
（1）$[(x / 2)+y-3 z]^5$ ．
（2）$\left(1+2+\ldots+100+x_1+x_2+\ldots+x_n\right)^k$ ．
（3）$(x+y+z)^{10}(w+x+y+z)^2$ ．
解（1）$\binom{5+2}{2}$ ．
（2）相當於 $\left(x_0+x_1+x_2+\ldots+x_n\right)^k, x_0=5050$ ，共 $\binom{n+k}{n}$ 項。
（3）原式 $=(x+y+z)^{10} \cdot\left(w^2+2 w(x+y+z)+(x+y+z)^2\right)$
$$
=w^2(x+y+z)^{10}+2 w(x+y+z)^{11}+(x+y+z)^{12}
$$

而此三式展開所得項各不相同，故共有 $\binom{12}{2}+\binom{13}{2}+\binom{14}{2}$ 。

基礎類題
1．How many distinct terms arise in the expansion in
（1）$(a+b+c+d)^5$ ．
【99政大資科】【97師大資工類題】【98台大電機】
（2）$(a+3 b-2 c+1)^6$ ．
【98成大資工】
（3）$(5 a+8 b)^{16}$ ．
【102 交大資エ】
解
（1）$\binom{5+3}{3}$ ．
（2）$\binom{6+3}{3}$ ．
（3）$\binom{16+1}{1}$ ．