---
subject: Data Structure
status: finished
---

## 定義

**主定理（Master Theorem）** 用來快速求解形如

$$
T(n) = aT\left(\frac{n}{b}\right) + f(n)
$$

的遞迴時間函數，其中 $a \geq 1$、$b > 1$ 為常數，$f(n)$ 為漸近正函數（asymptotically positive function）。此類遞迴通常源自「將規模 $n$ 的問題分成 $a$ 個規模 $n/b$ 的子問題，再花 $f(n)$ 時間合併」的分治法（Divide and Conquer）演算法。

相較於 [[遞迴時間函數求解法代入法UnrollingMethod|展開代入法]]，Master Theorem 提供了「查表即得答案」的捷徑，但僅適用於 $a, b$ 為常數、且 $f(n)$ 與 $n^{\log_b a}$ 可比較的情形。

## 核心模型/公式

先計算比較基準 $n^{\log_b a}$，再依 $f(n)$ 與其相對大小分三種情況：

| Case | 條件 | 結論 |
|---|---|---|
| **Case 1** | 存在常數 $\varepsilon>0$，使 $f(n) = O(n^{\log_b a - \varepsilon})$（$f(n)$ **嚴格小於** $n^{\log_b a}$） | $T(n) = \Theta(n^{\log_b a})$ |
| **Case 2** | $f(n) = \Theta(n^{\log_b a})$（$f(n)$ 與 $n^{\log_b a}$ **同階**） | $T(n) = \Theta(n^{\log_b a} \log n)$ |
| **Case 3** | 存在常數 $\varepsilon>0$，使 $f(n) = \Omega(n^{\log_b a + \varepsilon})$（$f(n)$ **嚴格大於** $n^{\log_b a}$），且對足夠大的 $n$ 滿足 regularity condition $a f(n/b) \leq c f(n)$（$c<1$） | $T(n) = \Theta(f(n))$ |

**解題口訣**：比較 $f(n)$ 與 $n^{\log_b a}$ 誰的次方較大，較大者即為 $T(n)$ 的量級；若兩者同階，則多乘一個 $\log n$。

### 例題 1：$T(n) = 2T(n/2) + n^3$

$a=2, b=2, f(n)=n^3$，$n^{\log_b a} = n^{\log_2 2} = n$

$$
\frac{f(n)}{n^{\log_b a}} = \frac{n^3}{n} = n^2 \to f(n) \text{ 遠大於 } n^{\log_b a}
$$

套用 **Case 3**：$T(n) = \Theta(n^3)$

### 例題 2：$T(n) = T(9n/10) + n$

$a=1, b=10/9, f(n)=n$，$n^{\log_b a} = n^{\log_{10/9} 1} = n^0 = 1$

$$
\frac{f(n)}{n^{\log_b a}} = \frac{n}{1} = n \to f(n) \text{ 遠大於 } n^{\log_b a}
$$

套用 **Case 3**：$T(n) = \Theta(n)$

### 例題 3：$T(n) = 16T(n/4) + n^2$

$a=16, b=4, f(n)=n^2$，$n^{\log_b a} = n^{\log_4 16} = n^2$

$$
\frac{f(n)}{n^{\log_b a}} = \frac{n^2}{n^2} = 1 \to f(n) \text{ 與 } n^{\log_b a} \text{ 同階}
$$

套用 **Case 2**：$T(n) = \Theta(n^2 \log n)$

### 例題 4：$T(n) = n + 4T(n/2)$（改用 Master Theorem 驗證展開法結果）

$a=4, b=2, f(n)=n$，$n^{\log_b a} = n^{\log_2 4} = n^2$，$f(n)=n$ 小於 $n^{\log_b a}$

套用 **Case 1**：$T(n) = \Theta(n^2)$（與 [[遞迴時間函數求解法代入法UnrollingMethod|展開代入法]] 所得結果一致）

### 例題 5：$T(n) = 2T(n/2) + n\log n$（Case 2 的推廣型，含 $\log^k n$ 因子）

$a=2, b=2, f(n) = n\log n$，$n^{\log_b a} = n$

$$
\frac{f(n)}{n^{\log_b a}} = \frac{n\log n}{n} = \log n = \log^k n, \quad k=1
$$

套用 **Case 2 推廣式** $T(n) = \Theta(n^{\log_b a} \log^{k+1} n)$：

$$
T(n) = \Theta(n \log^2 n)
$$
