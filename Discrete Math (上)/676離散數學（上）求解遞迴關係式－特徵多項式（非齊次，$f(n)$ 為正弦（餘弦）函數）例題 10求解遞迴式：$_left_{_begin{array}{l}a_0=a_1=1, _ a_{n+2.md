676
離散數學（上）

求解遞迴關係式－特徵多項式（非齊次，$f(n)$ 為正弦（餘弦）函數）
例題 10
求解遞迴式：$\left\{\begin{array}{l}a_0=a_1=1, \\ a_{n+2}-a_n=\sin \left(\frac{n \pi}{2}\right), n \geq 0\end{array}\right.$ ．
【 $84 、 95$ 成大電機】

解 特徴式為 $\alpha^2-1=0$ ，得特徵根為 $1,-1$ ，
故設齊次解為 $a_n^{(h)}=c_1 1^n+c_2(-1)^n$ ，
令特殊解 $a_n^{(p)}=d_1 \cos \left(\frac{n \pi}{2}\right)+d_2 \sin \left(\frac{n \pi}{2}\right)$ ，
代回原式得 $d_1 \cos \left(\frac{(n+2) \pi}{2}\right)+d_2 \sin \left(\frac{(n+2) \pi}{2}\right)-d_1 \cos \left(\frac{n \pi}{2}\right)-d_2 \sin \left(\frac{n \pi}{2}\right)=\sin \left(\frac{n \pi}{2}\right)$ ，
整理得 $-d_1 \cos \left(\frac{n \pi}{2}\right)-d_2 \sin \left(\frac{n \pi}{2}\right)-d_1 \cos \left(\frac{n \pi}{2}\right)-d_2 \sin \left(\frac{n \pi}{2}\right)=\sin \left(\frac{n \pi}{2}\right)$ ，
即 $-2 d_1=0,-2 d_2=1$ ，得 $d_1=0, d_2=\frac{-1}{2}$ ，
$\therefore a_n^{(p)}=\frac{-1}{2} \sin \left(\frac{n \pi}{2}\right)$ ，
故 $a_n=c_1+c_2(-1)^n+\frac{-1}{2} \sin \left(\frac{n \pi}{2}\right)$ ，
再由初值條件 $\left\{\begin{array}{l}a_0=1=c_1+c_2 \\ a_1=1=c_1-c_2-\frac{1}{2}\end{array}\right.$ ，解得 $c_1=\frac{5}{4}, c_2=\frac{-1}{4}$ ，
得 $a_n=\frac{5}{4}-\frac{1}{4} \cdot(-1)^n-\frac{1}{2} \sin \left(\frac{n \pi}{2}\right), n \geq 0$ 。