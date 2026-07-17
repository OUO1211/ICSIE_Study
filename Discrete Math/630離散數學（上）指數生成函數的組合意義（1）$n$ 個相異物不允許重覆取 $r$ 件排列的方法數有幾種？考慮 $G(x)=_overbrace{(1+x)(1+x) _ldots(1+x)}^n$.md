630
離散數學（上）

指數生成函數的組合意義
（1）$n$ 個相異物不允許重覆取 $r$ 件排列的方法數有幾種？
考慮 $G(x)=\overbrace{(1+x)(1+x) \ldots(1+x)}^n$ 中 $x^r$ 之係數，設為 $S$ ，則相當於從 $n$ 個相異物 $(n$ 項），每物皆不可重複拿，共取 $r$ 個的方法數，而每次拿出 $r$ 個後，又有 $r!$ 個不同的排列方式，故原問題有 $S \cdot r!$ 種方法，但此數亦即為 $G(x)=(1+x)^n=\sum_{i=0}^n\binom{n}{i} x^i=\sum_{i=0}^n \frac{n!}{(n-i)!} \cdot \frac{x^i}{i!}$ 中 $\frac{x^r}{r!}$之係數，取 $i=r$ 得 $\frac{x^r}{r!}$ 之係數 $=\frac{n!}{(n-r)!}=P_r^n$ 。
（2）$n$ 個相異物允許重覆取 $r$ 件排列的方法數有幾種？
同上例的討論，得原問題即為
$G(x)=\overbrace{\left(1+\frac{x}{1!}+\frac{x^2}{2!}+\cdots\right)\left(1+\frac{x}{1!}+\frac{x^2}{2!}+\cdots\right) \cdots\left(1+\frac{x}{1!}+\frac{x^2}{2!}+\cdots\right)}^{n \text { 項 }}$ 中 $\frac{x^r}{r!}$ 之係數 ，
而 $G(x)=\left(e^x\right)^n=e^{n x}=\sum_{i=0}^{\infty} \frac{(n x)^i}{i!}$ ，取 $i=r$ 得 $\frac{x^r}{r!}$ 之係數 $=n^r$ 。
Note
此處之每個括弧寫成 $1+\frac{x}{1!}+\frac{x^2}{2!}+\cdots$ ，而非 $1+x+x^2+\cdots$ 的原因是：
$\frac{x^r}{r!}$ 之係數是由各括弧中的係數對乘再加總而得，故在探討此排列型問題時亦應為由各括弧中的排列型係數對乘再去加總。
（3）$m$ 個相異物放入 $n$ 個相異箱不允許有空箱的方法數有幾種？
即 $G(x)=\overbrace{\left(\frac{x}{1!}+\frac{x^2}{2!}+\cdots\right)\left(\frac{x}{1!}+\frac{x^2}{2!}+\cdots\right) \cdots\left(\frac{x}{1!}+\frac{x^2}{2!}+\cdots\right)}^{n \text { 項 }}$ 中 $\frac{x^m}{m!}$ 之係數 ，
而 $G(x)=\left(e^x-1\right)^n=\sum_{i=0}^n\binom{n}{i}(-1)^i\left(e^x\right)^{n-i}=\sum_{i=0}^n(-1)^i\binom{n}{i} e^{(n-i) x}=\sum_{i=0}^n(-1)^i\binom{n}{i} \sum_{j=0}^{\infty} \frac{(n-i)^{\prime} x^j}{j!}$ ；
取 $j=m$ 得 $\frac{x^m}{m!}$ 之係數 $=\sum_{i=0}^n(-1)^i\binom{n}{i}(n-i)^m$ 。