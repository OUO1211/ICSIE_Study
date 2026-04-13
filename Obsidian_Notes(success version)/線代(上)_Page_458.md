## 特殊的線性映射 — 旋轉(rotation)

> **定義**
>
> 定義 $T_\theta: R^2 \to R^2$，定義 $T_\theta\begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{bmatrix}\begin{bmatrix} x \\ y \end{bmatrix}$
>
> 表示平面上的點 $\begin{bmatrix} x \\ y \end{bmatrix}$，逆時針旋轉 $\theta$ 角到對應位置。【參考書】

> **【證明】**
>
> $T_\theta\begin{bmatrix} 1 \\ 0 \end{bmatrix} = \begin{bmatrix} \cos\theta \\ \sin\theta \end{bmatrix}$，$T_\theta\begin{bmatrix} 0 \\ 1 \end{bmatrix} = \begin{bmatrix} -\sin\theta \\ \cos\theta \end{bmatrix}$
>
> $\therefore T_\theta = \begin{bmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{bmatrix}$

> **Note**
>
> (1) $(T_\theta)^{-1} = T_{-\theta}$，$(T_\theta)^T = T_{-\theta}$，$T_\theta T_\phi = T_{\theta+\phi}$。
>
> (2) 繞著 $R^3$ 上的 $x,y,z$ 軸作旋轉的旋轉矩陣如下：
>
> (a) $\begin{bmatrix} 1 & 0 & 0 \\ 0 & \cos\theta & -\sin\theta \\ 0 & \sin\theta & \cos\theta \end{bmatrix}$，表繞著 $x$ 軸，由 $y$ 方向往 $z$ 方向旋轉 $\theta$ 角的線性映射矩陣
>
> (b) $\begin{bmatrix} \cos\theta & 0 & -\sin\theta \\ 0 & 1 & 0 \\ \sin\theta & 0 & \cos\theta \end{bmatrix}$，表繞著 $y$ 軸，由 $x$ 方向往 $z$ 方向旋轉 $\theta$ 角的線性映射矩陣
>
> (c) $\begin{bmatrix} \cos\theta & -\sin\theta & 0 \\ \sin\theta & \cos\theta & 0 \\ 0 & 0 & 1 \end{bmatrix}$，表繞著 $z$ 軸，由 $x$ 方向往 $y$ 方向旋轉 $\theta$ 角的線性映射矩陣

以下為三種旋轉情況示意圖（繞 $x$ 軸、$y$ 軸、$z$ 軸）。