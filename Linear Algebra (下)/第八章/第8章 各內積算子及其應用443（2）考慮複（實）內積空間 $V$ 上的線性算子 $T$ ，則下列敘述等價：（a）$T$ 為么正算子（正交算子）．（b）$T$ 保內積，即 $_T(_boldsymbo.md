第8章 各內積算子及其應用
443

（2）考慮複（實）內積空間 $V$ 上的線性算子 $T$ ，則下列敘述等價：
（a）$T$ 為么正算子（正交算子）．
（b）$T$ 保內積，即 $<T(\boldsymbol{u}), T(\boldsymbol{v})>=<\boldsymbol{u}, \boldsymbol{v}>, \forall \boldsymbol{u}, \boldsymbol{v} \in V$ 。
（c）$T$ 保長度，即 $\|T(\boldsymbol{v})\|=\|\boldsymbol{v}\|, \forall \boldsymbol{v} \in V$ ．

【91成大應數】

【證明】
（a）⇒（b）
設 $T$ 為么正算子，則
$\forall \boldsymbol{u}, \boldsymbol{v} \in V,<T(\boldsymbol{u}), T(\boldsymbol{v})>=<T^* T(\boldsymbol{u}), \boldsymbol{v}>=<I(\boldsymbol{u}), \boldsymbol{v}>=<\boldsymbol{u}, \boldsymbol{v}>$ ，即 $T$ 保內積。
（b）⇒（c）
設 $T$ 保內積，則
$\forall \boldsymbol{v} \in V,\|T(\boldsymbol{v})\|^2=<T(\boldsymbol{v}), T(\boldsymbol{v})>=<\boldsymbol{v}, \boldsymbol{v}>=\|\boldsymbol{v}\|^2, \therefore\|T(\boldsymbol{v})\|=\|\boldsymbol{v}\|$ ，即 $T$ 保長度．
（c）⇒（a）
設 $T$ 保長度，則
$$
\forall v \in V,\langle v, v\rangle=\|v\|^2=\|T(v)\|^2=\langle T(v), T(v)\rangle=\left\langle T^* T(v), v\right\rangle,
$$
$\therefore \forall v \in V, T^* T(v)=v$ ，即 $T^* T=I$ ，即 $T$ 為么正算子．
（3）由保內積與保長度可得：
$T$ 為么正算子⇔若 $\beta$ 為 $V$ 的一單範正交基底，則 $T(\beta)$ 亦為 $V$ 的一單範正交基底．
（4）因為保內積與保長度，故也會保角度，保正交，保單範正交．