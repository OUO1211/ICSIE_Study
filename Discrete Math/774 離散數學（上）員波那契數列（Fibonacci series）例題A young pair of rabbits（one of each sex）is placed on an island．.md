774 離散數學（上）

員波那契數列（Fibonacci series）
例題
A young pair of rabbits（one of each sex）is placed on an island．A pair of rabbits does not breed until they are two months old．After they are 2 months old，each pair of rabbits produces another pair each month．Assume that no rabbits ever die．Then the recurrence equation for the number of pairs of rabbits on the island after $n$ months is：$\left\{\begin{array}{l}F_n=F_{n-1}+F_{n-2}, n \geq 2 \\ F_0=0, F_1=1\end{array} \quad\right.$ 【很重要】

解（1）列遞迴式：
設第 $n$ 個月的兔子有 $F_n$ 對，明顯可得，$F_0=0, F_1=1, F_2=1$ ，對其他的 $n$ ，在免子不死下，前一月的兔子（有 $F_{n-1}$ 對）繼續在本月出現，
而二月前的兔子在本月均做出貢獻（新生了 $F_{n-2}$ 對），故得 $F_n=F_{n-1}+F_{n-2}$ ，
故得遞迴式：$\left\{\begin{array}{l}F_0=0, F_1=1 \\ F_n=F_{n-1}+F_{n-2}, n \geq 2\end{array}\right.$ 。
（2）以特徵函數法解：
其特徵式為 $\alpha^2-\alpha-1=0$ ，特徵根為：$\alpha_1=\frac{1+\sqrt{5}}{2}, \alpha_2=\frac{1-\sqrt{5}}{2}$ ，
設 $F_n=c_1\left(\frac{1+\sqrt{5}}{2}\right)^n+c_2\left(\frac{1-\sqrt{5}}{2}\right)^n$ ，由初值條件 $\left\{\begin{array}{l}0=F_0=c_1+c_2 \\ 1=F_1=c_1\left(\frac{1+\sqrt{5}}{2}\right)+c_2\left(\frac{1-\sqrt{5}}{2}\right)\end{array}\right.$ ，
解聯立得 $c_1=\frac{1}{\sqrt{5}}, c_2=-\frac{1}{\sqrt{5}}$ ，
故得通解 $F_n=\frac{1}{\sqrt{5}}\left(\left(\frac{1+\sqrt{5}}{2}\right)^n-\left(\frac{1-\sqrt{5}}{2}\right)^n\right), n \geq 0$ 。
（3）生成函數法解：
【84 清大資科】【89、91 中山資エ】【 103 中央資エ】
原式等於 $F_n-F_{n-1}-F_{n-2}=0, \therefore \sum_{n=2}^{\infty} F_n x^n-\sum_{n=2}^{\infty} F_{n-1} x^n-\sum_{n=2}^{\infty} F_{n-2} x^n=0$
令 $A(x)=\sum_{n=0}^{\infty} F_n x^n$ ，
則原式成為 $\left(A(x)-F_0-F_1 x\right)-x \sum_{n-1=1}^{\infty} F_{n-1} x^{n-1}-x^2 \sum_{n-2=0}^{\infty} F_{n-2} x^{n-2}=0$ ，