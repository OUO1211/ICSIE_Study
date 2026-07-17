392
離散數學（上）

今有物不知其数，三三數之餘二，五五數之餘三，七七數之餘四，問物幾何？
解曰：三人同行七十稀，五樹梅花二一枝，七子團圓正月半，除百零五便得知。
射鵰英雄傳

中國剩餘定理（Chinese Remainder Theorem）
若 $n_i \in N, r_i \in Z, i=1 \sim k$ 且 $\operatorname{gcd}\left(n_i, n_j\right)=1, \forall i \neq j$ ，則同餘方程 $\left\{\begin{array}{c}x \equiv r_1 \bmod n_1 \\ x \equiv r_2 \bmod n_2 \\ \vdots \\ x \equiv r_k \bmod n_k\end{array}\right.$
在 $\bmod n$ 下有唯一解 $\sum_{j=1}^k r_j N_j M_j$ ，其中 $n=\prod_{i=1}^k n_i, N_j=\frac{n}{n_j}, M_j N_j \equiv 1 \bmod n_j$ ．
【90 海洋資科】【96 台科資エ】【110中央資工】
【證明】
$$
\because \operatorname{gcd}\left(n_i, n_j\right)=1, \forall i \neq j \text {, 且 } N_j=\frac{n_1 \times n_2 \times \ldots \times n_j \times \ldots \times n_k}{n_j}, \therefore \operatorname{gcd}\left(n_j, N_j\right)=1, \forall j \text {, }
$$

且 $n_j \mid N_i \forall i \neq j$
$$
\because x^*=\sum_{j=1}^k r_j N_j M_j=r_1 N_1 M_1+\ldots+r_k N_k M_k \equiv r_j N_j M_j \equiv r_j \bmod n_j, \forall j
$$

故得 $x^*$ 滿足各個模同餘方程，即此為其解。
又若有另一解 $x^{\prime}$ 滿足 $x^{\prime} \equiv r_j \bmod n_j$ ，即得 $x^* \equiv x^{\prime} \equiv r_j \bmod n_j, \forall j$ ，
$\therefore n_j \mid x^*-x^{\prime}, \therefore x^* \equiv x^{\prime} \bmod n$ ，故知 $x^*$ 在 $\bmod n$ 下為唯一解。
例 ：求解同餘方程組 $\left\{\begin{array}{lll}x \equiv 2 & \bmod & 3 \\ x \equiv 3 & \bmod & 5 \\ x \equiv 2 & \bmod & 7\end{array}\right.$ 。
【91成大電機】【97中正資工】【98 清大資工】【104 刑事警察】
解
$$
\begin{array}{llll}
n_1=3 & r_1=2 & N_1=5 \cdot 7=35 & M_1 \cdot 35 \equiv 1 \bmod 3 \\
n_2=5 & , n=105 & M_1 \equiv 2 \bmod 3 \\
n_3=7 & r_2=3 \cdot N_2=3 \cdot 7=21, & M_2 \cdot 21 \equiv 1 \bmod 5 \Rightarrow & M_2 \equiv 1 \bmod 5 \\
\therefore x \equiv 2 \cdot 35 \cdot 2+3 \cdot 21 \cdot 1+2 \cdot 15 \cdot 1 \equiv 233 \equiv 23 \bmod 105 & r_3=2 & N_3=3 \cdot 5=15 & M_3 \cdot 15 \equiv 1 \bmod 7
\end{array},
$$