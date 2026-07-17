## 特殊的線性映射 — 鏡射(reflection)

> **定義**
>
> 定義 $T: R^2 \to R^2$，定義 $T\begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}\begin{bmatrix} x \\ y \end{bmatrix}$
>
> 表示平面上的點 $\begin{bmatrix} x \\ y \end{bmatrix}$，對 $x$ 軸做鏡射到對應位置。
>
> 定義 $T: R^2 \to R^2$，定義 $T\begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix}\begin{bmatrix} x \\ y \end{bmatrix}$
>
> 表示平面上的點 $\begin{bmatrix} x \\ y \end{bmatrix}$，對 $y$ 軸做鏡射到對應位置。

> **Note**
>
> (1) $\begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & -1 \end{bmatrix}$ 為 $R^3$ 上對 $xy$ 平面做鏡射的矩陣表示。
>
> (2) $\begin{bmatrix} 1 & 0 & 0 \\ 0 & -1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$ 為 $R^3$ 上對 $xz$ 平面做鏡射的矩陣表示。
>
> (3) $\begin{bmatrix} -1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$ 為 $R^3$ 上對 $yz$ 平面做鏡射的矩陣表示。
>
> (4) 對其他平面的鏡射則用 Householder 矩陣（詳第八章討論）。
>
> (5) 縮放：成為 $T_s: R^2 \to R^2$，定義為 $T_s\begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} k_x & 0 \\ 0 & k_y \end{bmatrix}\begin{bmatrix} x \\ y \end{bmatrix}$，
>
> 表示平面上的點 $(x,y)$，縮放以 $k$ 到對應的位置。
