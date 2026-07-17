606
離散數學（上）

運用生成函數求和

例題
（1）Obtain a formula for $\sum_{k=0}^n k^2$ ．
（2）Find the value of $3 \cdot 2 \cdot 1+4 \cdot 3 \cdot 2+\cdots+(n+1) n(n-1)$ ．
【 $84 、 95$ 成大電機】
（3）$(15 \%)$ Compute $\sum_{k=0}^{\infty}(2 k+1) \cdot \frac{1}{3^{2 k}}$ ．
【104 台大電機】

解（1）由例題1（5）知 $0+\left(0^2+1^2\right) x+\left(0^2+1^2+2^2\right) x^2+\left(0^2+1^2+2^2+3^2\right) x^3+\cdots$
$=x(1+x)(1-x)^{-4}=f(x)$ ，而 $x^n$ 係數 $0^2+1^2+2^2+\cdots+n^2$ 即為所求，
$$
f(x)=x(1+x)(1-x)^{-4}=\left(x+x^2\right) \sum_{i=0}^{\infty}\binom{-4}{i}(-x)^i=x \sum_{i=0}^{\infty}\binom{3+i}{i} x^i+x^2 \sum_{i=0}^{\infty}\binom{3+i}{i} x^i
$$

前項取 $i=n-1$ ，後項取 $i=n-2$ ，
共得係數 $\binom{n+2}{n-1}+\binom{n+1}{n-2}=\frac{n(n+1)(2 n+1)}{6}$ 。
（2）$\because 1+x+x^2+x^3+\cdots=(1-x)^{-1}$ ，
左右各對 $x$ 微分得 $1+2 x+3 x^2+4 x^3+5 x^4+\cdots=(1-x)^{-2}$ ，
再左右各對 $x$ 微分得 $2 \cdot 1+3 \cdot 2 x+4 \cdot 3 x^2+5 \cdot 4 x^3+\cdots=2(1-x)^{-3}$ ，
再左右各對 $x$ 微分得 $3 \cdot 2 \cdot 1+4 \cdot 3 \cdot 2 x+5 \cdot 4 \cdot 3 x^2+\cdots=6(1-x)^{-4}$ ，
左右同乘以 $\frac{1}{1-x}$ 得
$3 \cdot 2 \cdot 1+(3 \cdot 2 \cdot 1+4 \cdot 3 \cdot 2) x+(3 \cdot 2 \cdot 1+4 \cdot 3 \cdot 2+5 \cdot 4 \cdot 3) x^2+\cdots=6(1-x)^{-5}$ ，
左式的 $x^{n-2}$ 項係數 $(3 \cdot 2 \cdot 1+4 \cdot 3 \cdot 2+\cdots+(n+1) n(n-1))$ 為所求，
而 $6(1-x)^{-5}=6 \sum_{i=0}^{\infty}\binom{-5}{i}(-x)^i=6 \sum_{i=0}^{\infty}\binom{4+i}{i} x^i$ ，
取 $i=n-2$ ，得右式 $x^{n-2}$ 係數 ： $6\binom{n+2}{n-2}$ ，
（3）$\because 1+x+x^2+x^3+x^4+x^5+\cdots=\frac{1}{1-x}$ ，
且 $1-x+x^2-x^3+x^4-x^5+\cdots=\frac{1}{1+x}$ ，
兩式相減，再除以 2 得