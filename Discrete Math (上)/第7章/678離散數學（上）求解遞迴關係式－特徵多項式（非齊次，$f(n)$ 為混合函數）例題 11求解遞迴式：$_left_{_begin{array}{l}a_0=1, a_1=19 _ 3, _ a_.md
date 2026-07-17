678
離散數學（上）

求解遞迴關係式－特徵多項式（非齊次，$f(n)$ 為混合函數）
例題 11
求解遞迴式：$\left\{\begin{array}{l}a_0=1, a_1=19 / 3, \\ a_n-4 a_{n-1}+4 a_{n-2}=(1+n) \times 2^n, n \geq 2\end{array}\right.$ 。
解 其特徵式為 $\alpha^2-4 \alpha+4=0$ ，得特徵根為 2，2，
設齊次解 $a_n^{(h)}=c_1 2^n+c_2 n 2^n$ ，
因 $f(n)=(1+n) 2^n$ 且特徵根有 2 ，
故令特殊解 $a_n^{(p)}=\left(d_0+d_1 n\right) 2^n \times n^2=d_0 n^2 2^n+d_1 n^3 2^n$ ，
代回原式得 $\left(d_0 n^2 2^n+d_1 n^3 2^n\right)-4\left(d_0(n-1)^2 2^{n-1}+d_1(n-1)^3 2^{n-1}\right)$
$$
+4\left(d_0(n-2)^2 2^{n-2}+d_1(n-2)^3 2^{n-2}\right)=(n+1) 2^n
$$

同除以 $2^n$ 得
$$
\left(d_0 n^2+d_1 n^3\right)-2\left(d_0(n-1)^2+d_1(n-1)^3\right)+\left(d_0(n-2)^2+d_1(n-2)^3\right)=(n+1)
$$

整理得 $6 d_1 n+2 d_0-6 d_1=n+1$ ，
比較係數得 $\left\{\begin{array}{l}6 d_1=1 \\ 2 d_0-6 d_1=1\end{array}, \therefore d_1=\frac{1}{6}, d_0=1, a_n^{(p)}=n^2 2^n+\frac{1}{6} n^3 2^n\right.$ ，
故 $a_n=c_1 2^n+c_2 n 2^n+n^2 2^n+\frac{1}{6} n^3 2^n$ ，
再由初值條件 $\left\{\begin{array}{l}a_0=1=c_1 \\ a_1=\frac{19}{3}=2 c_1+2 c_2+2+\frac{2}{6}\end{array} \therefore c_1=c_2=1\right.$ ，
得 $a_n=2^n+n 2^n+n^2 2^n+\frac{1}{6} n^3 2^n, n \geq 0$ ．