第4章 數學歸納法與數論 347

輾轉相除法（Euclidean Algorithm）一求兩正整數的最大公因數
（1）引用性質：
考虑正整数 $a, b$ 且 $a \geq b$ ，若 $a$ 除以 $b$ 得商 $q$ 與非零餘數 $r$ ，則 $\operatorname{gcd}(a, b)=\operatorname{gcd}(b, r)$
（2）一般化的表達：
令 $a=r_0, b=r_1 \in N$ ，若 $\left\{\begin{array}{l}r_0=r_1 \cdot q_1+r_2 \\ r_1=r_2 \cdot q_2+r_3 \\ \vdots \\ r_{n-2}=r_{n-1} \cdot q_{n-1}+r_n \\ r_{n-1}=r_n \cdot q_n\end{array}\right.$ ，其中 $0<r_{i+1}<r_i, \forall i=1 \sim n-1$ ，
則 $r_n=\operatorname{gcd}(a, b)$ 。

【91暨南資工】

【證明】
（1）令 $\operatorname{gcd}(a, b)=h, \operatorname{gcd}(b, r)=k$ ，
所以 $h|a, h| b, \therefore h|a-b q, \therefore h| r, \therefore h$ 為 $b, r$ 之公因數，$\therefore h \leq k$ $\_\_\_\_$

又 $\because k|b, k| r, \therefore k|b q+r, \therefore k| a, \therefore k$ 為 $a, b$ 之公因數，$\therefore k \leq h$ $\_\_\_\_$

由 $(*),(* *)$ 知 $\therefore k=h$ 。
（2）利用前述結果可得 ：
$$
\operatorname{gcd}(a, b)=\operatorname{gcd}\left(r_0, r_1\right)=\operatorname{gcd}\left(r_1, r_2\right)=\ldots=\operatorname{gcd}\left(r_{n-1}, r_n\right)=\operatorname{gcd}\left(r_n q_n, r_n\right)=r_n .
$$

例如：以 Euclid＇s algorithm 求 $\operatorname{gcd}(208,234)$ 的步驟如下：
$$
\begin{aligned}
& 234=208 * 1+26 \\
& 208-26 * 8+0 \quad \therefore \operatorname{gcd}(234,208)=26 .
\end{aligned}
$$

例如：令 $n=13923$ 且 $m=13056$ ，用以下演算法計算 $\operatorname{gcd}(n, m)$ 。
while $(m>0)$ do
$$
\begin{gathered}
\{r=n \bmod m ; \\
n=m ; \\
m=r ;\}
\end{gathered}
$$

Return $n$

【105清大資工】
$$
\begin{aligned}
& 13923=13056 \times 1+867 \\
& 13056=867 \times 15+51 \\
& 867=51 \times 17+0, \\
& \therefore \operatorname{gcd}(13923,13056)=51 .
\end{aligned}
$$