第 6 章 生成函數
591

6－1 一般生成函數
本小節介紹另一種計算組合性問題的工具。在介紹完定義與常用生成函數之後，同學必須能在給定數列後，寫出其對應的一般生成函數的封閉性表達（closed form）；反之，給一生成函數後也能表達出所對應的數列。其次重要的是求某特定項的係數，最後再去了解如何以生成函數的技巧解決問題。

般生成函數（generating function）
给定数列 $a_0, a_1, a_2, \ldots$ ，
則稱函数 $G(x)=a_0+a_1 x+a_2 x^2+\ldots=\sum_{i=0}^{\infty} a_i x^i$ 為此数列所對應的生成函数。
Note
（1）有限項等比級數和公式：
$$
a+a r+a r^2+\ldots+a r^{n-1}=\frac{a\left(1-r^n\right)}{1-r}, r \neq 1
$$
（2）無限項等比級數和公式：
$$
a+a r+a r^2+\ldots=\frac{a}{1-r},|r|<1
$$
（3）常用生成函數：
（1）$\frac{1-x^{n+1}}{1-x}=1+x+x^2+\ldots+x^n=\sum_{i=0}^n x^i, x \neq 1$ 。
（2）$\frac{1}{1-x}=1+x+x^2+x^3+x^4+\ldots=\sum_{i=0}^{\infty} x^i,|x|<1$ 。
（3）分別對（2）左右式的 $x$ 微分後，得 $\frac{1}{(1-x)^2}=1+2 x+3 x^2+4 x^3+\cdots=\sum_{i=1}^{\infty} i x^{i-1}$ 。
（4）$(1+x)^{-n}=\frac{1}{(1+x)^n}=\sum_{r=0}^{\infty}\binom{-n}{r} x^r=\sum_{r=0}^{\infty}(-1)^r\binom{n+r-1}{r} x^r$ 。（此為負二項式定理）
$$
\text { 其中, } \begin{aligned}
\binom{-n}{r} & =\frac{(-n) \cdot(-n-1) \cdot(-n-2) \cdots \cdot(-n-r+1)}{r!} \\
& =(-1)^{\prime} \frac{n \cdot(n+1) \cdot(n+2) \cdots \cdot(n+r-1)}{r!}
\end{aligned}
$$