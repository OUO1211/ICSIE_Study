656
離散數學（上）

求解遞迴關係式－特徵多項式
稱 $b_n a_n+b_{n-1} a_{n-1}+\ldots+b_{n-k} a_{n-k}=f(n)$ 為 $-k$ 階，常係数，線性，遞迴關係式。
其中，$n, k \in N, b_n \sim b_{n-k}$ 為實数常数，$b_n^{\prime}, b_{n-k} \neq 0$ ，且
當 $f(n)=0$ 時，又稱為齊次式（homogeneous）；
當 $f(n) \neq 0$ 時，又稱為非齊次式（nonhomogeneous）。
解題步驟 ：
1．判別是否為常係數，線性，齊次遞迴式。
2．以 $a_n=A \alpha^n$ 代入原式，化簡得 $b_n \alpha^k+b_{n-1} \alpha^{k-1}+\ldots+b_{n-k}=0$ ，
3．解出其特徴根：$\alpha_1, \alpha_2, \ldots, \alpha_k$ 。
4．令 $a_n=c_1 \alpha_1^n+c_2 \alpha_2^n+\ldots+c_k \alpha_k^n$ ，並以是否重根完成修正。
5．以題目之初值條件解常係數 $c_1, c_2, \ldots, c_k$ 。

求解遞迴關係式－特徵多項式（齊次，特徵根相異）
若有 $\alpha_1, \alpha_2, \ldots, \alpha_r$ 為相異特徵根，則 $a_n=c_1 \alpha_1^n+c_2 \alpha_2^n+\ldots+c_r \alpha_r^n, c_1 \sim c_r$ 為常數。
例如：若只 $2,3,-4$ 為其特徵根，則設 $a_n=c_1 2^n+c_2 3^n+c_3(-4)^n$ 。

例題
解下列各遞迴關係式：
（1）$\left\{\begin{array}{l}a_n=a_{n-1}+2 a_{n-2}, n \geq 2 \\ a_0=-3, a_1=0\end{array}\right.$ ．

【＊＊＊＊＊資エ】

（2）$\left\{\begin{array}{l}2 a_{n+3}=a_{n+2}+2 a_{n+1}-a_n, n \geq 0 \\ a_0=0, a_1=1, a_2=2\end{array}\right.$ ．
【99清大資應類題】【105台北資工】【暨南資工】

解（1）化簡得特徵式：$\alpha^2-\alpha-2=(\alpha+1)(\alpha-2)=0$ ，得特徵根為 $-1,2$ ，
故設 $a_n=c_1 \cdot(-1)^n+c_2 \cdot 2^n$ ，
再由初值條件 $\left\{\begin{array}{l}a_0=-3=c_1 \cdot(-1)^0+c_2 \cdot 2^0 \\ a_1=0=c_1 \cdot(-1)^1+c_2 \cdot 2^1\end{array}\right.$ ，解得 $c_1=-2, c_2=-1$ ，
$$
\therefore a_n=-2 \cdot(-1)^n-2^n, n \geq 0 。
$$
（2）整理得 $2 a_n-a_{n-1}-2 a_{n-2}+a_{n-3}=0$ ，
其特徵式： $2 \alpha^3-\alpha^2-2 \alpha+1=(2 \alpha-1)(\alpha+1)(\alpha-1)=0$ ，