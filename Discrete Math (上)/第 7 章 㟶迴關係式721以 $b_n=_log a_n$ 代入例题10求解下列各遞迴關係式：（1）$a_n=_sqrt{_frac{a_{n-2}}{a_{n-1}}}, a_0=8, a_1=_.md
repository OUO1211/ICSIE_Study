第 7 章 㟶迴關係式
721

以 $b_n=\log a_n$ 代入
例题

10

求解下列各遞迴關係式：
（1）$a_n=\sqrt{\frac{a_{n-2}}{a_{n-1}}}, a_0=8, a_1=\frac{1}{2 \sqrt{2}}$ ．
（2）$\left\{\begin{array}{l}a_{n+2}=a_{n+1}^2 / a_n, n \geq 0 \\ a_0=1, a_1=2\end{array}, a_n \geq 0\right.$ ．
【88 中興資科】【107 成大工科】
解（1）原式等於 ： $\log _2 a_n=\log _2\left(\sqrt{\frac{a_{n-2}}{a_{n-1}}}\right)=\frac{1}{2}\left(\log _2 a_{n-2}-\log _2 a_{n-1}\right)$ ，
令 $b_n=\log _2 a_n$ 代入原式，得 $\left\{\begin{array}{l}b_n=\frac{1}{2}\left(b_{n-2}-b_{n-1}\right) \\ b_0=3, b_1=-\frac{3}{2}\end{array}\right.$ ，解得 $b_n=2^{-n}+2 \cdot(-1)^n$ ，
還原得 $a_n=2^{2^{-n}+2 \cdot(-1)^n}, n \geq 0$ ．
（2）原式等於 ： $\log _2 a_{n+2}=\log _2\left(\frac{a_{n+1}^2}{a_n}\right)=2 \log _2 a_{n+1}-\log _2 a_n$ ，
令 $b_n=\log _2 a_n$ 代入原式，得 $\left\{\begin{array}{l}b_{n+2}=2 b_{n+1}-b_n \\ b_0=0, b_1=1\end{array}\right.$ ，可解得 $b_n=n$ ，
還原得 $a_n=2^{b_n}=2^n, n \geq 0$ 。
另解一 ：
原式：$\frac{a_{n+2}}{a_{n+1}}=\frac{a_{n+1}}{a_n}=\cdots=\frac{a_1}{a_0}=2, \therefore a_{n+2}=2 a_{n+1}=\cdots=2^{n+2} a_0=2^{n+2}$ ，
$$
\therefore a_n=2^n, n \geq 0 \text { 。 }
$$

另解二：
觀察原遞迴關係可得 ：$a_0=1, a_1=2, a_2=4, a_3=8, a_4=16, \ldots$ ，
可猜測通解為 $a_n=2^n, ~ n \geq 0$ ，再以歸納法完成證明。