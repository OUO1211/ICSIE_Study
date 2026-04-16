---
subject: Linear Algebra
tags: [行列式, 方法, Chapter2]
status: finished
---

## 定義

> **Laplace 展開法**：固定某一列（行），將 $n$ 階行列式展開為 $(n-1)$ 階行列式的線性組合。

**按第 $i$ 列展開**：

$$\det(A) = \sum_{k=1}^{n} a_{ik}\,\text{cof}(a_{ik}) = \sum_{k=1}^{n} a_{ik}(-1)^{i+k}\det(M_{ik})$$

**按第 $j$ 行展開**：

$$\det(A) = \sum_{k=1}^{n} a_{kj}\,\text{cof}(a_{kj})$$

## 技巧

選擇含**最多零**的列或行展開，可大幅減少計算量。

## 例子（按第一行展開）

$$A = \begin{bmatrix} a & b & c \\ d & e & f \\ g & h & i \end{bmatrix}$$

$$\det(A) = a(ei - fh) - d(bi - ch) + g(bf - ce)$$

## 步驟

- **Step 1**：選定展開的列（行），通常選零最多的
- **Step 2**：對每個非零元素 $a_{ik}$，計算其[[小行列式與餘因子|餘因子]] $\text{cof}(a_{ik})$
- **Step 3**：累加 $a_{ik} \cdot \text{cof}(a_{ik})$

## 相關連結

- [[小行列式與餘因子]]
- [[行列式定義]]
- [[特殊矩陣的行列式]]
