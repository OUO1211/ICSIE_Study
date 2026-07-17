610
離散數學（上）

生成函數的組合意義
（1）$n$ 種相異物允許重覆取 $r$ 件組合的方法數

【 87 、 89 中山電機】【 100 清大資工】

考慮 $G(x)=\overbrace{\left(1+x+x^2+\ldots\right)\left(1+x+x^2+\ldots\right) \ldots\left(1+x+x^2+\ldots\right)}^{n \text { 項 }}$ 中 $x^r$ 之係數，
則相當於從 $n$ 種相異物（ $n$ 項），每種皆可重複拿（拿幾個就是次數多少），
總共取 $r$ 個的方法數，
而 $G(x)=\left(\frac{1}{1-x}\right)^n=(1-x)^{-n}=\sum_{i=0}^{\infty}\binom{-n}{i}(-x)^i$ ，
取 $i=r$ 得 $x^r$ 之係數 $=\binom{-n}{r}(-1)^r=\binom{n+r-1}{r}$ 。
（2）$n$ 個相異物不允許重覆取 $r$ 件組合的方法數
考慮 $G(x)=\overbrace{(1+x)(1+x) \ldots(1+x)}^{n \text { 項 }}$ 中 $x^r$ 之係數，
則相當於從 $n$ 個相異物（ $n$ 項），每物皆不可重複拿（即頂多一個），
總共取 $r$ 個方法數，
而 $G(x)=(1+x)^n=\sum_{i=0}^{\infty}\binom{n}{i} x^i$ ，
取 $i=r$ 得 $x^r$ 之係數 $=\binom{n}{r}$ 。
（3）$r$ 個相同球放入 $n$ 個相異箱不允許空箱的方法數
考慮 $G(x)=\overbrace{\left(x+x^2+\ldots\right)\left(x+x^2+\ldots\right) \ldots\left(x+x^2+\ldots\right)}^{n \text { 項 }}$ 中 $x^r$ 之係數，
則相當於 $n$ 個相異箱（ $n$ 項），每箱皆不可空（即至少一個），
總共放了 $r$ 個相同球的方法數，
而 $G(x)=\left(\frac{x}{1-x}\right)^n=x^n(1-x)^{-n}=x^n \sum_{i=0}^{\infty}\binom{-n}{i}(-x)^i$ ，
取 $i=r-n$ ，得 $x^r$ 之係數 $=\binom{-n}{r-n}(-1)^{r-n}=\binom{r-1}{r-n}$ 。