# 第二章 線性方程組與求解 109

## 2-1 線性方程組

> **定義：線性方程組 (system of linear equations)**
>
> 稱
> $$\begin{cases} a_{11}x_1 + a_{12}x_2 + \cdots + a_{1n}x_n = b_1 \\ a_{21}x_1 + a_{22}x_2 + \cdots + a_{2n}x_n = b_2 \\ \vdots \\ a_{m1}x_1 + a_{m2}x_2 + \cdots + a_{mn}x_n = b_m \end{cases}$$
>
> 為 $m$ 等式 $n$ 變數的線性系統或線性方程組，也以
>
> $Ax = b$ 表示，其中 $A = \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ a_{21} & a_{22} & \cdots & a_{2n} \\ \vdots & & \ddots & \vdots \\ a_{m1} & a_{m2} & \cdots & a_{mn} \end{bmatrix}$ 為係數矩陣，$x = \begin{bmatrix} x_1 \\ x_2 \\ \vdots \\ x_n \end{bmatrix}$，$b = \begin{bmatrix} b_1 \\ b_2 \\ \vdots \\ b_m \end{bmatrix}$。

> **Note**
>
> (1) $[A \mid b] = \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n} & b_1 \\ a_{21} & a_{22} & \cdots & a_{2n} & b_2 \\ \vdots & & & \vdots & \vdots \end{bmatrix}$ 稱為 $Ax = b$ 的**增廣矩陣 (augmented matrix)**。
>
> (2) 若 $Ax = b$ 有解，則稱此系統為**一致的 (consistent)**，否則稱不一致的 (inconsistent)。
>
> (3) $Ax = b$ 的解集合稱為 $Ax = b$ 的**解空間 (solution space)**。
>
> (4) $Ax = b$（$b = 0$）稱 $A$ 為**齊次的 (homogeneous)** 方程組，否則稱非齊次 (nonhomogeneous)。
>
> (5) $Ax = 0$ 的解空間又稱為 $A$ 的**零空間 (null space)**，或 $A$ 的**核空間 (kernel)**。
>
> (6) 零向量為 $Ax = 0$ 的**零解（trivial solution）**。
>
> (7) 若兩線性系統有相同解，則稱此兩線性系統等價（equivalent）。
>
> 【97 台科資工】
>
> (i) 若 $\{A_1\}$ 列等價於 $\{A_2 \mid b_2\}$，則 $A_1x = b_1$ 與 $A_2x = b_2$ 具有相同的解集合。
>
> (ii) 若 $A$ 列等價於 $A_2$，則 $A_1x = 0$ 與 $A_2x = 0$ 具有相同的解集合。
>
> (8) 若 $Ax = b$ 有解，則解集合中所有元素的形式 $\{x_0 + u \mid u \in U\} = \{u \mid Au = 0\}$。
>
> (9) **解線性方程組的常用方法：**
>
> (i) 高斯消去法（高斯－喬丹消去法）
>
> (ii) 先求出 $A^{-1}$，則 $x = A^{-1}b$（$A$ 為可逆矩陣時）
>
> (iii) 先對 $A$ 做 LU 分解（當然先要 $A$ 能做 LU 分解）
>
> (iv) Cramer's rule（$A$ 為可逆矩陣時）
