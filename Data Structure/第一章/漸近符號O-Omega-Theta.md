---
subject: Data Structure
status: finished
---

## 定義

**漸近符號（Asymptotic Notation）** 用來描述函數在輸入規模趨近無窮大時的成長趨勢，忽略常數與低階項。

- **Big-Oh（$O$，上界）**：$f(n) = O(g(n))$，讀作 "f of n is big oh of g of n"，若存在正常數 $c$ 與 $n_0$，使得對所有 $n \geq n_0$，皆有
$$
f(n) \leq c \cdot g(n)
$$
即 $g(n)$ 是 $f(n)$ 的一個漸近**上界**。

- **Big-Omega（$\Omega$，下界）**：$f(n) = \Omega(g(n))$，若存在正常數 $c$ 與 $n_0$，使得對所有 $n \geq n_0$，皆有
$$
f(n) \geq c \cdot g(n)
$$
即 $g(n)$ 是 $f(n)$ 的一個漸近**下界**。

- **Big-Theta（$\Theta$，緊界）**：$f(n) = \Theta(g(n))$，若同時存在正常數 $c_1, c_2, n_0$，使得對所有 $n \geq n_0$，皆有
$$
c_1 \cdot g(n) \leq f(n) \leq c_2 \cdot g(n)
$$
即 $g(n)$ 同時是 $f(n)$ 的上界與下界，$\Theta$ 是三者中**最精確**的描述。

## 核心模型/公式

### Big-Oh 範例

1. $3n + 2 = O(n)$　∵ $3n+2 \leq 4n$，for all $n \geq 2$（取 $c=4, n_0=2$）
2. $100n + 6 = O(n)$　∵ $100n+6 \leq 101n$，for $n \geq 10$（取 $c=101, n_0=10$）
3. $10n^2 + 4n + 2 = O(n^2)$　∵ $10n^2+4n+2 \leq 11n^2$，for $n \geq 5$

摘要：$O(1)$ 為常數時間，$O(n)$ 為線性時間。

### Big-Theta 範例

1. $3n+2 = \Theta(n)$　∵ $3n \leq 3n+2 \leq 4n$，for all $n \geq 2$
2. $10n^2+4n+2 = \Theta(n^2)$
3. $10\log n + 4 = \Theta(\log n)$
4. 反例：$6 \cdot 2^n + n^2 \neq \Theta(1)$，$3n+3 \neq \Theta(n^2)$，$10n^2+4n+3 \neq \Theta(n)$

### 漸近符號的性質（考選擇題常考）

| 性質 | 內容 |
|---|---|
| **Transitivity（遞移律）** | $f(n)=\Theta(g(n))$ 且 $g(n)=\Theta(h(n))$ $\Rightarrow$ $f(n)=\Theta(h(n))$；$O$ 與 $\Omega$ 亦同 |
| **Reflexivity（反身律）** | $f(n)=\Theta(f(n))$；$O$、$\Omega$ 亦同 |
| **Symmetry（對稱律）** | $f(n)=\Theta(g(n))$ iff $g(n)=\Theta(f(n))$ |
| **Transpose Symmetry（轉置對稱律）** | $f(n)=O(g(n))$ iff $g(n)=\Omega(f(n))$ |

**解題技巧**：$\Theta$ 比 $O$、$\Omega$ 更精確，因為它同時限制了上界與下界；若題目要求「最精確」描述成長率，答案通常是 $\Theta$ 而非 $O$。
