538
離散數學（上）

二項式定理應用（2）－將二項式定理微分後，再代入特定值
請證明 $\sum_{j=0}^n j \cdot\binom{n}{j}=n \cdot 2^{n-1}$ ，其中 $n$ 為正整数。

【重要】

【證明】
由二項式定理 $(x+y)^n=\sum_{i=0}^n\binom{n}{i} x^i y^{n-i}$ ，
左右分別對 $x$ 微分，得 $n(x+y)^{n-1}=\sum_{i=1}^n i\binom{n}{i} x^{i-1} y^{n-i}$ ，
代入 $x=y=1$ ，得 $n \cdot 2^{n-1}=\sum_{i=0}^n i\binom{n}{i}$ 。
另證 ：
$$
\sum_{j=0}^n j\binom{n}{j}=\sum_{j=1}^n j\binom{n}{j}=\sum_{j=1}^n j \frac{n}{j}\binom{n-1}{j-1}=n \sum_{k=0}^{n-1}\binom{n-1}{k}=n \cdot 2^{n-1} 。
$$

基礎類題
1．What is the value of the summation $\sum_{k=1}^n k C(n, k)$ when $n=10$ ？

【104 政大資科】
解 $2^9 \times 10$

2．$\sum_{k=0}^n\left(k 3^{k-1} \cdot C(n, k)\right)=$ ？

【108 台大電棈】

解 由二項式定理 $(x+y)^n=\sum_{i=0}^n\binom{n}{i} x^i y^{n-i}$ ，
左右分別對 $x$ 微分，得 $n(x+y)^{n-1}=\sum_{i=1}^n i\binom{n}{i} x^{i-1} y^{n-i}$ ，
代入 $x=3, y=1$ ，得 $n(3+1)^{n-1}=\sum_{i=1}^n i \cdot 3^{i-1}\binom{n}{i}$ ，
故回答：$n \cdot 4^{n-1}$ 。