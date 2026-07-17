422
線性代數（下）

自伴算子（self－adjoint）與斜自伴算子（skew self－adjoint）
考虑 $V$ 上的線性算子 $T$ ，
若 $T^*=T$ ，則稱 $T$ 為自伴算子．
若 $T^*=-T$ ，則稱 $T$ 為斜自伴算子。
Note
（1）令 $\beta$ 為實內積空間 $V$ 上的一單範正交基底，$T$ 為 $V$ 上的一算子使 $[T]_\beta=A$ ，則
（a）$T$ 為斜自伴算子 $\Leftrightarrow A^T=-A$ ．
【94 成大應數】
【證明】
$\beta=\left\{\boldsymbol{u}_1, \ldots, \boldsymbol{u}_n\right\}$ 為 $V$ 的一單範正交基底使 $A=\left[a_{i j}\right]=[T]_\beta$ ，
則 $T\left(\boldsymbol{u}_i\right)=a_{1 i} \boldsymbol{u}_1+\ldots+a_{n i} \boldsymbol{u}_n$ ，for $i=1 \sim n, a_{i j} \in R$ ，
故 for $i, j \in\{1,2, \ldots, n\}$ ，
$<T\left(\boldsymbol{u}_i\right), \boldsymbol{u}_j>=<a_{1 i} \boldsymbol{u}_1+\ldots+a_{n i} \boldsymbol{u}_n, \boldsymbol{u}_j>=<a_{j i} \boldsymbol{u}_j, \boldsymbol{u}_j>=a_{j i}<\boldsymbol{u}_j, \boldsymbol{u}_j>=a_{j i}$,
又 $<T\left(\boldsymbol{u}_i\right), \boldsymbol{u}_j>=-<\boldsymbol{u}_i, T\left(\boldsymbol{u}_j\right)>=-<\boldsymbol{u}_i, a_{1 j} \boldsymbol{u}_1+\ldots+a_{n j} \boldsymbol{u}_n>=-<\boldsymbol{u}_i, a_{i j} \boldsymbol{u}_i>=-a_{i j}$ ，
得 $A^T=-A$ ．
反之，設 $A^T=-A$ ，即 $a_{j i}=-a_{i j}$ ，
則可得 $<T\left(\boldsymbol{u}_i\right), \boldsymbol{u}_j>=-<\boldsymbol{u}_i, T\left(\boldsymbol{u}_j\right)>$ ，for $i, j \in\{1,2, \ldots, n\}$ ，
而因 $\left\{\boldsymbol{u}_1, \ldots, \boldsymbol{u}_n\right\}$ 為 $V$ 的一單範正交基底，故 $\langle T(\boldsymbol{x}), \boldsymbol{y}\rangle=-<\boldsymbol{x}, T(\boldsymbol{y})>$ 。
（b）$T$ 為自伴算子 $\Leftrightarrow A^T=A$ ．
【97彰師數學】
【證明】請讀者仿造（a）的證明技巧自行練習．
（2）若 $T, U$ 為自伴算子，則
$T U$ 為自伴算子 $\Leftrightarrow U T=T U$.
【證明】
$\Rightarrow \because T U, T, U$ 為自伴算子，$\therefore(T U)^*=T U, T^*=T, U^*=U$ ，
$\therefore T U=(T U)^*=U^* T^*=U T$ ．
$\Leftarrow \because T U=U T, \therefore(T U)^*=(U T)^*=T^* U^*=T U, \therefore T U$ 為自伴算子．
（3）若 $T$ 為斜自伴，且子空間 $W$ 為 $T$ 不變，則 $W^{\perp}$ 亦為 $T$ 不變．
【94成大應數】
【證明】（若 $T$ 為自伴時，本性質亦成立．）
【97彰師數學】
設 $T(\boldsymbol{v}) \in T\left(W^{\perp}\right)$ ，即 $\boldsymbol{v} \in W^{\perp}$ ，
$\forall \boldsymbol{w} \in W$ ，因為 $W$ 為 $T-$ 不變子空間，$\therefore T(\boldsymbol{w}) \in W, \therefore\langle\boldsymbol{v}, T(\boldsymbol{w})\rangle=0$ ，
又 $\langle\boldsymbol{v}, T(\boldsymbol{w})\rangle=-\langle T(\boldsymbol{v}), \boldsymbol{w}\rangle, \therefore\langle T(\boldsymbol{v}), \boldsymbol{w}\rangle=0$ ，
$\therefore T(\boldsymbol{v}) \in W^{\perp}, \therefore T\left(W^{\perp}\right) \subseteq W^{\perp}$ ．