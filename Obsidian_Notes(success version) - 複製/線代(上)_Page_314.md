## 矩陣相依或獨立－用所在空間的維度參考

這裡採用下一小節會介紹的“維度”。若向量空間 $V$ 的維度為 $k$，$S$ 為 $V$ 的一個向量集，且 $S$ 中有超過 $k$ 個向量，則 $S$ 必為相依集。

> **例題 11**
>
> 判斷獨立或相依：
>
> (1) $\{x+1, x^2-x+1, x^2+3x-2, 2x^2+8x+1\}$ in $P_2$。 【95 成大資工】
>
> (2) $\{(1,5,1), (5,1,-1), (3,3,0), (10,14,1)\}$ in $\mathbb{R}^3$。 【99 師大資工】
>
> (3) $A=\begin{bmatrix}\cos(\pi/4) & \sin(\pi/4) \\ -\sin(\pi/4) & \cos(\pi/4)\end{bmatrix}$，$B=\begin{bmatrix}e & 1 \\ 1 & e^{-1}\end{bmatrix}$，$C=\begin{bmatrix}1 & -1 \\ 1 & 1\end{bmatrix}$，$D=\begin{bmatrix}0 & 1 \\ 2 & 1\end{bmatrix}$，$E=\begin{bmatrix}0 & 8 \\ 4 & 0\end{bmatrix}$ in $\mathbb{R}^{2\times 2}$。 【99 成大資工】
>
> **解**
>
> (1) 線性相依。因為 $\dim(P_2)=3$，故最大獨立集只能有 3 個向量。
>
> (2) 線性相依。
>
> (3) 線性相依。因為 $\mathbb{R}^{2\times 2}$ 中的最大獨立集合有 4 個向量。