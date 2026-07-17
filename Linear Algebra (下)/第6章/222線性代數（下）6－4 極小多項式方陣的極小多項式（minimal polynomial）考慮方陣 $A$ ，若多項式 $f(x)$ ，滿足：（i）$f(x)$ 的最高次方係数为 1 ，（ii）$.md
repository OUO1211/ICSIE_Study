222

線性代數（下）



6－4 極小多項式



方陣的極小多項式（minimal polynomial）

考慮方陣 $A$ ，若多項式 $f(x)$ ，滿足：

（i）$f(x)$ 的最高次方係数为 1 ，

（ii）$f(A)=O$ ，

（iii）若 $g(x)$ 亦滿足 $g(A)=O$ ，則 $\operatorname{deg}(f(x)) \leq \operatorname{deg}(g(x))$ ，

則稱 $f(x)$ 为 $A$ 的極小多項式，亦記成 $f(x)=\min _A(x)$ 。



【94 交大底数】



Note

（1）最高次項係數為一的多項式又稱為首一（monic）多項式。

（2） $\min _A(x)$ 必存在：由 Cayley－Hamilton 定理知 $A$ 的特徵多項式滿足條件（ii），若再調整最高次項係數使其為一（即乘以 -1 的次方），則亦可滿足條件（i）．

（3）極小多項式必唯一。



【94 交大應數】



【證明】

設多項式 $g(x), h(x)$ 都是 $A$ 的極小多項式，

則因 $g, h$ 都滿足條件（iii），故 $\operatorname{deg}(g(x))=\operatorname{deg}(h(x))$ ，

設 $g(x)=h(x) \cdot a+k(x), a$ 為常數， $\operatorname{deg}(k(x))<\operatorname{deg}(h(x))$ ，或 $k(x)=0$ ，

$\because g(x), h(x)$ 最高次項係數都是 1 ，故 $a=1$ ，

又 $O=g(A)=h(A) \cdot 1+k(A)=O+k(A), \therefore k(A)=O$ ，

而調整 $k(x)$ 的最高次項係數後可得一使 $A$ 代入後成為零矩陣，且最高次項係數為 1 ，但次數卻比 $h(x)$ 更小，與 $h(x)$ 是極小多項式矛盾，故得 $k(x)=0$ ，即 $g(x)=h(x)$ 。

（4） $\min _A(x)$ 與 $\operatorname{char}_A(x)$ 的相關性質

（a） $\min _A(x)$ 與 $\operatorname{char}_A(x)$ 有相同根。



【94 交大應數】



【證明】

令非零向量 $\boldsymbol{v}$ 為 $A$ 相對於 $\lambda$ 的特徵向量，（即 $A \boldsymbol{v}=\lambda \boldsymbol{v}$ ，即 $(A-\lambda I) \boldsymbol{v}=\mathbf{0}$ ），令極小多項式 $\min _A(x)=q(x)(x-\lambda)+c, c \in F$ ，

則由 $\min _A(A)=O$ ，得 $O=q(A)(A-\lambda I)+c I$ ，

所以 $O v=[q(A)(A-\lambda I)] v+c I v, \therefore \mathbf{0}=q(A)(A-\lambda I) v+c v=q(A) \mathbf{0}+c v=c v$ ，

但 $\boldsymbol{v} \neq \mathbf{0}$ ，故 $c=0$ ，即 $\min _A(x)=q(x)(x-\lambda)$ ，

即 $\lambda$ 亦為 $\min _A(x)$ 的一根。