第4章 數學歸納法與數論
403

正因數個數與總和
設 $n=p_1^{e_1} p_2^{e_2} \ldots p_k^{e_k}$ 為 $n$ 之質因数分解，則
（1）$n$ 的正因数個数為 $\prod_{i=1}^k\left(e_i+1\right)$ 。
（2）$n$ 的所有正因数個数之和為 $\prod_{i=1}^k\left(p_i^0+p_i^1+\ldots+p_i^{e_i}\right)$ 。
例如： $60=2^2 \times 3 \times 5$ ，
所以 60 共有 $(2+1)(1+1)(1+1)=12$ 個正因數 ：
$$
1,2,3,4,5,6,10,12,15,20,30,60 .
$$

又，所有 60 之正因數之總和：
$$
\begin{aligned}
= & 2^0 3^0 5^0+2^0 3^0 5^1+2^0 3^1 5^0+2^0 3^1 5^1+2^1 3^0 5^0+2^1 3^0 5^1+2^1 3^1 5^0+2^1 3^1 5^1 \\
& +2^2 3^0 5^0+2^2 3^0 5^1+2^2 3^1 5^0+2^2 3^1 5^1 \\
= & \left(2^0+2^1+2^2\right)\left(3^0+3^1\right)\left(5^0+5^1\right)=168 .
\end{aligned}
$$

例題
（15\％）Given a number $x=329313600$ ，please answer the following questions．
（1）How many positive divisors does $x$ have？
（2）How many positive divisors of $x$ that are divisible by 252 ？
（3）Determine how many positive divisors of $x$ are perfect squares？

【102 中山電機】

解 $x=329313600=2^6 \times 3^5 \times 5^2 \times 7 \times 11^2$ ，
（1）正因數個數為 $(6+1)(5+1)(2+1)(1+1)(2+1)=756$ ．
（2） $252=2^2 \times 3^2 \times 7$ ，令 $d$ 為 $x$ 的正因數且可被 252 整除，則 $d=2^i \times 3^j \times 5^k \times 7 \times 11^l$ ，其中， $2 \leq i \leq 6,2 \leq j \leq 5,0 \leq k \leq 2,0 \leq l \leq 2$ ，故共有 $5 \times 4 \times 3 \times 3=180$ 種 $d$ 。
（3）令 $p$ 為 $x$ 的正因數且為完全平方數，則 $p=2^i \times 3^j \times 5^k \times 11^l$ ，其中， $0 \leq i \leq 6,0 \leq j \leq 5,0 \leq k \leq 2,0 \leq l \leq 2$ ，且均為偶數，
故共有 $4 \times 3 \times 2 \times 2=48$ 種 $p$ 。