第4章 數學歸納法與數論
313

先觀察出規律性後，再以歸納法證明
例題 4
Show that $1(1!)+2(2!)+\ldots+n(n!)$ can be expressed as difference of two factorials for $n=1,2,3, \ldots$（we assume $0!=1$ ）．【 85 中央資工】【 108 師大資工】【 108 高雄資エ】
解 證明原式可表成 $(n+1)!-1$ ！如下：
$n=1$ 時，左式等於 $1 \cdot 1!=1$ ，右式等於 $2!-1=1!$ ，原式成立。
設 $n=k \geq 1$ 時，原式成立。
則 $n=k+1$ 時，
左式 $=1 \cdot 1!+2 \cdot 2!+\ldots+k \cdot k!+(k+1) \cdot(k+1)!=(k+1)!-1+(k+1) \cdot(k+1)!$
$$
=(k+2) \cdot(k+1)!-1!=(k+2)!-1!=\text { 右式, }
$$

所以由數學歸納法知原式成立。

基礎類題
1．（10\％）Consider the homogeneous difference equation with non－constant coefficients $x_n=n x_{n-1}$ ， $n=1,2,3, \ldots$ ，with initial conditions $x_0=1$ ．Find a general solution to $x_n$ ．（Hint：you could calculate enough terms to see a pattern，and confirm your guess using mathematical induction．）

【103成大工科】
解
$$
\begin{aligned}
& x_1=1 x_0=1! \\
& x_2=2 x_1=2 \times 1=2! \\
& x_3=3 x_2=3 \times 2!=3!
\end{aligned}
$$
$\cdots \quad \therefore$ 猜測 $x_n=n!$ ，其中 $n \geq 0$ ，
$n=0$ 時，$x_0=1=0!$ ，猜測成立，
設 $n=k \geq 0$ 時，$x_k=k!$ ，
則 $n=k+1$ 時，$\because x_{k+1}=(k+1) x_k=(k+1) \times k!=(k+1)!$ ，故由歸納法知猜測成立。
2．Define $s_n=\frac{1}{2!}+\frac{2}{3!}+\frac{3}{4!}+\ldots+\frac{n}{(n+1)!}$ ，where $n$ is a positive integer．
（1）Compute $s_1, s_2, s_3, s_4$ ．
（2）On the basis of your result in part（1），conjecture a formula for the sum of the terms in $s_n$ ．

【86 中興資科】【93 北科資工】