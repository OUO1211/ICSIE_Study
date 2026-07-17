第 6 章 生成函數
611

列出生成函數、並應用在求整數解個數上
例題
Find the generating function and the number of integer solutions for each equation ：
（1）$x_1+x_2+x_3+x_4=19$ ，where $-5 \leq x_i \leq 10$ for all $1 \leq i \leq 4$ ．
【84 中正資工類題】【95 成大資工】【105、99 暨南資工】
（2）$x_1+x_2+x_3+x_4=20$ ，where $-3 \leq x_1,-3 \leq x_2,-5 \leq x_3 \leq 5,0 \leq x_4$ ．
【102、110 中山資工類題】【102 中山電機】
解（1）考慮生成函數 $G(x)=\left(x^{-5}+x^{-4}+\cdots+x^9+x^{10}\right)^4$ ，則 $x^{19}$ 的係數即為所求，
$$
\begin{aligned}
\because G(x) & =\left(\frac{x^{-5}\left(1-x^{16}\right)}{1-x}\right)^4=x^{-20}\left(1-x^{16}\right)^4(1-x)^{-4} \\
& =x^{-20} \sum_{i=0}^4\binom{4}{i}\left(-x^{16}\right)^i \sum_{j=0}^{\infty}\binom{-4}{j}(-x)^j
\end{aligned}
$$

分別取 $i=0, j=39 ; i=1, j=23 ; i=2, j=7$ ，得 $x^{19}$ 係數：
$$
\begin{aligned}
& \binom{4}{0}(-1)^0\binom{-4}{39}(-1)^{39}+\binom{4}{1}(-1)^1\binom{-4}{23}(-1)^{23}+\binom{4}{2}(-1)^2\binom{-4}{7}(-1)^7, \\
& =\binom{4}{0}\binom{4+39-1}{39}+\binom{4}{1}(-1)^1\binom{4+23-1}{23}+\binom{4}{2}(-1)^2\binom{4+7-1}{7}, \\
& =\binom{42}{39}-\binom{4}{1}\binom{26}{23}+\binom{4}{2}\binom{10}{7} .
\end{aligned}
$$
（2）考慮 $G(x)=\left(x^{-3}+x^{-2}+\cdots\right)\left(x^{-3}+x^{-2}+\cdots\right)\left(x^{-5}+\cdots+x^5\right)\left(1+x+x^2+\cdots\right)$
$G(x)=x^{-11}\left(1+x+x^2+\cdots\right)^3\left(1+x+x^2+\cdots+x^{10}\right)=x^{-11}(1-x)^{-3}\left(\frac{1-x^{11}}{1-x}\right)$
$G(x)$ 中之 $x^{20}$ 係數即為所求，仿（1）的計算過程可得 $\binom{34}{3}-\binom{23}{3}$ 。

例題 6
（10\％）Let $h_n$ denotes the number of combinations of $n$ gems consisting of an odd numbers of rubies，an even number of sapphires，at most one topaz，and any number of emeralds．（Gems of the same kind are the same．）Find the generating function（in a compact form，not a power series） and an explicit formula（in terms of $n$ ）of $h_n$ ．

【104 交大應数】