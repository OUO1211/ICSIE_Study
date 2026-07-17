598
離散數學（上）

求係數

例題
Find the coefficient of
（1）$x^9$ in $\frac{1}{1+3 x}$ ．

【106清大資工】

（2）$x^{50}$ in $\left(x^7+x^8+x^9+\cdots\right)^6$ ．
【99、103 中山資工類題】【97 成大資工】
（3）$x^{83}$ in $\left(x^5+x^8+x^{11}+x^{14}+x^{17}\right)^{10}$ ．
（4）$x^7$ in $\frac{x^2-3 x}{(1-x)^5}+3 x^7+5$ ．
【95師大資工類題】【97、107中山資工】

解（1）$\frac{1}{1+3 x}=\sum_{i=0}^{\infty}(-3 x)^i$ ，
$\therefore x^9$ 的係數是 $(-3)^9$ 。
（2）$\left(x^7+x^8+x^9 \cdots\right)^6=x^{42}\left(1+x+x^2+\cdots\right)^6=x^{42}(1-x)^{-6}$
$=x^{42} \sum_{i=0}^{\infty}\binom{-6}{i}(-x)^i=x^{42} \sum_{i=0}^{\infty}\binom{5+i}{i} x^i$ ，取 $i=8$ ，得 $x^{50}$ 係數 $\binom{13}{8}$ 。
（3）$\left(x^5+x^8+x^{11}+x^{14}+x^{17}\right)^{10}=x^{50}\left(1+x^3+x^6+x^9+x^{12}\right)^{10}=x^{50}\left(\frac{1-x^{15}}{1-x^3}\right)^{10}$
$=x^{50}\left(1-x^{15}\right)^{10}\left(1-x^3\right)^{-10}=x^{50} \times \sum_{i=0}^{10}\binom{10}{i}\left(-x^{15}\right)^i \times \sum_{j=0}^{\infty}\binom{-10}{j}\left(-x^3\right)^j$,
$=x^{50} \times \sum_{i=0}^{10}\binom{10}{i}\left(-x^{15}\right)^i \times \sum_{j=0}^{\infty}\binom{9+j}{j} x^{3 j}$,
在 $i=0, j=11 ; i=1, j=6 ; i=2, j=1$ 均得 $x^{83}$ 係數，
共 $\binom{10}{0}\binom{20}{11}-\binom{10}{1}\binom{15}{6}+\binom{10}{2}\binom{10}{1}$ 。
（4）$\frac{x^2-3 x}{(1-x)^5}+3 x^7+5=\left(x^2-3 x\right) \sum_{k=0}^{\infty}\binom{-5}{k}(-x)^k+3 x^7+5$
$=x^2 \sum_{k=0}^{\infty}\binom{5+k-1}{k} x^k-3 x \sum_{k=0}^{\infty}\binom{5+k-1}{k} x^k+3 x^7+5$ ，
分別取 $k=5,6$ 得 $x^7$ 的係數為 $\binom{9}{5}-3\binom{10}{6}+3$ 。