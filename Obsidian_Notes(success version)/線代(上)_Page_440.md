> **試題 13**
>
> (15%) Let $A = \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix}$ be an orthogonal matrix.
>
> (1) Suppose $\begin{bmatrix} y_0 \\ y_1 \end{bmatrix} = A \begin{bmatrix} x_0 \\ x_1 \end{bmatrix}$, where $\begin{bmatrix} x_0 \\ x_1 \end{bmatrix}$ and $\begin{bmatrix} y_0 \\ y_1 \end{bmatrix}$ are the coordinate vectors relative to the old orthonormal basis $\left\{ \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \begin{bmatrix} 0 \\ 1 \end{bmatrix} \right\}$ and a new basis, respectively. Find the new basis.
>
> (2) Suppose $\begin{bmatrix} y_{0,0} & y_{0,1} \\ y_{1,0} & y_{1,1} \end{bmatrix} = A \begin{bmatrix} x_{0,0} & x_{0,1} \\ x_{1,0} & x_{1,1} \end{bmatrix} A^T$, where $\begin{bmatrix} x_{0,0} & x_{0,1} \\ x_{1,0} & x_{1,1} \end{bmatrix}$ and $\begin{bmatrix} y_{0,0} & y_{0,1} \\ y_{1,0} & y_{1,1} \end{bmatrix}$ are the coordinate vectors to the old orthonormal basis $\left\{ \begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 1 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 \\ 1 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 \\ 0 & 1 \end{bmatrix} \right\}$ and a new basis, respectively. Find the new basis.
>
> 【97、101 暨南資工】

解：

(1) 令 $\beta = \left\{ \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \begin{bmatrix} 0 \\ 1 \end{bmatrix} \right\}$，$\alpha$ 為欲求得的基底，由題意知 $A$ 為 $\beta$ 到 $\alpha$ 的座標轉移矩陣，

設 $\alpha = \begin{bmatrix} a \\ c \end{bmatrix}, \begin{bmatrix} b \\ d \end{bmatrix}$，則 $\begin{bmatrix} a & b \\ c & d \end{bmatrix} = A^{-1} = \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix}$，故 $\alpha = \left\{ \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ 1 \end{bmatrix}, \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ -1 \end{bmatrix} \right\}$。

(2) 考慮新基底 $\beta = \left\{ \begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 1 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 \\ 1 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 \\ 0 & 1 \end{bmatrix} \right\}$，

代入 $\begin{bmatrix} y_{0,0} & y_{0,1} \\ y_{1,0} & y_{1,1} \end{bmatrix} = A \begin{bmatrix} x_{0,0} & x_{0,1} \\ x_{1,0} & x_{1,1} \end{bmatrix} A^T$，

分別得到新座標 $\alpha = \left\{ \dfrac{1}{2} E_1 + \dfrac{1}{2} E_2 + \dfrac{1}{2} E_3 + \dfrac{1}{2} E_4, \ldots \right\}$，

$$\gamma = \left\{ \begin{bmatrix} \frac{1}{2} & \frac{1}{2} \\ \frac{1}{2} & \frac{1}{2} \end{bmatrix}, \begin{bmatrix} \frac{1}{2} & -\frac{1}{2} \\ \frac{1}{2} & -\frac{1}{2} \end{bmatrix}, \begin{bmatrix} \frac{1}{2} & \frac{1}{2} \\ -\frac{1}{2} & -\frac{1}{2} \end{bmatrix}, \begin{bmatrix} \frac{1}{2} & -\frac{1}{2} \\ -\frac{1}{2} & \frac{1}{2} \end{bmatrix} \right\}$$
