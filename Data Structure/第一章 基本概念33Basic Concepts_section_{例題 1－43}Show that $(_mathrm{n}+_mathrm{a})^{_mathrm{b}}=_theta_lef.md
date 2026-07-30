第一章 基本概念
33
Basic Concepts

\section*{例題 1－43}

Show that $(\mathrm{n}+\mathrm{a})^{\mathrm{b}}=\theta\left(\mathrm{n}^{\mathrm{b}}\right)$
證 須找出 $\mathrm{c}_1, \mathrm{c}_2, \mathrm{n}_0$ ，s．t．
$$
0 \leq c_1 \cdot n^b \leq(n+a)^b \leq c_2 \cdot n^b \text { for all } n \geq n_0
$$
Note that：
$$
\mathrm{n}+\mathrm{a} \leq \mathrm{n}+|\mathrm{a}| \leq 2 \cdot \mathrm{n} \text { when }|\mathrm{a}| \leq \mathrm{n}
$$
and
$$
n+a \geq n-|a| \geq \frac{1}{2} n \text { when }|a| \leq \frac{1}{2} n
$$
Thus， $0 \leq \frac{1}{2} \mathrm{n} \leq \mathrm{n}+\mathrm{a} \leq 2 \mathrm{n}$ when $\mathrm{n} \geq 2|\mathrm{a}|$
Since $b>0$ ，所以兩邊都冪次 $b$ 方仍然成立
$$
\begin{aligned}
0 & \leq\left(\frac{1}{2} n\right)^b \leq(n+a)^b \leq(2 n)^b \\
0 & \leq\left(\frac{1}{2}\right)^b n^b \leq(n+a)^b \leq 2^b n^b \\
\therefore c_1 & =\left(\frac{1}{2}\right)^b, c_2=2^b, n_0=2|a|, \text { Satisfy the definition }
\end{aligned}
$$