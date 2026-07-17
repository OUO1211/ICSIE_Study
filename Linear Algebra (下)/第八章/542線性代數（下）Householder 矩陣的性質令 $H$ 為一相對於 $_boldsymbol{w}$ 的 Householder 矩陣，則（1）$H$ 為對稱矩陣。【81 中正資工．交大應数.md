542
線性代數（下）

Householder 矩陣的性質
令 $H$ 為一相對於 $\boldsymbol{w}$ 的 Householder 矩陣，則
（1）$H$ 為對稱矩陣。
【81 中正資工．交大應数、 100 嘉義應数】
（2）$H$ 為正交矩陣．
【 100 嘉義應数】
（3） $\operatorname{det}(H)=-1$ ．
【證明】
考慮 $R^{n \times 1}$ 中的非零向量 $\boldsymbol{w}$ ，令 $H=I-\frac{2}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w} \boldsymbol{w}^T$ ，為對於 $\boldsymbol{w}$ 的 Householder 矩陣，則
（1）$H^T=\left(I-\frac{2}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w} \boldsymbol{w}^T\right)^T=I^T-\frac{2}{\boldsymbol{w}^T \boldsymbol{w}}\left(\boldsymbol{w} \boldsymbol{w}^T\right)^T=I-\frac{2}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w} \boldsymbol{w}^T=H$ ，故 $H$ 為對稱矩陣．
（2）
$$
\begin{aligned}
H^T H & =H^2=\left(I-\frac{2}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w} \boldsymbol{w}^T\right)\left(I-\frac{2}{\mathbf{w}^T \boldsymbol{w}} \boldsymbol{w} \boldsymbol{w}^T\right)=I-\frac{4}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w} \boldsymbol{w}^T+\left(\frac{2}{\boldsymbol{w}^T \boldsymbol{w}}\right)^2\left(\boldsymbol{w} \boldsymbol{w}^T\right)\left(\boldsymbol{w} \boldsymbol{w}^T\right) \\
& =I-\frac{4}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w} \boldsymbol{w}^T+\left(\frac{2}{\boldsymbol{w}^T \boldsymbol{w}}\right)^2\left(\boldsymbol{w}\left(\boldsymbol{w}^T \boldsymbol{w}\right) \boldsymbol{w}^T\right)=I-\frac{4}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w} \boldsymbol{w}^T+\frac{4}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w} \boldsymbol{w}^T=I
\end{aligned}
$$

故 $H$ 為正交．
（3）$H \boldsymbol{w}=\left(I-\frac{2}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w} \boldsymbol{w}^T\right) \boldsymbol{w}=\boldsymbol{w}-\frac{2}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w}\left(\boldsymbol{w}^T \boldsymbol{w}\right)=\boldsymbol{w}-2 \boldsymbol{w}=-\boldsymbol{w}, \therefore-1$ 為 $H$ 的一個特徵根令 $W=\operatorname{span}\{\boldsymbol{w}\}$ ，則 $\operatorname{dim}(W)=1$ ，
又因 $R^{n \times 1}=W \oplus W^{\perp}, n=\operatorname{dim}(W)+\operatorname{dim}\left(W^{\perp}\right), \therefore \operatorname{dim}\left(W^{\perp}\right)=n-1$ ，
考慮 $\left\{\boldsymbol{w}_2, \boldsymbol{w}_3, \ldots, \boldsymbol{w}_n\right\}$ 為 $W^{\perp}$ 的一組基底，
則 for $2 \leq i \leq n, H \boldsymbol{w}_i=\left(I-\frac{2}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w} \boldsymbol{w}^T\right) \boldsymbol{w}_i=\boldsymbol{w}_i-\frac{2}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w}\left(\boldsymbol{w}^T \boldsymbol{w}_i\right)=\boldsymbol{w}_i,\left(\because \boldsymbol{w} \perp \boldsymbol{w}_i\right)$
$\therefore 1$ 為 $H$ 的一個特徵根，
但 $\left\{\boldsymbol{w}_2, \boldsymbol{w}_3, . ., \boldsymbol{w}_n\right\}$ 為獨立集，故 1 的代數重數 $\geq 1$ 的幾何重數 $=\operatorname{dim}(V(1)) \geq n-1$ ，又已知 -1 是一特徵根了，故 1 的代數重數恰 $=n-1, \operatorname{det}(H)=-1 \cdot 1 \cdot 1 \cdot \ldots \cdot 1=-1$ ．