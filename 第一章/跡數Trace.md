---
subject: Linear Algebra
tags: [矩陣, 定義, Chapter1]
status: finished
core_mapping: "求對角項之和，利用 tr(AB)=tr(BA) 交換循環"
mantra: "跡數加對角，AB 換位跡不變"
pattern_signal_strong:
  - condition: "題目出現 tr(A) 或要計算對角項之和"
    weight: 3
  - condition: "題目涉及 AB-BA=I 的矛盾證明"
    weight: 3
pattern_signal_weak:
  - condition: "出現 tr(A^T)=tr(A) 或 tr(A^H)=tr(A) 的共軛"
    weight: 1
  - condition: "出現 tr(αA+βB) 的線性組合"
    weight: 1
anti_signal:
  - condition: "tr(AB) ≠ tr(A)tr(B)（乘積跡數不等於跡數乘積）"
  - condition: "tr(A^n) ≠ (tr(A))^n（高次跡數不等於跡數的冪次）"
---

## 定義

> **跡數 (trace)**：方陣 $A$ 的對角項之和。
>
> $$\text{tr}(A) = \sum_{i=1}^{n} a_{ii}$$

## 例子

$$A = \begin{bmatrix} 1 & 4 \\ 2 & 3 \end{bmatrix}, \quad \text{tr}(A) = 1 + 3 = 4$$

$$B = \begin{bmatrix} 9 & -1 & 2 \\ -4 & 5 & 3 \\ 1 & 6 & -7 \end{bmatrix}, \quad \text{tr}(B) = 9 + 5 + (-7) = 7$$

## 性質

1. $\text{tr}(\alpha A + \beta B) = \alpha\,\text{tr}(A) + \beta\,\text{tr}(B)$（**線性函數**）
2. $\text{tr}(A^T) = \text{tr}(A)$
3. $\text{tr}(A^H) = \overline{\text{tr}(A)}$
4. $\text{tr}(AB) = \text{tr}(BA)$ 【**重要**】
5. $\text{tr}(AB) \neq \text{tr}(A)\text{tr}(B)$（一般不成立）
6. $\text{tr}(A^n) \neq (\text{tr}(A))^n$（一般不成立）
7. $\text{tr}(I_n) = n$
8. $\text{tr}(A^T A) = A$ 的各元素的平方和

## 經典考題

〔多校〕**證明不存在方陣 $A$、$B$ 使 $AB - BA = I$。**

**解：** 若 $AB - BA = I_n$，則 $\text{tr}(AB - BA) = n$，但 $\text{tr}(AB) - \text{tr}(BA) = 0$，矛盾。

## 相關連結

- [[矩陣定義]]
- [[對稱矩陣與斜對稱矩陣]]
