第 2 章 㘳合埝

135



排容原理的應用一 ：Euler＇s phi function

$\phi(n)=|\{m \mid 1 \leq m \leq n, \operatorname{gcd}(m, n)=1\}|$ ，其中，$n$ 为大於 1 的正整数•

（即叶算小於等於 $n$ 又與 $n$ 互質的正整数個数共有多少圆）

【 77 交大資科】【 77 交大應数】【 79 交大責工】【 $91 、 97$ 台大責工】

例如，$\phi(6)=|\{1,5\}|=2$ 。

Note

（1）$\phi(n)=n \prod_{i=1}^k\left(1-\frac{1}{p_i}\right)$ ，其中 $n=p_1^\rho \ldots p_k^{e_k}, p_1, \ldots, p_k$ 为 $n$ 的相是寊因數 $\cdot e_i \geq 1, \forall i$ 。

【證明】

定義 $U=\left\{x \in Z^{+} \mid 1 \leq x \leq n\right\}$ ，且 $A_i=\left\{x \in U \mid p_i\right.$ 整除 $\left.x\right\} \cdot 1 \leq i \leq k \cdot$

其中 $|U|=n$ ，

$$

\begin{aligned}

& \left|A_i\right|=\frac{n}{p_i}, 1 \leq i \leq k \\

& \left|A_i \cap A_j\right|=\frac{n}{p_i p_j}, 1 \leq i<j \leq k \\

& \left|A_i \cap A_j \cap A_l\right|=\frac{n}{p_i p_j p_l}, 1 \leq i<j<l \leq k

\end{aligned}

$$



故由排容原理知，所求 $\phi(n)=\left|\bigcap_{i=1}^k \bar{A}_i\right|$

$$

\begin{aligned}

& =n-\sum_{\mid \leq i \leq k} \frac{n}{p_i}+\sum_{\mid \leq i<j \leq k} \frac{n}{p_i p_j}-\sum_{|\leq i<j<| \leq k} \frac{n}{p_i p_j p_l}+\ldots+(-1)^k \frac{n}{p_1 p_2 \cdots p_k} \\

& =n\left(1-\frac{1}{p_1}\right)\left(1-\frac{1}{p_2}\right) \cdots\left(1-\frac{1}{p_k}\right)=n \prod_{i=1}^k\left(1-\frac{1}{p_i}\right)

\end{aligned}

$$

（2）若 $p$ 為質數，則 $\phi(p)=p-1$ 。

（3）若 $p, q$ 為相異質數，則 $\phi(p \times q)=(p-1)(q-1)$ 。