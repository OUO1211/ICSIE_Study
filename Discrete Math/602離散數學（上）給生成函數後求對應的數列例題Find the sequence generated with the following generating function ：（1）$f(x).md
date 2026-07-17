602
離散數學（上）

給生成函數後求對應的數列
例題
Find the sequence generated with the following generating function ：
（1）$f(x)=\frac{1}{(3-x)}-(3-x)$ ．
【98 中山資エ】【100 成大資工類題】【98 成大資工】
（2）$f(x)=\frac{4}{x^2-8 x+15}$ ．

【103中山資工】

（3）$f(x)=\frac{1-2 x+2 x^2}{1-x-6 x^2}$ ．
【91成大資工】
解（1）$\frac{1}{(3-x)}=\frac{1}{3} \cdot \frac{1}{1-\left(\frac{x}{3}\right)}=\frac{1}{3}\left(1+\frac{x}{3}+\left(\frac{x}{3}\right)^2+\left(\frac{x}{3}\right)^3+\cdots\right)$
$\therefore f(x)=\left(\frac{1}{3}-3\right)+\left(\frac{1}{9}+1\right) x+\frac{1}{27} x^2+\frac{1}{81} x^3+\cdots$
令所對應數列為 $a_n$ ，則 $a_n=\left\{\begin{array}{l}\frac{-8}{3}, n=0 \\ \frac{10}{9}, n=1 \\ \frac{1}{3^{n+1}}, n \geq 2\end{array}\right.$ 。
（2）$\frac{4}{15-8 x+x^2}=\frac{2}{3-x}-\frac{2}{5-x}$ $\_\_\_\_$ （化成部份分式）
$$
=\frac{2}{3} \sum_{i=0}^{\infty}\left(\frac{x}{3}\right)^i-\frac{2}{5} \sum_{i=0}^{\infty}\left(\frac{x}{5}\right)^i=\sum_{i=0}^{\infty} 2\left(3^{-i-1}-5^{-i-1}\right) x^i
$$
$\therefore x^n$ 的係數 $=2\left(3^{-n-1}-5^{-n-1}\right)$ 。
（3）$f(x)=\frac{1-2 x+2 x^2}{1-x-6 x^2}=\frac{-1}{3}+\frac{4-7 x}{3\left(1-x-6 x^2\right)}$
（除法）
$$
\begin{aligned}
& =\frac{-1}{3}+\frac{1}{3}\left(\frac{1}{1-3 x}+\frac{3}{1+2 x}\right) \cdots \cdots \cdots \cdots \cdots \cdots \cdots \cdots \cdots \text { (化成部份分 } \\
& =\frac{-1}{3}+\frac{1}{3}\left(1+3 x+(3 x)^2+\cdots\right)+\left(1-2 x+(2 x)^2-\cdots\right) \\
& =\frac{-1}{3}+\frac{1}{3} \sum_{i=0}^{\infty}(3 x)^i+\sum_{i=0}^{\infty}(-2 x)^i=\frac{-1}{3}+\sum_{i=0}^{\infty}\left(\frac{3^i}{3}+(-2)^i\right) x^i,
\end{aligned}
$$
∴ 所對應的數列為 $a_n=\left\{\begin{array}{ll}\frac{-1}{3}+\frac{1}{3}+(-2)^0 & n=0 \\ 3^{n-1}+(-2)^n & n \geq 1\end{array}\right.$ 。