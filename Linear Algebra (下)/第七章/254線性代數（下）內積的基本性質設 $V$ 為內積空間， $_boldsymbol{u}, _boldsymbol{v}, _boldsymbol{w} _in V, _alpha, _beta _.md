254
線性代數（下）

內積的基本性質
設 $V$ 為內積空間， $\boldsymbol{u}, \boldsymbol{v}, \boldsymbol{w} \in V, \alpha, \beta \in F, T \in L(V, V)$ ，則
（1）$\langle\boldsymbol{u}, \alpha \boldsymbol{v}\rangle=\bar{\alpha}\langle\boldsymbol{u}, \boldsymbol{v}\rangle$ ．
（2）$\langle\boldsymbol{u}, \alpha \boldsymbol{v}+\beta \boldsymbol{w}\rangle=\bar{\alpha}\langle\boldsymbol{u}, \boldsymbol{v}\rangle+\bar{\beta}\langle\boldsymbol{u}, \boldsymbol{w}\rangle$（共軛右缐性）
（3）$\langle\boldsymbol{\nu}, \mathbf{0}\rangle=\langle\mathbf{0}, \boldsymbol{\nu}\rangle=0$ ．
（4）$\langle\boldsymbol{v}, \boldsymbol{v}\rangle=0 \Leftrightarrow \boldsymbol{v}=\mathbf{0}$ ．
（5）$[\forall v \in V,\langle\boldsymbol{u}, v\rangle=0] \Leftrightarrow \boldsymbol{u}=\mathbf{0}$ ．

【94 台大電信】

（6）$[\forall \boldsymbol{v} \in V,\langle\boldsymbol{u}, \boldsymbol{v}\rangle=\langle\boldsymbol{w}, \boldsymbol{v}\rangle] \Leftrightarrow \boldsymbol{u}=\boldsymbol{w}$ ．
（7）設 $\left\{\boldsymbol{b}_1, \boldsymbol{b}_2, \ldots, \boldsymbol{b}_n\right\}$ 为 $V$ 的一基底， $\boldsymbol{u} \in V$ ，則
$$
\left[<\boldsymbol{u}, \boldsymbol{b}_i>=0, \forall i=1,2, \ldots, n\right] \Leftrightarrow \boldsymbol{u}=\mathbf{0} .
$$
（8）若 $<T(\boldsymbol{u}), \boldsymbol{v}>=0, \forall \boldsymbol{u}, \boldsymbol{v} \in V$ ，則 $T=O$ ．
（9）若 $\langle T(\boldsymbol{v}), \boldsymbol{v}\rangle=0, \forall \boldsymbol{v} \in V$ ，則 $T=O$ ．
【91 成大應数、104 中正應数】
【證明】
（1）$\langle\boldsymbol{u}, \alpha \boldsymbol{v}\rangle=\overline{\langle\alpha \boldsymbol{v}, \boldsymbol{u}\rangle}=\overline{\alpha\langle\boldsymbol{v}, \boldsymbol{u}\rangle}=\bar{\alpha}\langle\boldsymbol{u}, \boldsymbol{v}\rangle$ ．
（2）
$$
\begin{aligned}
\langle\boldsymbol{u}, \alpha \boldsymbol{v}+\beta \boldsymbol{w}\rangle & =\overline{\langle\alpha \boldsymbol{v}+\beta \boldsymbol{w}, \boldsymbol{u}\rangle}=\overline{\alpha\langle\boldsymbol{v}, \boldsymbol{u}\rangle+\beta\langle\boldsymbol{w}, \boldsymbol{u}\rangle} \\
& =\bar{\alpha} \overline{\langle\boldsymbol{v}, \boldsymbol{u}\rangle}+\bar{\beta} \overline{\langle\boldsymbol{w}, \boldsymbol{u}\rangle}=\bar{\alpha}\langle\boldsymbol{u}, \boldsymbol{v}\rangle+\bar{\beta}\langle\boldsymbol{u}, \boldsymbol{w}\rangle
\end{aligned}
$$
（3）$\langle\boldsymbol{v}, \mathbf{0}\rangle=\langle\boldsymbol{v}, \mathbf{0}+\mathbf{0}\rangle=\langle\boldsymbol{v}, \mathbf{0}\rangle+\langle\boldsymbol{v}, \mathbf{0}\rangle$ ，由純量加法的消去性，$\therefore\langle\boldsymbol{v}, \mathbf{0}\rangle=\mathbf{0}$ 。 $\langle\mathbf{0}, \boldsymbol{v}\rangle=\langle\mathbf{0}+\mathbf{0}, \boldsymbol{v}\rangle=\langle\mathbf{0}, \boldsymbol{v}\rangle+\langle\mathbf{0}, \boldsymbol{v}\rangle$ ，由純量加法的消去性，$\therefore\langle\mathbf{0}, \boldsymbol{v}\rangle=0$ ．
（4）設 $\langle\boldsymbol{v}, \boldsymbol{v}\rangle=0$ ，若 $\boldsymbol{v} \neq \mathbf{0}$ ，則由正定性，$\langle\boldsymbol{v}, \boldsymbol{v}\rangle>0$ ，矛盾，故 $\boldsymbol{v}=\mathbf{0}$ ．
設 $\boldsymbol{v}=\mathbf{0}$ ，則 $\langle\boldsymbol{v}, \boldsymbol{v}\rangle=\langle\mathbf{0}, \mathbf{0}\rangle=0$ ．
（因此，有些地方在定義內積時，以＂$\forall v,<v, v>\geq 0$＂當作第三個條件．）
（5）取 $v=u$ ，則 $<u, u>=0$ ，由（4）得 $u=0$ ；反之，若 $u=0$ ，明顯可得 $<u, v>=0, \forall v$ 。
（6）$\because\langle\boldsymbol{u}, \boldsymbol{v}\rangle=\langle\boldsymbol{w}, \boldsymbol{v}\rangle, \forall \boldsymbol{v}, \therefore\langle\boldsymbol{u}, \boldsymbol{v}\rangle-\langle\boldsymbol{w}, \boldsymbol{v}\rangle=0, \therefore\langle\boldsymbol{u}-\boldsymbol{w}, \boldsymbol{v}\rangle=0, \therefore \boldsymbol{u}=\boldsymbol{w}$ ，by（5）
反之，若 $\boldsymbol{u}=\boldsymbol{w}$ ，明顯可得 $\langle\boldsymbol{u}, \boldsymbol{v}\rangle=\langle\boldsymbol{w}, \boldsymbol{v}\rangle, \forall \boldsymbol{v}$ ．
（7）若 $\boldsymbol{u}=\mathbf{0}$ ，明顯可得 $\left\langle\boldsymbol{u}, \boldsymbol{b}_i\right\rangle=0, \forall i=1,2, \ldots, n$ ．
若 $\left\langle\boldsymbol{u}, \boldsymbol{b}_i\right\rangle=0, \forall i=1,2, \ldots, n$ ，
$$
\forall \boldsymbol{v} \in V \text {, 令 } \boldsymbol{v}=\sum_{i=1}^n \alpha_i \boldsymbol{b}_i \text {, 則 }\langle\boldsymbol{u}, \boldsymbol{v}\rangle=\left\langle\boldsymbol{u}, \sum_{i=1}^n \alpha_i \boldsymbol{b}_i\right\rangle=\sum_{i=1}^n \overline{\alpha_i}<\boldsymbol{u}, \boldsymbol{b}_i>=\sum_{i=1}^n \overline{\alpha_i} \cdot \mathbf{0}=\mathbf{0} \text {, }
$$

故 $\boldsymbol{u}=\mathbf{0}$ by（5）．
（8）$\because<T(\boldsymbol{u}), \boldsymbol{v}>=0, \forall \boldsymbol{u}, \boldsymbol{v} \in V, \therefore<T(\boldsymbol{u}), T(\boldsymbol{u})>=0, \forall \boldsymbol{u} \in V, \therefore T(\boldsymbol{u})=\mathbf{0}, \forall \boldsymbol{u} \in V$ ，即 $T$ 為零映射
（9）$\because\langle T(\boldsymbol{v}), \boldsymbol{v}\rangle=0, \forall \boldsymbol{v} \in V$ ，