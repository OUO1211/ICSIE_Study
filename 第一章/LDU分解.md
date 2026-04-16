---
subject: Linear Algebra
tags: [矩陣, 分解, Chapter1]
status: finished
---

## 定義

> **LDU 分解**：給定 $n$ 階方陣 $A$，若存在 $A = LDU$，其中：
>
> - $L$：下三角矩陣，對角項全為 $1$
> - $D$：對角矩陣
> - $U$：上三角矩陣，對角項全為 $1$

〔92 成大統計〕

## 步驟

1. 先做 [[LU分解]] 得 $A = L U_0$（$L$ 對角項為 1）
2. 令 $D = \operatorname{diag}(u_{11}, u_{22}, \ldots, u_{nn})$（$U_0$ 的對角項）
3. $U = D^{-1} U_0$（對角項全化為 1）
4. 得 $A = L D U$

## 例子

$$A = \begin{bmatrix} 2 & 3 & 1 \\ 4 & 1 & 4 \\ 3 & 4 & 6 \end{bmatrix} = \underbrace{\begin{bmatrix} 1 & 0 & 0 \\ 2 & 1 & 0 \\ \frac{3}{2} & \frac{1}{10} & 1 \end{bmatrix}}_{L} \underbrace{\begin{bmatrix} 2 & 0 & 0 \\ 0 & -5 & 0 \\ 0 & 0 & \frac{43}{10} \end{bmatrix}}_{D} \underbrace{\begin{bmatrix} 1 & \frac{3}{2} & \frac{1}{2} \\ 0 & 1 & -\frac{2}{5} \\ 0 & 0 & 1 \end{bmatrix}}_{U}$$

## 相關連結

- [[LU分解]]
- [[對角矩陣與單位矩陣]]
