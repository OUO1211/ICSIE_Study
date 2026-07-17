第 5 章 組合計數
545

二項式定理應用（5）－進階性質
請證明下列等式：
（1）$\left(\sum_{k=0}^n\binom{n}{k}\right)^2=\sum_{k=0}^{2 n}\binom{2 n}{k}$ ．
【89 交大應数】
（2）$\binom{n}{0}+\frac{1}{2}\binom{n}{1}+\frac{1}{3}\binom{n}{2}+\ldots+\frac{1}{n+1}\binom{n}{n}=\frac{2^{n+1}-1}{n+1}$ ．
【 87 交大底数】

【證明】
（1）$\because\left((x+y)^n\right)^2=(x+y)^{2 n}$ ，
$$
\begin{aligned}
& \therefore\left(\binom{n}{0} x^0 y^n+\binom{n}{1} x^1 y^{n-1}+\ldots+\binom{n}{n} x^n y^0\right)^2=\binom{2 n}{0} x^0 y^{2 n}+\binom{2 n}{1} x^1 y^{2 n-1}+\ldots+\binom{2 n}{2 n} x^{2 n} y^0 \\
& x=y=1 \text { 代入, 得 }\left(\binom{n}{0}+\binom{n}{1}+\ldots+\binom{n}{n}\right)^2=\left(\binom{2 n}{0}+\binom{2 n}{1}+\ldots+\binom{2 n}{2 n}\right) 。
\end{aligned}
$$

另證 ：
因為 $\binom{t}{0}+\binom{t}{1}+\ldots+\binom{t}{n}=2^t, \therefore$ 左式 $=\left(2^n\right)^2=2^{2 n}$ ，右式 $=2^{2 n}$ ，故等式成立。
（2）左式 $=\frac{1}{n+1}\left(\frac{n+1}{1}\binom{n}{0}+\frac{n+1}{2}\binom{n}{1}+\frac{n+1}{3}\binom{n}{2}+\ldots+\frac{n+1}{n+1}\binom{n}{n}\right)$
$$
=\frac{1}{n+1}\left(\binom{n+1}{1}+\binom{n+1}{2}+\binom{n+1}{3}+\ldots+\binom{n+1}{n+1}\right)=\frac{2^{n+1}-1}{n+1}=\text { 右式。 }
$$