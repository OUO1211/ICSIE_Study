---
subject: Linear Algebra
tags: [矩陣, 分解, Chapter1]
status: finished
---

## 定義

> **PLU 分解**：對任意 $n$ 階方陣 $A$，存在置換矩陣 $P$、下三角矩陣 $L$、上三角矩陣 $U$，使：
>
> $$PA = LU$$

其中 $P$ 為置換矩陣（各列各行恰有一個 $1$，其餘為 $0$）。

## 需要 PLU 的情況

當 $A$ 無法直接 LU 分解時（例如某主對角元素為 $0$），需先做**列置換 (row pivoting)** 以避免除以零。

## 例子

$$PA = LU \implies A = P^{-1}LU = P^T LU$$

（置換矩陣 $P$ 為正交矩陣，$P^{-1} = P^T$）

解方程組 $Ax = b$：$\implies$ 解 $PAx = Pb$ $\implies$ $LUx = Pb$

先解 $Ly = Pb$，再解 $Ux = y$。

## 相關連結

- [[LU分解]]
- [[基本列運算]]
