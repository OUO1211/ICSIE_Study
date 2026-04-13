# 第二章 線性方程組與求解 158

## 齊次方程的奇異 (singular) 與非奇異 (nonsingular)

> **定義**
>
> 若 $Ax = 0$ 有非零解，稱矩陣 $A$ 為**奇異的**。
>
> 若 $Ax = 0$ 只有零解，稱矩陣 $A$ 為**非奇異的**。
>
> 【100 政大統計】

> **Note**
>
> 若此時所討論的矩陣為方陣，則 $A$ 為可逆矩陣是 $A$ 為非奇異的充要條件。

例如：

(1) $\begin{cases} x + y = 0 \\ 2x + 2y = 0 \end{cases}$ 有解：$(0,0)$，$(1,-1)$，…，故為奇異的系統。

而且 $A = \begin{bmatrix} 1 & 1 \\ 2 & 2 \end{bmatrix}$ 不可逆。

(2) $\begin{cases} x + y + z = 0 \\ 2x + 2y + z = 0 \end{cases}$ 有解：$(0,0,0)$，$(1,-1,0)$，…，故為奇異的系統。

而且 $A = \begin{bmatrix} 1 & 1 & 1 \\ 2 & 2 & 1 \end{bmatrix}$ 不可逆。

(3) $\begin{cases} x + y = 0 \\ 2x + y = 0 \end{cases}$ 只有解：$(0,0)$，故為非奇異的系統。

而且 $A = \begin{bmatrix} 1 & 1 \\ 2 & 1 \end{bmatrix}$ 為可逆矩陣。

(4) $\begin{cases} x + y = 0 \\ x - y = 0 \\ 2x - 3y = 0 \end{cases}$ 只有解：$(0,0)$，故為非奇異的系統。

而且 $A = \begin{bmatrix} 1 & 1 \\ 1 & -1 \\ 2 & -3 \end{bmatrix}$ 為不可逆矩陣。