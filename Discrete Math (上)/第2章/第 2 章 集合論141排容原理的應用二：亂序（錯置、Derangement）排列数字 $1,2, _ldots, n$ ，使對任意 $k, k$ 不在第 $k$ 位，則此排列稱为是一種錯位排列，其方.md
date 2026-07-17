第 2 章 集合論
141

排容原理的應用二：亂序（錯置、Derangement）
排列数字 $1,2, \ldots, n$ ，使對任意 $k, k$ 不在第 $k$ 位，則此排列稱为是一種錯位排列，其方法数記為 $D_n$ ，則 $D_n=n!\times\left[1-\frac{1}{1!}+\frac{1}{2!}-\frac{1}{3!}+\ldots+(-1)^n \frac{1}{n!}\right]=n!\times\left(\sum_{k=0}^n(-1)^k \frac{1}{k!}\right)$

【證明】
令 $U$ 為 $n$ 個數字的所有排列法所成集合，集合 $A_i$ 表數字 $i$ 在正確位置的排列方法，則所求 $D_n=\left|\overline{A_1} \cap \overline{A_2} \cap \ldots \cap \overline{A_n}\right|$ ，

其中 $|U|=n!$ ，
$\left|A_i\right|=i$ 必在正確位置的排列法 $=(n-1)!, 1 \leq i \leq n$ ，
$\left|A_i \cap A_j\right|=i$ 與 $j$ 必在正確位置之排列法 $=(n-2)!\cdot 1 \leq i<j \leq n \cdot$
$$
\vdots
$$

故由排容原理知所求 $D_n$
$$
\begin{aligned}
& =|U|-\sum_{1 \leq i s n}\left|A_i\right|+\sum_{1 \leq i<j \leq n}\left|A_i \cap A_j\right|-\sum_{1 \leq i<j<k \leq n}\left|A_i \cap A_j \cap A_k\right|+\ldots \\
& =n!-\binom{n}{1} \cdot(n-1)!+\binom{n}{2} \cdot(n-2)!-\binom{n}{3} \cdot(n-3)!+\ldots+(-1)^n \cdot\binom{n}{n} \cdot(n-n)! \\
& =\sum_{i=0}^n(-1)^i \cdot\binom{n}{i} \cdot(n-i)!=n!\cdot \sum_{i=0}^n \frac{(-1)^i}{i!}
\end{aligned}
$$

Note
（1）$\because e^{-x}=1-\frac{x}{1!}+\frac{x^2}{2!}-\frac{x^3}{3!}+\ldots, \therefore \lim _{n \rightarrow \infty} \frac{D_n}{n!}=1-\frac{1}{1!}+\frac{1}{2!}-\frac{1}{3!}+\ldots=e^{-1}=\frac{1}{2.71828 \ldots} \approx 37 \%$ 。即當 $n$ 很大時，每個數字皆排錯的機率將近 3 成 7 。

【103 嘉美資工】

（2）亂序數推廣：$n$ 相異數的排列法中，
（1）恰 $r$ 個數不在正確位置上的方法數 ：$\binom{n}{r} D_r$ 。
（2）$r$ 個數以上不在正確位置上的方法數 ：$\sum_{k=r+1}^n\binom{n}{k} D_k$ 。
（3）亂序數的遞迴求算技巧：$\left\{\begin{array}{l}D_n=(n-1)\left(D_{n-1}+D_{n-2}\right), \forall n \geq 3, \\ D_1=0, D_2=1\end{array}\right.$
（148頁有證明）。