548
離散數學（上）

項式定理（multi－nomial theorem）
$$
\left(x_1+x_2+\ldots+x_t\right)^n=\sum_{n_1+\ldots+n_t=n} \frac{n!}{n_{1}!n_{2}!\ldots n_{t}!} x_1^{n_1} x_2^{n_2} \ldots x_t^{n_t} .
$$

【81中山資工】

與二項式定理的討論方式相同，觀察各項係數組成的方式，即可得此定理成立。

例題
求特定項的係数：
（1）$x^2 y z^2$ in $[(x / 2)+y-3 z]^5$ ．
【101宜蘭資工類題】【101成大資工】
（2）$x^{23}$ in $\left(1+x^5+x^9\right)^{100}$ ．
【86 台大資工】【94 政大資科】【101 資訊技師】
（3）$x^2 y^3$ in $(x-2 y+3 z-4 / z+5)^{16}$ ．
【102台大工科】
解（1）$\left(\frac{x}{2}+y-3 z\right)^5=\sum_{a+b+c=5} \frac{5!}{a!b!c!}\left(\frac{x}{2}\right)^a y^b(-3 z)^c$ ，
取 $a=2, b=1, c=2$ ，
得 $x^2 y z^2$ 之係數為：$\frac{5!}{2!\cdot 1!\cdot 2!} \cdot\left(\frac{1}{2}\right)^2 \cdot(-3)^2$ 。
（2）$\left(1+x^5+x^9\right)^{100}=\sum_{a+b+c=100} \frac{100!}{a!b!c!} \cdot 1^a \cdot x^{5 b} \cdot x^{9 c}$ ，
由 $5 b+9 c=23$ 得知，須 $b=1, c=2, a=97$ ，故得係數為 $\frac{100!}{1!2!97!}$ 。
（3）展開式中，$(x-2 y)^5 \cdot\left(3 z-\frac{4}{z}+5\right)^{11}$ 的係數是 $\binom{16}{5}$ ，且 $(x-2 y)^5$ 中 $x^2 y^3$ 的係數是 $\binom{5}{2}(-2)^3$ ，
$\left(3 z-\frac{4}{z}+5\right)^{11}$ 的常數項為 $\sum_{i=0}^5 \frac{11!}{i!i!(11-2 i)!} 3^i(-4)^i 5^{11-2 i}$ ，
故原式中 $x^2 y^3$ 之係數為：
$$
\binom{16}{5} \times\binom{ 5}{2}(-2)^3 \times \sum_{i=0}^5 \frac{11!}{i!i!(11-2 i)!} 3^i(-4)^i 5^{11-2 i}
$$