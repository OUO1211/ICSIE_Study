第4章 數學歸納法與數論 365

應用乘法反元素於同餘方程的計算：
例題 10
（1）（5\％）Find an inverse of $72 \bmod 233$.
【91、92 中央資工類题】
（2）$(5 \%)$ Solve the congruence $72 x \equiv 6 \bmod 233$ ．
【98、100、101、104、106、109、110中正資工】

解（1）先完成 233 與 72 的輾轉相除法：
$$
233=72 \cdot 3+17,72=17 \cdot 4+4,17=4 \cdot 4+1
$$

故得
$$
\begin{aligned}
1 & =17-4 \cdot 4=17-4 \cdot(72-17 \cdot 4) \\
& =17 \cdot 17-4 \cdot 72=(233-72 \cdot 3) \cdot 17-4 \cdot 72 \\
& =233 \cdot 17-72 \cdot 55
\end{aligned}
$$

左右同取 $\bmod 233$ ，得 $1 \equiv 72(-55) \bmod 233$ ，
又 $-55 \equiv 178 \bmod 233$ ，故 72 的乘法反元素為 178 。
（2）由 $72 x \equiv 6 \bmod 233$ 左右同乘以 178 ，
則左側 $(178) 72 x \equiv x \bmod 233$ ，右側 $178 \cdot 6 \equiv 1068 \equiv 136 \bmod 233$ ，
故得 $x \equiv 136 \bmod 233$（也相當於 $x=136+233 k, k$ 為任意整數）。

例題 11
（ $4 \%$ ）Find all solutions，if any，to the system of congruences $\left\{\begin{array}{c}2 x \equiv 4 \bmod 8 \\ x \equiv 6 \bmod 9\end{array}\right.$. 【 104 交大資工】
解 求解 $2 x \equiv 4 \bmod 8$ ，即求解 $8 \mid 4-2 x$ ，找整數 $x, y$ 使 $4-2 x=8 y$ 成立。
求解 $x \equiv 6 \bmod 9$ ，即求解 $9 \mid 6-x$ ，即找整數 $x, z$ 使 $6-x=9 z$ 成立。
整理兩式，代入消去 $x$ ，
亦即找整數 $y, z$ 使 $8=18 z-8 y$ ，即 $4=9 z-4 y$ ，
可得一解 $(4,8)$ ，得 $z$ 的一般解 $4+4 t, ~ t$ 為整數，
代回得 $x=6-9(4+4 t)=-30-36 t$ ，
即 $x \equiv 6 \bmod 36$ 。（也可回答 $x \equiv 6$ 或 $42 \bmod 72$ ）