第 7 章 內積空間 321

正交投影算子（orthogonal projection operator）
考虑向量空間 $V_F$ 上的子空間 $W$ ，定義函数 $P: V \rightarrow V$ 為 $P(\boldsymbol{v})=p r o j_W \boldsymbol{v}, \forall \boldsymbol{v} \in V$ ，
則稱 $P$ 為 $V$ 在 $W$ 上的正交投影算子。
（1）若 $\left\{\boldsymbol{v}_1, \ldots, \boldsymbol{v}_k\right\}$ 為 $V$ 的子空間 $W$ 的一組正交基底，則
【95中正資工】 $\forall \boldsymbol{v} \in V$ ，定義 $P(\boldsymbol{v})=\sum_{i=1}^k \frac{\left\langle\boldsymbol{v}, \boldsymbol{v}_i\right\rangle}{\left\langle\boldsymbol{v}_i, \boldsymbol{v}_i\right\rangle} \boldsymbol{v}_i$ ，則 $P: V \rightarrow V$ 為一 $W$ 上之正交投影算子．
（2）若 $W=C S(A)$ 為 $V$ 的子空間且 $A$ 行獨立，
$\forall \boldsymbol{v} \in V$ ，定義 $P(\boldsymbol{v})=A\left(A^H A\right)^{-1} A^H \boldsymbol{v}$ ，則 $P: V \rightarrow V$ 為一 $W$ 上之正交投影算子．
（3）$P$ 為一線性映射。

【95中正資工】

【證明】
$$
\forall \alpha \in F, \boldsymbol{u}, \boldsymbol{v} \in V \text {, 令 } P(\boldsymbol{u})=\boldsymbol{u}_0, P(\boldsymbol{v})=\boldsymbol{v}_0 \text {, 即 }\left\langle\boldsymbol{u}-\boldsymbol{u}_0, \boldsymbol{w}\right\rangle=\left\langle\boldsymbol{v}-\boldsymbol{v}_0, \boldsymbol{w}\right\rangle=0, \forall \boldsymbol{w} \in W \text {, }
$$

欲證 $P$ 為一線性映射，即欲證明：$P(\alpha \boldsymbol{u}+\boldsymbol{v})=\alpha P(\boldsymbol{u})+P(\boldsymbol{v})$ ．
因 $W \subseteq V, \therefore \alpha \boldsymbol{u}_0+\boldsymbol{v}_0 \in W$ ，
則 $\left\langle(\alpha \boldsymbol{u}+\boldsymbol{v})-\left(\alpha \boldsymbol{u}_0+\boldsymbol{v}_0\right), \boldsymbol{w}\right\rangle=\alpha\left\langle\boldsymbol{u}-\boldsymbol{u}_0, \boldsymbol{w}\right\rangle+\left\langle\boldsymbol{v}-\boldsymbol{v}_0, \boldsymbol{w}\right\rangle=0+0=0, \forall \boldsymbol{w} \in W$,
即 $P(\alpha \boldsymbol{u}+\boldsymbol{v})=\left(\alpha \boldsymbol{u}_0+\boldsymbol{v}_0\right)$ ，故得 $P(\alpha \boldsymbol{u}+\boldsymbol{v})=\alpha P(\boldsymbol{u})+P(\boldsymbol{v})$ ．
（4） $\operatorname{Im}(P)=W$ ．
【證明】
由 $P(\boldsymbol{v})$ 的定義明顯可得 $\operatorname{Im}(P) \subseteq W$ ，
又 $\because \forall \boldsymbol{v} \in W, \boldsymbol{v}=P(\boldsymbol{v}) \in \operatorname{Im}(P)$ ，故 $W \subseteq \operatorname{Im}(P)$ ，
故 $\operatorname{Im}(P)=W$ ．
（5）$P^2=P$ ．

【95中正資工】

【證明】
$\because \forall v \in V, P(v) \in W$（由 $P$ 的定義可得），
且 $\forall v \in W, P(v)=v$（因為 $v-v$ 與 $W$ 上的任意向量正交，$\therefore P(v)=v$ ），
$$
\therefore P(P(\boldsymbol{v}))=P(\boldsymbol{v}), \therefore P^2=P .
$$