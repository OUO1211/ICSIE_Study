第4章 數學歸納法與數論
353

整係數方程式問題
整係数方程式 $a x+b y=c$ 有整数解 $\Leftrightarrow \operatorname{gcd}(a, b) \mid c$ ，
且若解存在，其解集合為 $S=\left\{(x, y) \left\lvert\, x=x_0+\frac{b}{d} k\right., y=y_0-\frac{a}{d} k, k \in Z\right\}$ ，
其中 $\left(x_0, y_0\right)$ 為 $a x+b y=c$ 之一解，$d=\operatorname{gcd}(a, b)$ 。
Note
$a x+b y=c$ 又稱 Diophantine equation。
【證明】
（⇒）
設 $\left(x_0, y_0\right)$ 為 $a x+b y=c$ 之一組整數解，即 $a x_0+b y_0=c$ ，
令 $d=\operatorname{gcd}(a, b)$ ，則存在整數 $u, v$ ，使 $a=u d, b=v d$ ，
$\therefore c=a x_0+b y_0=u d x_0+v d y_0=d\left(u x_0+v y_0\right)$ ，得 $d \mid c$ 。
$(\Leftarrow)$
若 $d=\operatorname{gcd}(a, b) \mid c$ ，即存在整數 $k$ ，使 $c=d k$ ，
因為 $d=\operatorname{gcd}(a, b)=\min \{a s+b t \mid s, t \in Z$ ，and $a s+b t>0\}$ ，
∴ 存在整數 $u, v$ ，使 $d=a u+b v$ ，
$\therefore c=d k=(a u+b v) k=a(u k)+b(v k)$
即找到 $a x+b y=c$ 的一組整數解 $x=u k, ~ y=v k 。$
另外，對 $a x+b y=c$ 的解集合的描述 ：
很明顯，$S$ 中的元素均為 $a x+b y=c$ 的解。
反之，由 $a x+b y=c$ 與 $a x_0+b y_0=c$ 可得 $a\left(x-x_0\right)+b\left(y-y_0\right)=0$ ，即 $\frac{-\left(x-x_0\right)}{b}=\frac{y-y_0}{a}$ ，
令 $d=\operatorname{gcd}(a, b)$ ，且 $a=d s, b=d r$ ，其中 $s, r$ 為互質整數，
$\therefore y-y_0=-\frac{a\left(x-x_0\right)}{b}=-\frac{s\left(x-x_0\right)}{r} \in Z$ ，
又因 $r, s$ 互質，故 $\frac{x-x_0}{r}$ 為一整數（設為 $-k$ ），同理可得，$\frac{y-y_0}{s}$ 亦為一整數 $(k)$ ，
所以 $x=x_0-\frac{b}{d} \times \frac{y-y_0}{s}=x_0+\frac{b}{d} k, y=y_0-\frac{a}{d} \times \frac{x-x_0}{r}=y_0-\frac{a}{d} k$ 為 $a x+b y=c$ 的一般解。