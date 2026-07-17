364
線性代數（下）

正交補空間與直和分解
令 $W$ 是一有限维內積空間 $V$ 的一個子空間，則
（1）$V=W \oplus W^{\perp}$ ．
（2）$\left(W^{\perp}\right)^{\perp}=W$ 。【103．104 中正應數、108 政大統計、110 政大資科、110 交大資工】
【證明】
令 $P$ 為 $W$ 上的正交投影算子，
（1）for $\boldsymbol{v} \in V, \because \boldsymbol{v}=P(\boldsymbol{v})+(\boldsymbol{v}-P(\boldsymbol{v}))$ ，且 $P(\boldsymbol{v}) \in W, \boldsymbol{v}-P(\boldsymbol{v}) \in W^{\perp}$ ，故得 $V=W+W^{\perp}$ ，又因 $W \cap W^{\perp}=\{\mathbf{0}\}$ ，故 $V=W \oplus W^{\perp}$ ．
（2）因 $W$ 與 $W^{\perp}$ 都是 $V$ 的子空間，
由（1）可得 $\left\{\begin{array}{c}\operatorname{dim}(V)=\operatorname{dim}(W)+\operatorname{dim}\left(W^{\perp}\right) \\ \operatorname{dim}(V)=\operatorname{dim}\left(W^{\perp}\right)+\operatorname{dim}\left(W^{\perp}\right)\end{array} \therefore \operatorname{dim}(W)=\operatorname{dim}\left(W^{\perp \perp}\right)\right.$ ，
又因 $W \subseteq W^{\perp \perp}$ ，故得 $W=W^{\perp}$ ．

Note
令 $W$ 為內積空間 $V$ 上的一個子空間 $W$ ，則
（1）對 $V$ 中的任意向量 $\boldsymbol{v}$ ，唯一存在 $\boldsymbol{w} \in W, \boldsymbol{u} \in W^{\perp}$ ，使得 $\boldsymbol{v}=\boldsymbol{w}+\boldsymbol{u}$ ．
【證明】

【89．97 中山應數、103 政大統計】

由上方的證明過程可知，取 $\boldsymbol{w}=\operatorname{proj}_W(\boldsymbol{v}) \in W, \boldsymbol{u}=\boldsymbol{v}-\operatorname{proj}_W(\boldsymbol{v}) \in W^{\perp}$ ，可得 $\boldsymbol{v}=\boldsymbol{w}+\boldsymbol{u}$ ，又因 $V=W \oplus W^{\perp}$ ，故此表示法必唯一。
（2） $\operatorname{dim}(V)=\operatorname{dim}(W)+\operatorname{dim}\left(W^{\perp}\right)$ ．

【97台大電機、107中央資工】

（3）需 $\operatorname{dim}(W)<\infty$ 時，$W^{\perp}=W$ ，否則有反例．