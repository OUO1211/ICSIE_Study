686
離散數學（上）

求解遞迴關係式－使用生成函數

使用生成函數法解遞迴關係，步驟如下：
Step 1：變換 index 使成為 $c_n a_n+c_{n-1} a_{n-1}+\ldots+c_{n-k} a_{n-k}=\ldots$
Step 2：各項乘以 $x^n$ ，再加總取 $\sum_{n=k}^{\infty}$ 。
Step 3 ：引入 $A(x)=a_0+a_1 x+a_2 x^2+\ldots=\sum_{i=0}^{\infty} a_i x^i$.
Step 4 ：代入初值條件，$a_0, a_1, \ldots$
Step 5：整理 $A(x)$ ，則 $x^n$ 之係數即為 $a_n$ 的一般式。
（還可以用特徵多項式法對答案）

例題 13
（5\％）To solve the recurrence relation $a_{n+2}=a_{n+1}+2 a_n+(-1)^n, n \geq 0, a_0=1, a_1=1$ ．What will be the corresponding generating function $f(x)$ ？

【100、101 中央資工】
解 原式等於 $a_n-a_{n-1}-2 a_{n-2}=(-1)^{n-2}$ ，
$$
\begin{aligned}
& \therefore \sum_{n=2}^{\infty} a_n x^n-\sum_{n=2}^{\infty} a_{n-1} x^n-2 \sum_{n=2}^{\infty} a_{n-2} x^n=\sum_{n=2}^{\infty}(-x)^n, \\
& \text { 令 } f(x)=\sum_{n=0}^{\infty} a_n x^n,
\end{aligned}
$$

則原式成為 $\left(f(x)-a_0-a_1 x\right)-x \sum_{n=2}^{\infty} a_{n-1} x^{n-1}-2 x^2 \sum_{n=2}^{\infty} a_{n-2} x^{n-2}=\frac{x^2}{1+x}$ ，
變數變換 ：$(f(x)-1-x)-x \sum_{i=1}^{\infty} a_i x^i-2 x^2 \sum_{i=0}^{\infty} a_i x^i=\frac{x^2}{1+x}$ ，
$$
f(x)-a_0-a_1 x-x\left(f(x)-a_0\right)-2 x^2 f(x)=\frac{x^2}{1+x}
$$

代入初值條件：$f(x)-1-x-x(f(x)-1)-2 x^2 f(x)=\frac{x^2}{1+x}$ ，
整理得 $\left(1-x-2 x^2\right) f(x)=\frac{x^2}{1+x}+1=\frac{x^2+x+1}{1+x}$ ，
$$
\therefore f(x)=\frac{1+x+x^2}{(1+x)\left(1-x-2 x^2\right)}=\frac{1+x+x^2}{(1+x)(1-2 x)(1+x)} \text {, }
$$