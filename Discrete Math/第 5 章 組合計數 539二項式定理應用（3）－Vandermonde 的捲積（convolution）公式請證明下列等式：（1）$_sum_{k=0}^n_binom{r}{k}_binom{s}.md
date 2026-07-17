第 5 章 組合計數 539

二項式定理應用（3）－Vandermonde 的捲積（convolution）公式
請證明下列等式：
（1）$\sum_{k=0}^n\binom{r}{k}\binom{s}{n-k}=\binom{r+s}{n}$ ．
【87中山資工】【92、102中央資工】
（2）$\sum_{k=0}^n\binom{n}{k}^2=\binom{2 n}{n}$ ．

【很重要】

【證明】
（1）$\binom{r+s}{n}$ 即從 $r+s$ 個相異物不重複取 $n$ 個的方法數，亦可考慮如下：
分成兩堆：左 $r$ 個，右 $s$ 個，
而從左取出 $k$ 個，右取出 $n-k$ 個， $0 \leq k \leq n$ ，則方法數為 $\binom{r}{k}\binom{s}{n-k}$ ，
故共有方法數為 $\binom{r}{0}\binom{s}{n}+\binom{r}{1}\binom{s}{n-1}+\binom{r}{2}\binom{s}{n-2}+\ldots+\binom{r}{n}\binom{s}{0}=\sum_{k=0}^n\binom{r}{k}\binom{s}{n-k}$ ，得證。
（2）將捲積公式以 $r=s=n$ 代入即可；
或另證如下：
由二項式定理知：$(1+x)^{2 n}=\sum_{i=0}^{2 n}\binom{2 n}{i} x^i$ ，所以 $x^n$ 係數為：$\binom{2 n}{n}$ ，
又 $(1+x)^{2 n}=(1+x)^n(1+x)^n=\left(\binom{n}{0}+\binom{n}{1} x+\ldots+\binom{n}{n} x^n\right)\left(\binom{n}{0}+\binom{n}{1} x+\ldots+\binom{n}{n} x^n\right)$ ，
故乘開可得 $x^n$ 係數為：
$\binom{n}{0}\binom{n}{n}+\binom{n}{1}\binom{n}{n-1}+\binom{n}{2}\binom{n}{n-2}+\ldots+\binom{n}{n}\binom{n}{0}=\binom{n}{0}^2+\binom{n}{1}^2+\binom{n}{2}^2+\ldots+\binom{n}{n}^2$ ，得證。