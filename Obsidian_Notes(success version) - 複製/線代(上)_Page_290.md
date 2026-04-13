## 第 3 章　向量空間

> **例題 4**
>
> (5%) $S_1 = \{(1, 2, 3), (2, 3, 4)\}$，$S_2 = \{(5, 8, 11), (1, 1, 1), (1, -1, -3)\}$. Is the space spanned by the set $S_1$ a subspace of the spanned by $S_2$?
>
> 【95 清大統計】

**解** 考慮 $S_1$：$\begin{bmatrix} 5 \\ 8 \\ 11 \end{bmatrix} = x_1 \begin{bmatrix} 1 \\ 2 \\ 3 \end{bmatrix} + x_2 \begin{bmatrix} 2 \\ 3 \\ 4 \end{bmatrix}$，$S_2 = y_1 \begin{bmatrix} 1 \\ 2 \\ 3 \end{bmatrix} + y_2 \begin{bmatrix} 2 \\ 3 \\ 4 \end{bmatrix} + y_3 \begin{bmatrix} -1 \\ -3 \end{bmatrix}$，是否有解。

檢查增廣矩陣 $\begin{bmatrix} 5 & 1 & 1 & 2 \\ 8 & 1 & -1 & 2 & 3 \\ 11 & 1 & -3 & 3 & 4 \end{bmatrix}$，列運算後可得 $\begin{bmatrix} 0 & 3 & 13 & 2 & -1 \\ 0 & 0 & 0 & 0 & 0 \end{bmatrix}$，

即可解出 $(x_1, x_2, x_3)$ 對應 $(y_1, y_2, y_3)$，

故 $S_1 \subseteq \text{span}(S_2)$，故 $\text{span}(S_1) \subseteq \text{span}(S_2)$。
