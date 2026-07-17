第 7 章 內積空間 301

7－3 正交投影及其應用

正交投影向量（orthogonal projection vector）
考虑向量空間 $V$ 上的一個子空間 $W$ ，對 $V$ 中任意向量 $\boldsymbol{v}$ ，若存在 $\boldsymbol{v}_0 \in W$ ，使得 $\left\langle\boldsymbol{v}-\boldsymbol{v}_0, \boldsymbol{w}\right\rangle=0, \forall \boldsymbol{w} \in W$ ，則稱 $\boldsymbol{v}_0$ 為 $\boldsymbol{v}$ 在 $W$ 上的正交投影向量，並記做 $\boldsymbol{v}_0=$ proj $_W \boldsymbol{v}$ 。

Note
（1）令 $\beta=\left\{\boldsymbol{b}_1, \ldots, \boldsymbol{b}_k\right\}$ 為 $W$ 的一組基底，則對任一向量 $\boldsymbol{v}$ ，
（a）$\langle\boldsymbol{v}, \boldsymbol{w}\rangle=0, \forall \boldsymbol{w} \in W \Leftrightarrow\left\langle\boldsymbol{v}, \boldsymbol{b}_i\right\rangle=0, \forall i$ ．
【證明】
⇒ 明顯成立。
$$
\Leftarrow \forall \boldsymbol{w} \in W \text {, 令 } \boldsymbol{w}=\sum_{i=1}^k \alpha_i \boldsymbol{b}_i \text {, 則 }\langle\boldsymbol{v}, \boldsymbol{w}\rangle=\left\langle\mathbf{v}, \sum_{i=1}^k \alpha_i \boldsymbol{b}_i\right\rangle=\sum_{i=1}^k \overline{\alpha_i}\left\langle\boldsymbol{v}, \boldsymbol{b}_i\right\rangle=\sum_{i=1}^k \overline{\alpha_i} \cdot 0=0 \text {. }
$$
（b）若 $\beta$ 為 $W$ 的一組正交基底，則 $p r o j_W \boldsymbol{v}=\boldsymbol{v}_0=\sum_{i=1}^k \frac{\left\langle\boldsymbol{v}, \boldsymbol{b}_i\right\rangle}{\left\langle\boldsymbol{b}_i, \boldsymbol{b}_i\right\rangle} \boldsymbol{b}_i$ ．
【證明】（由此而得一求得正交投影向量的方法）【95中正資工、95台北統計】由 $\boldsymbol{v}_0$ 的定義方式可知 $\boldsymbol{v}_0 \in \operatorname{span}(\beta)=W$ ，且 for $1 \leq j \leq k$ ，
$$
\begin{aligned}
\left\langle\boldsymbol{v}-\boldsymbol{v}_0, \boldsymbol{b}_j\right\rangle & \left.\left.\left.=<\boldsymbol{v}-\sum_{i=1}^k \frac{\left\langle\boldsymbol{v}, \boldsymbol{b}_i\right\rangle}{\left\langle\boldsymbol{b}_i, \boldsymbol{b}_i\right\rangle} \boldsymbol{b}_i, \boldsymbol{b}_j\right\rangle \quad=<\boldsymbol{v}, \boldsymbol{b}_j\right\rangle-\sum_{i=1}^k \frac{\left\langle\boldsymbol{v}, \boldsymbol{b}_i\right\rangle}{\left\langle\boldsymbol{b}_i, \boldsymbol{b}_i\right\rangle}<\boldsymbol{b}_i, \boldsymbol{b}_j\right\rangle \\
& \left.\left.\left.=<\boldsymbol{v}, \boldsymbol{b}_j\right\rangle-\frac{\left\langle\boldsymbol{v}, \boldsymbol{b}_j\right\rangle}{\left\langle\boldsymbol{b}_j, \boldsymbol{b}_j\right\rangle}\left\langle\boldsymbol{b}_j, \boldsymbol{b}_j\right\rangle=<\boldsymbol{v}, \boldsymbol{b}_j\right\rangle-<\boldsymbol{v}, \boldsymbol{b}_j\right\rangle=0
\end{aligned}
$$

故由（1）得 $\left\langle\boldsymbol{v}-\boldsymbol{v}_0, \boldsymbol{w}\right\rangle=0, \forall \boldsymbol{w} \in W$ ，即 $\boldsymbol{v}_0$ 為 $\boldsymbol{v}$ 在 $W$ 上的正交投影向量．
（c） $\boldsymbol{v}$ 在 $W$ 上的正交投影向量存在且唯一。
（2） proj $_W \boldsymbol{v}$ 的性質：
（a） $\boldsymbol{v} \in W \Leftrightarrow \operatorname{proj}_W \boldsymbol{v}=\boldsymbol{v}$ ．
（b） $\operatorname{proj}_W \mathbf{0}=\mathbf{0}$ ．
（c）若 $\boldsymbol{\nu}$ 與 $W$ 中的任何向量均正交，則 proj $_W \boldsymbol{\nu}=\mathbf{0}$ 。
（3）關於投影後的長度：
$\left\|\boldsymbol{v}-\operatorname{proj}_W(\boldsymbol{v})\right\| \leq\|\boldsymbol{v}-\boldsymbol{w}\|, \forall \boldsymbol{w} \in W$.
【98台科資工、98中興統計】
【證明】即 $\operatorname{proj}_W v$ 為 $W$ 上最靠近 $v$ 的向量，為 $v$ 在 $W$ 上的最佳逼近．