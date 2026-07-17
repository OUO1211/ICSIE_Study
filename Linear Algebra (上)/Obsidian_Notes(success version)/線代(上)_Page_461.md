> **試題 5**
>
> (3%) Let $T$ be a linear transformation from $R^3$ to $R^3$ defined by first rotating an angle $\theta_1$ about $y$-axis counterclockwise, and then rotating an angle $\theta_2$ about $z$-axis counterclockwise. Find the standard matrix representation of $T$ (write it as a multiplication of two matrices. No need to simplify your answer).
>
> 【95 交大資訊】

> **解**
>
> 對 $y$ 軸逆時針旋轉 $\theta_1$ 角所得的矩陣表示為：$\begin{bmatrix} \cos\theta_1 & 0 & \sin\theta_1 \\ 0 & 1 & 0 \\ -\sin\theta_1 & 0 & \cos\theta_1 \end{bmatrix}$
>
> 對 $z$ 軸逆時針旋轉 $\theta_2$ 角所得的矩陣表示為：$\begin{bmatrix} \cos\theta_2 & -\sin\theta_2 & 0 \\ \sin\theta_2 & \cos\theta_2 & 0 \\ 0 & 0 & 1 \end{bmatrix}$
>
> $\therefore$ 在標準基底的矩陣表示為：$\begin{bmatrix} \cos\theta_2 & -\sin\theta_2 & 0 \\ \sin\theta_2 & \cos\theta_2 & 0 \\ 0 & 0 & 1 \end{bmatrix}\begin{bmatrix} \cos\theta_1 & 0 & \sin\theta_1 \\ 0 & 1 & 0 \\ -\sin\theta_1 & 0 & \cos\theta_1 \end{bmatrix}$

---

> **試題 6**
>
> Find the standard matrix for the linear operators on $R^3$ that a rotation of 270° about the $x$-axis, followed by a reflection about the $yz$-plane and by a contraction with factor $k = 1/2$.
>
> 【99 中正逢甲機電融合、97 中山電機融合】

> **解**
>
> 繞 $x$ 軸旋轉 $270°$：$\cos 270° = 0$，$\sin 270° = -1$，得 $\begin{bmatrix} 1 & 0 & 0 \\ 0 & 0 & 1 \\ 0 & -1 & 0 \end{bmatrix}$。
>
> 對 $yz$ 平面鏡射：收縮矩陣為 $\begin{bmatrix} -1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$。
>
> 故合成為：
>
> $$\frac{1}{2}\begin{bmatrix} -1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}\begin{bmatrix} 1 & 0 & 0 \\ 0 & 0 & 1 \\ 0 & -1 & 0 \end{bmatrix} = \frac{1}{2}\begin{bmatrix} -1 & 0 & 0 \\ 0 & 0 & 1 \\ 0 & -1 & 0 \end{bmatrix}$$
