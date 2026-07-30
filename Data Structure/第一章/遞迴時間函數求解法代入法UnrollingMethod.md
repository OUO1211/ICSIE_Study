---
subject: Data Structure
status: finished
---

## 定義

**遞迴時間函數（Recurrence Relation）**：描述遞迴演算法時間複雜度的方程式，形如 $T(n) = \cdots T(\text{較小規模}) \cdots$，並附上邊界條件（如 $T(1)=1$）。求解此類方程式常用兩種手法：

1. **展開代入法（Unrolling / Substitution）**：反覆將 $T$ 的遞迴部分代入自身，觀察規律後歸納出通式。
2. **猜測驗證法（Guess-and-Verify）**：先猜測解的形式，再用數學歸納法代入驗證是否成立。

與 [[MasterTheorem主定理]] 相比，代入法適用範圍更廣（包含 Master Theorem 無法處理的型態，如 $T(n)=T(\sqrt{n})+1$），但需要較強的觀察與歸納能力。

## 核心模型/公式

### 型態一：$T(n) = T(n/2) + 1$

$$
T(n) = T\left(\frac{n}{2}\right) + 1 = T\left(\frac{n}{4}\right) + 2 = \cdots = T\left(\frac{n}{n}\right) + \log_2 n = T(1) + \log_2 n
$$

$$
\therefore T(n) = O(\log n)
$$

### 型態二：$T(n) = 2T(n/2) + n$，$T(1)=1$

$$
T(n) = O(n \log n)
$$

### 型態三：$T(n) = T(n-1) + n$，$T(0)=0$

$$
T(n) = O(n^2)
$$

### 型態四：$T(n) = 2T(n-1) + 1$，$T(1)=1$

$$
T(n) = 2^n - 1 = O(2^n)
$$

### 型態五：$T(n) = T(\sqrt{n}) + 1$，$T(2)=1$

$$
T(n) = T(n^{1/2}) + 1 = T(n^{1/4}) + 2 = T(n^{1/8}) + 3 = \cdots = T(2) + i
$$

其中 $n^{1/2^i} = 2 \Rightarrow \frac{1}{2^i}\log n = 1 \Rightarrow 2^i = \log n \Rightarrow i = \log\log n$

$$
\therefore T(n) = O(\log\log n)
$$

### 型態六（一般型，含係數）：$T(n) = n + 4T(n/2)$

$$
\begin{aligned}
T(n) &= n + 4\left(\frac{n}{2} + 4T\left(\frac{n}{4}\right)\right) = n + 2n + 4n + \cdots + 4^{\log n}T(1) \\
&= n\left(\sum_{k=0}^{\log n - 1} 2^k\right) + \Theta(n^2) = n \cdot \frac{2^{\log n}-1}{2-1} + \Theta(n^2) \\
&= \Theta(n^2) + \Theta(n^2) = \Theta(n^2)
\end{aligned}
$$

### 猜測驗證法範例：$T(n) = 2T(\lfloor n/2 \rfloor) + n$

猜測 $T(n) = O(n\log n)$，假設對 $\lfloor n/2 \rfloor$ 成立，即 $T(\lfloor n/2\rfloor) \leq c\lfloor n/2\rfloor \log\lfloor n/2\rfloor$：

$$
\begin{aligned}
T(n) &\leq 2\left(c\left\lfloor\frac{n}{2}\right\rfloor \log\left\lfloor\frac{n}{2}\right\rfloor\right) + n \\
&\leq cn\log\left(\frac{n}{2}\right) + n = cn\log n - cn\log 2 + n = cn\log n - cn + n \leq cn\log n
\end{aligned}
$$

驗證成立，故 $T(n) = O(n\log n)$。此技巧亦適用於邊界項不整除的情形，例如 $T(n) = 2T(\lfloor n/2\rfloor + 17) + n$：當 $n$ 很大時，$T(\lfloor n/2\rfloor)$ 與 $T(\lfloor n/2\rfloor+17)$ 差異可忽略，故仍猜測 $T(n)=O(n\log n)$。

**解題技巧**：展開代入法的關鍵是找出「展開到第幾層會碰到邊界條件」，這個層數通常就是 $\log$ 的次方數；猜測驗證法則適合處理係數不乾淨（如 $\lfloor n/2\rfloor + 17$）而無法直接套用 [[MasterTheorem主定理|Master Theorem]] 的情形。
