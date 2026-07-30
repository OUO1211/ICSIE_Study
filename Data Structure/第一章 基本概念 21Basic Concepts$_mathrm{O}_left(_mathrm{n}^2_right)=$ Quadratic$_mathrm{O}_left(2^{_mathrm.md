第一章 基本概念 21
Basic Concepts

$\mathrm{O}\left(\mathrm{n}^2\right)=$ Quadratic
$\mathrm{O}\left(2^{\mathrm{n}}\right)=$ Exponential（NP－Complete）
order（小→大）：
$O(1), O(\log n), O(n), O(n \log n), O\left(n^2\right), O\left(n^3\right), O\left(2^n\right), O(n!)$
（D）定理
if $\mathrm{f}(\mathrm{n})=\mathrm{a}_{\mathrm{m}} \mathrm{n}^{\mathrm{m}}+\mathrm{a}_{\mathrm{m}-1} \mathrm{n}^{\mathrm{m}-1}+\cdots \mathrm{a}_1 \mathrm{n}+\mathrm{a}_0$ ，
then $\mathrm{f}(\mathrm{n})=\mathrm{O}\left(\mathrm{n}^{\mathrm{m}}\right)$
【證明】
$$
\begin{aligned}
f(n) & \leq \sum_{i=0}^m \mid a_i n^i \\
& \leq n^m \sum_{i=0}^m\left|a_i\right| n^{i-m} \\
& \leq n^m \sum_{i=0}^m\left|a_i\right|, \text { for } n \geq 1 \quad\left(\text { 即 } c=\sum_{i=0}^m\left|a_i\right|, n_0=1\right)
\end{aligned}
$$
$\mathbf{1}-\mathbf{5}-\mathbf{2} \boldsymbol{\Omega}$
Definition ：［Omega］ $\mathrm{f}(\mathrm{n})=\Omega(\mathrm{g}(\mathrm{n}))$
if there exist two positive constants c and $\mathrm{n}_0$ s．t．
$\mathrm{f}(\mathrm{n}) \geqq \mathrm{cg}(\mathrm{n})$ ，for all $\mathrm{n}, \mathrm{n} \geqq \mathrm{n}_0$

例題 1－20
\begin{itemize}
\item[（1）] $\mathrm{f}(\mathrm{n})=3 \mathrm{n}+3=\Omega(\mathrm{n})$
$\because 3 \mathrm{n}+3 \geqq 3 \mathrm{n},\left(\mathrm{c}=3, \mathrm{n}_0=1\right)$ ，for $\mathrm{n} \geqq 1$
\item[（2）] $62^{\mathrm{n}}+\mathrm{n}^2=\Omega\left(2^{\mathrm{n}}\right)$
\end{itemize}

1－5－3 θ
Definition ：［Theta］ $\mathrm{f}(\mathrm{n})=\theta(\mathrm{g}(\mathrm{n}))$
If there exist three positive constants $\mathrm{c}_1, \mathrm{c}_2$ and $\mathrm{n}_0$ ，such that $\mathrm{c}_1 \mathrm{~g}(\mathrm{n}) \leqq \mathrm{f}(\mathrm{n}) \leqq \mathrm{c}_2 \mathrm{~g}(\mathrm{n})$ ，for all $\mathrm{n}, \mathrm{n} \geqq \mathrm{n}_0$