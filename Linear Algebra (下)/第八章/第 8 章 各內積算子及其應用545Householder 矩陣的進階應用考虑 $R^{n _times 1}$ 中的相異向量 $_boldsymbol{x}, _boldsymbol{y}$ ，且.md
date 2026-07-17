第 8 章 各內積算子及其應用
545

Householder 矩陣的進階應用
考虑 $R^{n \times 1}$ 中的相異向量 $\boldsymbol{x}, \boldsymbol{y}$ ，且 $\|\boldsymbol{x}\|=\|\boldsymbol{y}\|$ ，（使用2－norm），
令 $H$ 為相對於 $\boldsymbol{x}-\boldsymbol{y}$ 的 Householder 矩陣，則
（1）$\|x-y\|^2=2(x-y)^T x$ ，
（2）$H \boldsymbol{x}=\boldsymbol{y}$ ．
【 83.84 中正数統、 100 台大資工】
【證明】
（1）因為 $\|\boldsymbol{x}\|=\|\boldsymbol{y}\|$ ，得 $\|\boldsymbol{x}\|^2=\|\boldsymbol{y}\|^2, \therefore \boldsymbol{x}^T \boldsymbol{x}=\boldsymbol{y}^T \boldsymbol{y}$ ，
$$
\begin{aligned}
\therefore\|x-y\|^2 & =(x-y)^T(x-y)=\left(x^T-y^T\right)(x-y)=x^T x-x^T y-y^T x+y^T y \\
& =x^T x-y^T x-y^T x+x^T x,\left(\because x^T y=y^T x, x^T x=y^T y\right) \\
& =2(x-y)^T x .
\end{aligned}
$$
（2）
$$
\begin{aligned}
& \text { 令 } \boldsymbol{w}=\boldsymbol{x}-\boldsymbol{y}, \text { 則 } H=I-\frac{2}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w} \boldsymbol{w}^T=I-\frac{2}{\|\boldsymbol{x}-\boldsymbol{y}\|^2}(\boldsymbol{x}-\boldsymbol{y})(\boldsymbol{x}-\boldsymbol{y})^T \\
& \quad=I-\frac{2}{2(\boldsymbol{x}-\boldsymbol{y})^T \boldsymbol{x}}(\boldsymbol{x}-\boldsymbol{y})(\boldsymbol{x}-\boldsymbol{y})^T, \\
& \therefore H \boldsymbol{x}=\left[I-\frac{1}{(\boldsymbol{x}-\boldsymbol{y})^T \boldsymbol{x}}(\boldsymbol{x}-\boldsymbol{y})(\boldsymbol{x}-\boldsymbol{y})^T\right] \boldsymbol{x}=\boldsymbol{x}-\frac{1}{(\boldsymbol{x}-\boldsymbol{y})^T \boldsymbol{x}}(\boldsymbol{x}-\boldsymbol{y})(\boldsymbol{x}-\boldsymbol{y})^T \boldsymbol{x}=\boldsymbol{x}-(\boldsymbol{x}-\boldsymbol{y})=\boldsymbol{y}
\end{aligned}
$$

Note
（1）對 $R^{n \times 1}$ 中的任意向量 $\boldsymbol{x}$ ，取 $\alpha=\|\boldsymbol{x}\|, \boldsymbol{y}=\alpha \boldsymbol{e}_1, \boldsymbol{w}=\boldsymbol{x}-\boldsymbol{y}=\boldsymbol{x}-\alpha \boldsymbol{e}_1, H$ 為相對於 $\boldsymbol{w}$ 的 Householder 矩陣，則 $H x=\alpha \boldsymbol{e}_1=[\|x\| 0 \ldots 0]^T$ ，即後 $n-1$ 項為 0 ．
（2）設 $x=\left[\begin{array}{llll}x_1 & x_2 & \cdots & x_n\end{array}\right]^T \in R^{n \times 1}$ ，則存在一 Householder 矩陣 $H$ ，
使得 $H x$ 為一後 $n-k$ 項為 0 的行向量，for some $k, 1 \leq k \leq n$ ．
（3）考慮矩陣 $A \in R^{m \times n}$ ，
存在最多 $n$ 個 Householder 矩陣 $H_1, H_2, \ldots, H_n$ 使得 $H_n H_{n-1} \ldots H_1 A=R$ ，
其中，$(R)_{i j}=0, \forall i<j$ ，
又，若令 $Q=H_1 H_2 \ldots H_n$ ，則 $Q$ 為正交矩陣，且 $A=Q R$ ，為 $A$ 的 $Q R$ 分解．