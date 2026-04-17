---
subject: Linear Algebra
chapter: 3
section: 3-2
status: finished
tags: [Wronskian, 函數空間, 線性獨立]
---

# Wronskian（朗斯基行列式）

## 定義

設 $f_1, f_2, \ldots, f_n \in C^{n-1}[a,b]$（$n-1$ 次可微），定義其 **Wronskian**：

$$W(f_1, f_2, \ldots, f_n) = \det \begin{bmatrix} f_1 & f_2 & \cdots & f_n \\ f_1' & f_2' & \cdots & f_n' \\ \vdots & \vdots & & \vdots \\ f_1^{(n-1)} & f_2^{(n-1)} & \cdots & f_n^{(n-1)} \end{bmatrix}$$

## 性質

> 若存在 $x_0 \in [a,b]$ 使得 $W(f_1,\ldots,f_n)|_{x=x_0} \neq 0$，  
> 則 $\{f_1, f_2, \ldots, f_n\}$ 在 $C^{n-1}[a,b]$ 上為**線性獨立集**。

**注意**：逆命題不成立！

反例：$f_1 = x^2$，$f_2 = x|x|$ 在 $[-1,1]$ 上，$W=0$ 但 $\{f_1,f_2\}$ 為獨立集。

## 證明

$$W(f_1,\ldots,f_n) = \det(A) \neq 0 \text{ at } x_0$$

若 $\sum \alpha_i f_i = 0$，對兩端逐次微分，整理成矩陣方程 $A\alpha = 0$，

因為 $\det(A)|_{x_0} \neq 0$，唯一解為 $\alpha = 0$，故獨立。

## 經典考題

| 函數集 | Wronskian | 結論 |
|--------|-----------|------|
| $\{1, \cos x, \sin x\}$ | $= -1 \neq 0$ | 獨立 |
| $\{1, e^{ix}, e^{-ix}\}$ | $= -2i \neq 0$ | 獨立 |
| $\{e^x, e^{2x}, e^{3x}\}$ | $= -2e^{6x} \neq 0$ | 獨立 |
| $\{e^x+e^{-x}, e^x-e^{-x}, e^{2x}\}$ | $= 12e^{2x} \neq 0$ | 獨立 |

**相關**：[[線性獨立與相依]]、[[常見向量空間]]
