350
線性代數（下）

7－4 正交補空間

正交補空間（orthogonal complement space）
考慮內積空間 $V$ 的一子集 $S$ ，
定義 $S^{\perp}=\{\boldsymbol{v} \in V \mid<\boldsymbol{v}, \boldsymbol{u}>=0, \forall \boldsymbol{u} \in S\}$ ，稱作 $S$ 的正交補空間。
【108政大統計】
例如取 $V=R^2$ ，
$S=\{(1,0)\}$ ，則 $S^{\perp}=\{(0, y) \mid y \in R\} ;$
$W=\{(x, 0) \mid x \in R\}$ ，則 $W^{\perp}=\{(0, y) \mid y \in R\}$ ．

Note
（1）$\{\boldsymbol{0}\}^{\perp}=V, V^{\perp}=\{\boldsymbol{0}\}$ ．
（2）對任意向量集 $S$ ：
（a） $\mathbf{0} \in S^{\perp}$ ．
（b）$S \cap S^{\perp}=\left\{\begin{array}{ll}\{\mathbf{0}\} & \text { if } \mathbf{0} \in S \\ \varnothing & \text { if } \mathbf{0} \notin S\end{array}\right.$ ．
（c）$S^{\perp}$ 為 $V$ 的一個子空間．
【證明】
【89．91．102．103 中央資工、98 彰師數學、102 中正數學】
明顯可得 $S^{\perp}$ 為 $V$ 的子集合，且非空，（因 $\mathbf{0} \in S^{\perp}$ ）
$\forall \alpha, \forall \boldsymbol{u}, \boldsymbol{v} \in S^{\perp},\langle\alpha \boldsymbol{u}+\boldsymbol{v}, \boldsymbol{s}\rangle=\alpha\langle\boldsymbol{u}, \boldsymbol{s}\rangle+\langle\boldsymbol{v}, \boldsymbol{s}\rangle=0+0=0, \forall \boldsymbol{s} \in S$ ，
$\therefore \alpha \boldsymbol{u}+\boldsymbol{v} \in S^{\perp}, \therefore S^{\perp}$ 為 $V$ 的一個子空間．
（d）$S \subseteq S^{\perp \perp}$ ．
【證明】
$$
\forall \boldsymbol{s} \in S,\langle\boldsymbol{v}, \boldsymbol{s}\rangle=0, \forall \boldsymbol{v} \in S^{\perp},
$$

故 $\boldsymbol{s}$ 與 $S^{\perp}$ 中的向量都正交，故 $\boldsymbol{s}$ 屬於 $S^{\perp}$ 的正交補空間，
即 $\boldsymbol{s} \in\left(S^{\perp}\right)^{\perp}$ ，故 $S \subseteq S^{\perp \perp}$ 。
（3）考慮內積空間 $V$ ，令 $B=\left\{\boldsymbol{b}_1, \ldots, \boldsymbol{b}_k\right\}$ 為子空間 $W$ 的一組基底，則
$\boldsymbol{v} \in W^{\perp} \Leftrightarrow<\boldsymbol{v}, \boldsymbol{b}_i>=0, \forall i$ ．（由此而得一刻劃正交補空間的一種方法）
【證明】
⇒ 明顯可得．