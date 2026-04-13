> **訣題 4**
>
> The homogeneous coordinates map $[x \; y \; z]^T$ to $[x \; y \; z \; 1]^T$, that can help us format translation in the form of linear transformations. Consider the figure below. There are two coordinate systems. One is with basis $B_1 = \{e_x, e_y, e_z\}$ and origin $o_1$, and the other is with basis $B_2 = \{e_U, e_V, e_W\}$ and origin $o_2$. Both $B_1$ and $B_2$ are orthonormal bases and obey the right-handed convention. The relation between $B_1$ and $B_2$ is a rotation operation.
>
> (1) (3%) If $[e_x]_{B_2} = [1 \; 0 \; 0]^T$ and $[e_y]_{B_2} = \begin{bmatrix} 0 \\ \frac{1}{2} \\ \frac{\sqrt{3}}{2} \end{bmatrix}$, please find $[e_z]_{B_2}$.
>
> (2) (4%) Without consider translation, i.e., $o_1 = o_2$, please find a $3\times 3$ rotation matrix that can transform $B_2$ coordinates to $B_1$ coordinates based on (1).
>
> (3) (3%) If $[o_1 - o_2]_{B_2} = [1 \; 2 \; 1]^T$, please find $[o_1 - o_2]_{B_1}$ based on (1).
>
> (4) (5%) Find the linear transformation in the homogeneous coordinate system to transform $[u \; v \; w \; 1]^T$ to $[x \; y \; z \; 1]^T$ based on (1) and (3).
>
> 【109 交大資工】

**解**

$B_1 = \{e_x = \begin{bmatrix}1\\0\\0\end{bmatrix}, e_y = \begin{bmatrix}0\\1\\0\end{bmatrix}, e_z = \begin{bmatrix}0\\0\\1\end{bmatrix}\}$

由題意知 $e_x = 1e_U + 0e_V + 0e_W$，$e_y = 0e_U + \frac{1}{2}e_V + \frac{\sqrt{3}}{2}e_W$，

令 $e_z = ae_U + be_V + ce_W$。

由 $\|e_z\|_2 = a^2 + b^2 + c^2 = 1$，

因為 $B_1, B_2$ 為單範正交基，故 $\langle e_x, e_z \rangle = 0a + 0b + 0c = 0$，

$\langle e_y, e_z \rangle = 0a + \frac{1}{2}b + \frac{\sqrt{3}}{2}c = 0$

可解得 $(a, b, c) = (0, \frac{\sqrt{3}}{2}, -\frac{1}{2})$，或 $(0, -\frac{\sqrt{3}}{2}, \frac{1}{2})$。

若取 $(a, b, c) = (0, \frac{\sqrt{3}}{2}, -\frac{1}{2})$，旋轉矩陣 $P = \begin{bmatrix}1&0&0\\0&\frac{1}{2}&\frac{\sqrt{3}}{2}\\0&\frac{\sqrt{3}}{2}&-\frac{1}{2}\end{bmatrix}$，但此時 $P^2 = I$，$P$ 為鏡射矩陣，不合。

**(1)** 故取 $(a, b, c) = (0, -\frac{\sqrt{3}}{2}, \frac{1}{2})$，即

$$[e_z]_{B_2} = \begin{bmatrix} 0 \\ -\frac{\sqrt{3}}{2} \\ \frac{1}{2} \end{bmatrix}$$

**(2)** 旋轉矩陣 $P$ 使 $[v]_{B_2} = P[v]_{B_1}$，故所求為 $P^{-1} = Q$，

$$Q = \begin{bmatrix} 1 & 0 & 0 \\ 0 & \frac{1}{2} & \frac{\sqrt{3}}{2} \\ 0 & -\frac{\sqrt{3}}{2} & \frac{1}{2} \end{bmatrix}$$

使得 $[v]_{B_1} = Q[v]_{B_2}$。

**(3)** $[o_1 - o_2]_{B_1} = Q[o_1 - o_2]_{B_2} = \begin{bmatrix}1&0&0\\0&\frac{1}{2}&\frac{\sqrt{3}}{2}\\0&-\frac{\sqrt{3}}{2}&\frac{1}{2}\end{bmatrix} \begin{bmatrix}1\\2\\1\end{bmatrix} = \begin{bmatrix} 1 \\ \frac{2+\sqrt{3}}{2} \\ \frac{1-2\sqrt{3}}{2} \end{bmatrix}$

**(4)** 由(3)知 $o_1 - o_2 = e_U + 2e_V + e_W$，由(1)知

$$e_x = e_U, \quad e_y = \frac{1}{2}e_V + \frac{\sqrt{3}}{2}e_W, \quad e_z = -\frac{\sqrt{3}}{2}e_V + \frac{1}{2}e_W$$

考慮向量 $r$，$[r]_{B_1} = [x \; y \; z \; 1]^T$，$[r]_{B_2} = [u \; v \; w \; 1]^T$，則

$$r = xe_x + ye_y + ze_z + o_1 = ue_U + ve_V + we_W + o_2$$

故所求 $4 \times 4$ 齊次座標變換矩陣為：

$$\begin{bmatrix} x \\ y \\ z \\ 1 \end{bmatrix} = \begin{bmatrix} 1 & 0 & 0 & 1 \\ 0 & \frac{1}{2} & \frac{\sqrt{3}}{2} & \frac{2+\sqrt{3}}{2} \\ 0 & -\frac{\sqrt{3}}{2} & \frac{1}{2} & \frac{1-2\sqrt{3}}{2} \\ 0 & 0 & 0 & 1 \end{bmatrix} \begin{bmatrix} u \\ v \\ w \\ 1 \end{bmatrix}$$
