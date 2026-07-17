268
線性代數（下）

其他常見定義長度的方式
考虑向量 $\boldsymbol{x}=\left(x_1, x_2, \ldots, x_n\right)$ ：
（1） 1 －norm：$\|\boldsymbol{x}\|_1=\left|x_1\right|+\left|x_2\right|+\ldots+\left|x_n\right|$ ．
（2）$p$－norm：$\|\boldsymbol{x}\|_p=\left(\left|x_1\right|^p+\left|x_2\right|^p+\ldots+\left|x_n\right|^p\right)^{\frac{1}{p}}, p \geq 1$ ．
（3）$\infty$－norm：$\|\boldsymbol{x}\|_{\infty}=\max \left\{\left|x_1\right|,\left|x_2\right|, \ldots,\left|x_n\right|\right\}$ ．
例如：
$\boldsymbol{x}=(1,2,-3) \in R^3$ ，則 $\|\boldsymbol{x}\|_1=|1|+|2|+|-3|=6 ;\|\boldsymbol{x}\|_{\infty}=|-3|=3$,
$\boldsymbol{y}=(1,2+i, i) \in C^3,|1|=1,|2+i|=\sqrt{2^2+1^2}=\sqrt{5},|i|=\sqrt{0^2+1^2}=1$ ，
則 $\|\boldsymbol{y}\|_1=|1|+|2+i|+|i|=2+\sqrt{5} ;\|\boldsymbol{y}\|_{\infty}=|2+i|=\sqrt{5}$ ．

Note
各種 norm 的關係：
（1）$\frac{\|\boldsymbol{x}\|_2}{\sqrt{n}} \leq\|\boldsymbol{x}\|_{\infty} \leq\|\boldsymbol{x}\|_2$ ．
【95成大電通、100中興統計、108 中山應數】
（2）$\|\boldsymbol{x}\|_2 \leq\|\boldsymbol{x}\|_1 \leq \sqrt{n}\|\boldsymbol{x}\|_2$ ．
（3）$\frac{\|\boldsymbol{x}\|_1}{n} \leq\|\boldsymbol{x}\|_{\infty} \leq\|\boldsymbol{x}\|_1$ ．
【95成大電通、108中山應數】
【證明】
設 $\boldsymbol{x}=\left(x_1, x_2, \ldots, x_n\right)$ ，
（1）令 $\|\boldsymbol{x}\|_{\infty}=\max \left\{\left|x_1\right|,\left|x_2\right|, \ldots,\left|x_n\right|\right\}=\left|x_k\right|$ ，for some $k \in\{1,2, \ldots, n\}$ ，則
$$
\begin{aligned}
& \|\boldsymbol{x}\|_2^2=\sum_{i=1}^n\left|x_i\right|^2=\left|x_1\right|^2+\ldots+\left|x_n\right|^2 \leq n\left|x_k\right|^2=n\|\boldsymbol{x}\|_{\infty}^2 \therefore\|\boldsymbol{x}\|_2 \leq \sqrt{n}\|\boldsymbol{x}\|_{\infty}, \therefore \frac{\|\boldsymbol{x}\|_2}{\sqrt{n}} \leq\|\boldsymbol{x}\|_{\mathbb{N}}, \\
& \text { 又 }\|\boldsymbol{x}\|_{\infty}=\left(\left|x_k\right|^2\right)^{\frac{1}{2}} \leq\left(\sum_{i=1}^n\left|x_i\right|^2\right)^{\frac{1}{2}}=\|\boldsymbol{x}\|_2 .
\end{aligned}
$$
（2）$\|\boldsymbol{x}\|_2^2=\left(\sum_{i=1}^n\left|x_i\right|^2\right) \leq\left(\sum_{i=1}^n\left|x_i\right|\right)^2=\|\boldsymbol{x}\|_1^2, \therefore\|\boldsymbol{x}\|_2 \leq\|\boldsymbol{x}\|_1$ ．
又由 Cauchy－Schwarz 不等式知
$$
\begin{aligned}
& \left(1 \cdot\left|x_1\right|+1 \cdot\left|x_2\right|+\ldots+1 \cdot\left|x_n\right|\right)^2 \leq\left(1^2+1^2+\ldots+1^2\right)\left(\left|x_1\right|^2+\left|x_2\right|^2+\ldots+\left|x_n\right|^2\right) \\
& \therefore\left(\sum_{i=1}^n\left|x_i\right|\right)^2 \leq n \cdot \sum_{i=1}^n\left|x_i\right|^2 \therefore\|\boldsymbol{x}\|_1 \leq \sqrt{n}\|\boldsymbol{x}\|_2 .
\end{aligned}
$$
（3）由（1）（2）可得。