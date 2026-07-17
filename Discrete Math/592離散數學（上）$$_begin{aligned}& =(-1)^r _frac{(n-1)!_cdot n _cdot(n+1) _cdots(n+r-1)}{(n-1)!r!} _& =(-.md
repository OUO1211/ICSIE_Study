592
離散數學（上）
$$
\begin{aligned}
& =(-1)^r \frac{(n-1)!\cdot n \cdot(n+1) \cdots(n+r-1)}{(n-1)!r!} \\
& =(-1)^r \frac{(n+r-1)!}{r!(n-1)!}=(-1)^r\binom{n+r-1}{r}
\end{aligned}
$$
（5）由（4）可得 $(1-x)^{-n}=\sum_{r=0}^{\infty}\binom{n+r-1}{r} x^r$ 。
（6）若 $f(x)=a_0+a_1 x+a_2 x^2+\cdots$ ，則 $\frac{f(x)}{1-x}=a_0+\left(a_0+a_1\right) x+\left(a_0+a_1+a_2\right) x^2+\cdots$ 。
【102輔大資工】
（7）上述的一般式：若 $A(x)=\sum_{n=0}^{\infty} a_n x^n, B(x)=\sum_{n=0}^{\infty} b_n x^n, C(x)=A(x) B(x)=\sum_{n=0}^{\infty} c_n x^n$ ，則
$$
c_n=a_0 b_n+a_1 b_{n-1}+\ldots+a_{n-1} b_1+a_n b_0=\sum_{i=0}^n a_i b_{n-i} .
$$
（4）導出生成函數的常用方法：
（1）以基本定義列出。
（2）由已知兩式相加（減）。
（3）由已知式乘係數或變數。
（4）由已知式微分後再代入。