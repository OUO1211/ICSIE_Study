358
線性代數（下）

正交補空間上的投影
考虑內積空間 $V$ 上的子空間 $W$ ，令 $P$ 為 $W$ 上的正交投影算子，則
（1） $\operatorname{ker}(P)=W^{\perp}$ ．
（2） proj $_{W^{\perp}} \nu=\nu-P(\nu)$ ．
（3）$I-P$ 為 $V$ 在 $W^{\perp}$ 上的正交投影算子．
【證明】
（1） $\boldsymbol{v} \in \operatorname{ker}(P) \Leftrightarrow P(\boldsymbol{v})=\mathbf{0} \Leftrightarrow \operatorname{proj}_W \boldsymbol{v}=\mathbf{0} \Leftrightarrow \boldsymbol{v} \perp W \Leftrightarrow \boldsymbol{v} \in W^{\perp}$ ．
（2）$\because P(\boldsymbol{v}-P(\boldsymbol{v}))=P(\boldsymbol{v})-P^2(\boldsymbol{v})=P(\boldsymbol{v})-P(\boldsymbol{v})=\mathbf{0}$ ，故 $\boldsymbol{v}-P(\boldsymbol{v}) \in \operatorname{ker}(P)=W^{\perp}$ ，
$$
\therefore \forall \boldsymbol{w} \in W^{\perp},\langle\boldsymbol{v}-(\boldsymbol{v}-P(\boldsymbol{v})), \boldsymbol{w}\rangle=\langle P(\boldsymbol{v}), \boldsymbol{w}\rangle=0,(\because P(\boldsymbol{v}) \in W)
$$
$\therefore(\boldsymbol{v}-P(\boldsymbol{v}))$ 為 $\boldsymbol{v}$ 在 $W^{\perp}$ 上的正交投影向量．
（3）由（2）可得 $\operatorname{proj}_{W^{\perp}} v=v-P(v)=(I-P)(v), \forall v \in V$ 。