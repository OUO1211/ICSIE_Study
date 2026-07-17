662
離散數學（上）

求解遞迴關係式－特徵多項式（齊次，特徵根有重根）
若解得特徵根為 $\underbrace{\alpha_1, \ldots, \alpha_1}_{m_1 \text { 個 }}, \underbrace{\alpha_2, \ldots, \alpha_2}_{m_2 \text { 個 }}, \ldots, \underbrace{\alpha_t, \ldots, \alpha_t}_{m_t \text { 個 }}$ ，
則每個 $\alpha_i$ 對應的解為 $u_i(n)=\underbrace{c_0 \alpha_i^n+c_1 \alpha_i^n n+\ldots+c_{m_i-1} \alpha_i^n n^{m_i-1}}_{\text {共 } m_i \text { 项 }}$ ，
且 $a_n=u_1(n)+u_2(n)+\ldots+u_t(n)$ 。
例如：
若 $2,2,2,3,3,-4$ 為其特徵根，
則設通解為 $a_n=c_1 2^n+c_2 n 2^n+c_3 n^2 2^n+c_4 3^n+c_5 n 3^n+c_6(-4)^n$ 。

例題
6
解下列各遞迴關係式：
（1）$\left\{\begin{array}{l}a_n-6 a_{n-1}+9 a_{n-2}=0, n \geq 2 \\ a_0=5, a_1=12\end{array}\right.$ ．

【＊＊＊＊＊資エ】

（2）$\left\{\begin{array}{l}a_n+2 a_{n-1}-4 a_{n-2}-8 a_{n-3}=0, n \geq 3 \\ a_0=0, a_1=-6, a_2=8\end{array}\right.$ ．

【104 中山資工】

（3）$\left\{\begin{array}{l}a_n=-3 a_{n-1}-3 a_{n-2}-a_{n-3}, n \geq 3 \\ a_0=5, a_1=-9, a_2=15\end{array}\right.$ ．【97、100師大資工】【107政大資科】

解（1）特徴式：$\alpha^2-6 \alpha+9=(\alpha-3)(\alpha-3)=0$ ，得特徵根為 3 ， 3 ，
設 $a_n=c_1 3^n+c_2 n 3^n$ ，由初值條件 $\left\{\begin{array}{l}a_0=5=c_1+c_2 \cdot 0 \\ a_1=12=c_1 \cdot 3+c_2 \cdot 3\end{array}\right.$ ，
解得 $c_1=5, c_2=-1$ ，故 $a_n=5 \cdot 3^n-n 3^n, n \geq 0$ 。
（2）特徵式：$\alpha^3+2 \alpha^2-4 \alpha-8=(\alpha-2)(\alpha+2)(\alpha+2)=0$ ，特徵根為 $2,-2,-2$ ，
設 $a_n=c_1 2^n+c_2(-2)^n+c_3 n(-2)^n$ ，
由 $\left\{\begin{array}{l}a_0=0=c_1 \cdot 2^0+c_2 \cdot(-2)^0+c_3 0 \cdot(-2)^0 \\ a_1=-6=c_1 \cdot 2^1+c_2 \cdot(-2)^1+c_3 1 \cdot(-2)^1 \\ a_2=8=c_1 \cdot 2^2+c_2 \cdot(-2)^2+c_3 2 \cdot(-2)^2\end{array}\right.$ ，解得 $c_1=-1, c_2=c_3=1$ ，
故 $a_n=-2^n+(-2)^n+n(-2)^n, n \geq 0$ 。