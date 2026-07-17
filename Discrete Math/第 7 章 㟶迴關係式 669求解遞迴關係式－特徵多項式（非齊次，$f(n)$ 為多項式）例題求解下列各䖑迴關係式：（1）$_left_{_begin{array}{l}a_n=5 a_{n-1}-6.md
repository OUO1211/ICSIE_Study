第 7 章 㟶迴關係式 669

求解遞迴關係式－特徵多項式（非齊次，$f(n)$ 為多項式）
例題
求解下列各䖑迴關係式：
（1）$\left\{\begin{array}{l}a_n=5 a_{n-1}-6 a_{n-2}+2 n+1, n \geq 2 \\ a_0=5, a_1=6\end{array}\right.$ ．
【＊＊＊＊＊資エ】
（2）$\left\{\begin{array}{l}a_n=4 a_{n-1}-3 a_{n-2}+4, n \geq 3 \\ a_1=-9, a_2=-5\end{array}\right.$ ．
【＊＊＊＊＊資工】
解（1）$a_n-5 a_{n-1}+6 a_{n-2}=0$ 的特徵式為 $\alpha^2-5 \alpha+6=(\alpha-2)(\alpha-3)=0$ ，
得特徵根 2,3 ，設 $a_n^{(h)}=c_1 2^n+c_2 3^n$ ，
因 $f(n)=2 n+1$ 為一次多項式，故令 $a_n^{(p)}=s n+t$ ，並代回原式得 ：
$$
(s n+t)-5(s(n-1)+t)+6(s(n-2)+t))=2 n+1,
$$

代入 $n=2$ ，得 $2 s+t-5 s-5 t+6 t=5$ ，
代入 $n=1$ ，得 $s+t-5 t-6 s+6 t=3$ ，
整理得 $\left\{\begin{array}{l}-3 s+2 t=5 \\ -5 s+2 t=3\end{array}\right.$ ，解得 $s=1, t=4, \therefore a_n^{(p)}=n+4$ ，
故 $a_n=a_n^{(h)}+a_n^{(p)}=c_1 2^n+c_2 3^n+n+4$ ，
又由 $\left\{\begin{array}{l}a_0=c_1+c_2+4=5 \\ a_1=2 c_1+3 c_2+5=6\end{array}\right.$, 可得 $c_1=2, c_2=-1$ ，
故 $a_n=2^{n+1}-3^n+n+4, n \geq 0$ ．
（2）特徴式為 $\alpha^2-4 \alpha+3=(\alpha-1)(\alpha-3)=0$ ，得特徴根 1，3，
設齊次解為 $a_n^{(h)}=c_1 1^n+c_2 3^n$ ，
因 $f(n)=4$ ，且特徵根有 1 ，故令特殊解 $a_n^{(p)}=c n$ ，並代回原式得：
$$
c n-4 c(n-1)+3 c(n-2)=4,
$$

代入 $n=2$ 得 $2 c-4 c=4$ ，
解得 $c=-2, ~ a_n^{(p)}=-2 n$ ，
故 $a_n=a_n^{(h)}+a_n^{(p)}=c_1+c_2 \cdot 3^n-2 n$ ，
又由 $\left\{\begin{array}{l}a_1=-9=c_1+3 c_2-2 \\ a_2=-5=c_1+9 c_2-4\end{array}\right.$ ，解得 $c_1=-10, c_2=1$ ，
故 $a_n=-10+3^n-2 n, n \geq 1$ 。