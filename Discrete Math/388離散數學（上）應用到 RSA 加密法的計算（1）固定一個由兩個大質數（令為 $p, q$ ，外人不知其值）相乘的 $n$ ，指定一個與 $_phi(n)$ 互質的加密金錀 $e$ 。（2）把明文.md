388
離散數學（上）

應用到 RSA 加密法的計算
（1）固定一個由兩個大質數（令為 $p, q$ ，外人不知其值）相乘的 $n$ ，指定一個與 $\phi(n)$ 互質的加密金錀 $e$ 。
（2）把明文 $x$ 加密成為密文 $y$ ，其中 $y \equiv x^e \bmod n$ 。
（3）計算解密金䤻 $d$ ，其中，$e \times d \equiv 1 \bmod \phi(n), \phi(n)=(p-1)(q-1)$ 。
（4）利用 $y^d \equiv x \bmod n$ 可解回明文。
（5）就算 $n, y, e$ 都被得知，外界依舊不易解回明文 $x$ 。因為解密金錀 $d$ 的取得，需依賴 $\phi(n)$ ，亦即須先對 $n$ 完成質因數分解，故此加密法是安全的。

例題 14
（14\％）RSA encrypts an integer $X$ into another integer $Y$ by $Y=X^e \bmod n$ with a particular key $(n, e)$ ．
（1）If $n=p \times q(p, q$ primes $), \operatorname{gcd}(X, p)=\operatorname{gcd}(X, q)=1$ ，and $d e \equiv 1 \bmod (p-1)(q-1)$ ，please prove $Y^d \equiv X \bmod p q$ ．
（2）Given $Y=981$ and a key $(n=2537, e=13)$ ．Please decrypt $Y$ ，what is the original integer $X$ ？（Hint：the fast modular exponentiation．）

【108政大資科】
解（1）因為 $n=p q, ~ \therefore \phi(n)=(p-1)(q-1)$ ，且令 $d e=\phi(n) k+1, k \in Z$ ，
則尤拉定理得 $Y^d \equiv X^{e d} \equiv X^{\phi(n) k+1} \equiv\left[X^{\phi(n)}\right]^k X \equiv 1^k X \equiv X \bmod n$ 。
（2）$n=43 \times 59=p \times q, \phi(2537)=(p-1) \times(q-1)=42 \times 58=2436$ ，
先解 $13 d \equiv 1 \bmod 42 \times 58$ ，得 $d=937$ ，
$$
\therefore X \equiv Y^d \equiv 981^{937} \bmod 2537 \Leftrightarrow\left\{\begin{array} { l } 
{ X \equiv 9 8 1 ^ { 9 3 7 } \operatorname { m o d } 4 3 } \\
{ X \equiv 9 8 1 ^ { 9 3 7 } \operatorname { m o d } 5 9 }
\end{array} \Leftrightarrow \left\{\begin{array}{l}
X \equiv 16 \bmod 43 \\
X \equiv 28 \bmod 59
\end{array}\right.\right.
$$

其中，由費瑪小定理可得 $\left\{\begin{array}{l}981^{42} \equiv 1 \bmod 43 \\ 981^{58} \equiv 1 \bmod 59\end{array}\right.$ ，故
$$
\begin{aligned}
& 981^{937} \equiv 981^{42 \times 22+13} \equiv 1^{22} \cdot 981^{13} \equiv 35^{13} \equiv 35^8 \cdot 35^4 \cdot 35 \equiv(-8) \cdot 11 \cdot(-8) \equiv 16 \bmod 43 \\
& 981^{937} \equiv 981^{58 \times 16+9} \equiv 1^{16} \cdot 981^9 \equiv 37^9 \equiv 37^8 \cdot 37 \equiv 27 \cdot 37 \equiv 55 \bmod 59
\end{aligned}
$$
∴ 最後由中國剩餘定理解 $\left\{\begin{array}{l}X \equiv 16 \bmod 43 \\ X \equiv 55 \bmod 59\end{array}\right.$ ，得 $X \equiv 704 \bmod 2537$ 。