424
離散數學（上）

排列（permutation）
從 $n$ 件相異物，不允許重覆，取 $r$ 件排列的方法數為
$$
n \times(n-1) \times(n-2) \times \ldots \times(n-r+1)=\frac{n!}{(n-r)!}=P_r^n=P(n, r), \quad n \geq r .
$$

例如：
由兩個英文字母後接 4 個數字所構成的小客車執照，有 $26^2 \times 10^4$ 種不同的執照；又若兩英文字母必須相異，則有 $26 \times 25 \times 10^4$ 種。
Note
（1） $0!=1 ; \quad n!\approx \sqrt{2 \pi n} \times\left(\frac{n}{e}\right)^n$ ．（Stirling＇s approximation）

【91 台大資エ】

（2）排列的組合應用：考慮兩集合 $A 、 B,|A|=m,|B|=n$ ，則由 $A$ 至 $B$ 的一對一函數有 $P_m^n$個。

【91 台大資エ】

例題
（1）How many integers from 1 to 1000 do not have any repeated digits（e．g．，both 999 and 858 have repeated digits．）？
（2）What is the probability that an integer chosen at random from 1 through 1000 has at least one repeated digit？
解（1）只有個位數且數字不同的有 9 個，有兩位數且數字不同的有 9.9 個（因首不為 0 ），有三位數且數字不同的有 $9 \cdot 9 \cdot 8$ 個（因首不為 0 ），所以共有 $9+81+648=738^{\circ}$
（2） 1 到 1000 個數中，有重複數字的有 $1000-738=262$ ，故機率為 $\frac{262}{1000}$ 。