276
線性代數（下）

正交集的性質
（1）若 $S=\left\{\boldsymbol{v}_1, \ldots, \boldsymbol{v}_k\right\}$ 為一正交集，則 $\left\|\sum_{i=1}^k \alpha_i \boldsymbol{v}_i\right\|^2=\sum_{i=1}^k\left|\alpha_i\right|^2\left\|\boldsymbol{v}_i\right\|^2$ ．

【95中山電機】

特別在 $k=2, \alpha_1=\alpha_2=1$ 時，即為若 $v_1 \perp v_2$ ，則 $\left\|v_1+v_2\right\|^2=\left\|v_1\right\|^2+\left\|v_2\right\|^2$ 。（畢氏定理）
（2）若 $S=\left\{\boldsymbol{v}_1, \ldots, \boldsymbol{v}_k\right\}$ 為不含零向量的正交集，且 $\boldsymbol{v}=\sum_{i=1}^k \alpha_i \boldsymbol{v}_i$ ，則 $\alpha_i=\frac{\left\langle\boldsymbol{v}, \boldsymbol{v}_i\right\rangle}{\left\langle\boldsymbol{v}_i, \boldsymbol{v}_i\right\rangle}, \forall 1 \leq i \leq k$ ．
【證明】
【96暨南資工】
$$
\begin{aligned}
& \forall j,\left\langle\boldsymbol{v}, \boldsymbol{v}_j\right\rangle=\left\langle\sum_{i=1}^k \alpha_i \boldsymbol{v}_i, \boldsymbol{v}_j\right\rangle=\sum_{i=1}^k \alpha_i\left\langle\boldsymbol{v}_i, \boldsymbol{v}_j\right\rangle=\alpha_j\left\langle\boldsymbol{v}_j, \boldsymbol{v}_j\right\rangle,\left(\because\left\langle\boldsymbol{v}_i, \boldsymbol{v}_j\right\rangle=0, \forall i \neq j\right) \\
& \therefore \alpha_j=\frac{\left\langle\boldsymbol{v}, \boldsymbol{v}_j\right\rangle}{\left\langle\boldsymbol{v}_j, \boldsymbol{v}_j\right\rangle}
\end{aligned}
$$
（3）若 $S=\left\{\boldsymbol{v}_1, \ldots, \boldsymbol{v}_n\right\}$ 為單範正交基底，且 $[\boldsymbol{x}]_s=\left(x_1, \ldots, x_n\right)^T,[\boldsymbol{y}]_s=\left(y_1, \ldots, y_n\right)^T$ ，則 $\langle\boldsymbol{x}, \boldsymbol{y}\rangle=\sum_{i=1}^n x_i y_i$ ，且 distance $(\boldsymbol{x}, \boldsymbol{y})=\sqrt{\sum_{i=1}^n\left(x_i-y_i\right)^2}$.

【證明】

【100暨南資工】
$$
\begin{aligned}
\because \boldsymbol{x}=x_1 \boldsymbol{v}_1 & +x_2 \boldsymbol{v}_2+\ldots+x_n \boldsymbol{v}_n, \boldsymbol{y}=y_1 \boldsymbol{v}_1+y_2 \boldsymbol{v}_2+\ldots+y_n \boldsymbol{v}_n \\
\therefore<\boldsymbol{x}, \boldsymbol{y}> & =<x_1 \boldsymbol{v}_1+x_2 \boldsymbol{v}_2+\ldots+x_n \boldsymbol{v}_n, y_1 \boldsymbol{v}_1+y_2 \boldsymbol{v}_2+\ldots+y_n \boldsymbol{v}_n> \\
& =<x_1 \boldsymbol{v}_1, y_1 \boldsymbol{v}_1>+<x_2 \boldsymbol{v}_2, y_2 \boldsymbol{v}_2>+\ldots+<x_n \boldsymbol{v}_n, y_n \boldsymbol{v}_n> \\
& =x_1 y_1+x_2 y_2+\ldots+x_n y_n
\end{aligned}
$$

且可得 $d(\boldsymbol{x}, \boldsymbol{y})^2=\|\boldsymbol{x}-\boldsymbol{y}\|^2=\langle\boldsymbol{x}-\boldsymbol{y}, \boldsymbol{x}-\boldsymbol{y}\rangle=\sum_{i=1}^n\left(x_i-y_i\right)^2$ ．
（上述內積計算是佈於實數．）
（4）不含零向量的正交集必為線性獨立集．

【重要】

【證明】
令 $S=\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_k\right\}$ 為不含零向量的正交集，
設 $\alpha_1 \boldsymbol{v}_1+\alpha_2 \boldsymbol{v}_2+\ldots+\alpha_k \boldsymbol{v}_k=\mathbf{0}$ ，即 $\mathbf{0}=\sum_{i=1}^k \alpha_i \boldsymbol{v}_i$ ，
則由（2）得 $\alpha_i=\frac{\left\langle\boldsymbol{0}, \boldsymbol{v}_i\right\rangle}{\left\langle\boldsymbol{v}_i, \boldsymbol{v}_i\right\rangle}=0, \forall i$ ，
故 $S$ 為線性獨立集合。
（5）單範正交集必為線性獨立集。

【重要】