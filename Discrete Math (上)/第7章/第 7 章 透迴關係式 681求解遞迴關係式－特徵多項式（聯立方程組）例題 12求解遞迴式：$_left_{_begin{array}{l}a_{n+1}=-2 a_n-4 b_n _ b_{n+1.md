第 7 章 透迴關係式 681

求解遞迴關係式－特徵多項式（聯立方程組）

例題 12
求解遞迴式：$\left\{\begin{array}{l}a_{n+1}=-2 a_n-4 b_n \\ b_{n+1}=4 a_n+6 b_n\end{array} \quad n \geq 0, a_0=1, b_0=0\right.$ 。
【93 清大資應類題】【105 清大資工類題】【95中山資工】［96、106 台科資工］
解 用代入消去法：
由第 2 式得 ：$a_n=\frac{1}{4}\left(b_{n+1}-6 b_n\right)$ ，
代入第 1 式：$\frac{1}{4}\left(b_{n+2}-6 b_{n+1}\right)=-2 \cdot \frac{1}{4}\left(b_{n+1}-6 b_n\right)-4 b_n$ ，
整理得：$b_{n+2}-4 b_{n+1}+4 b_n=0$ ，
而初值條件為：$b_0=0, b_1=4 a_0+6 b_0=4$ ，
$b_n$ 之特徵式為 $\alpha^2-4 \alpha+4=(\alpha-2)^2=0$ ，特徵根為 2,2 ，
$$
\therefore b_n=c_1 2^n+c_2 2^n n \text {, }
$$

再由 $\left\{\begin{array}{l}b_0=0=c_1 \\ b_1=4=2 c_1+2 c_2\end{array}\right.$ ，解得 $c_1=0, c_2=2, \therefore b_n=n 2^{n+1}$ ，
$$
\therefore a_n=\frac{1}{4}\left(b_{n+1}-6 b_n\right)=\frac{1}{4}\left[(n+1) 2^{n+2}-6 n 2^{n+1}\right]=\frac{1}{4}(2-4 n) 2^{n+1}=(1-2 n) 2^n \text {, }
$$

故回答 $\left\{\begin{array}{l}a_n=(1-2 n) 2^n \\ b_n=n 2^{n+1}\end{array}, n \geq 0\right.$ 。