---
subject: Data Structure
status: finished
---

## 定義

**函數成長率排序（Ranking of Growth Rates）**：比較不同時間複雜度函數（如 $n!$、$2^n$、$n^2$、$\log n$ 等）在 $n \to \infty$ 時的相對大小關係，是選擇題中「請將下列 Time Complexity 由高到低排序」的常考題型。

解此類題目的關鍵不是死記排序結果，而是**熟悉一組恆等式（identities）**，將所有函數改寫成可直接比較指數或底數的形式。

## 核心模型/公式

### 常用恆等式

| 編號 | 恆等式 |
|---|---|
| (1) | $(\log n)^{\log n} = n^{\log\log n}$ |
| (2) | $4^{\log n} = n^2$ |
| (3) | $2^{\log n} = n$ |
| (4) | $n^{1/\log n} = 2$（將 (3) 兩邊取 $\frac{1}{\log n}$ 次方：$(2^{\log n})^{1/\log n} = n^{1/\log n}$） |
| (5) | $2^{\sqrt{2\log n}} = n^{\sqrt{2/\log n}}$（利用 (4) 取 $\sqrt{2\log n}$ 次方） |
| (6) | $(\sqrt{2})^{\log n} = \sqrt{n}$（∵ $(\sqrt2)^{\log n} = 2^{\frac12 \log n} = 2^{\log \sqrt n} = \sqrt n$） |
| (7) | $\log(n!) = \Theta(n\log n)$（由 Stirling's formula $n! = \Theta(n^{n+1/2}e^{-n})$ 推得） |
| (8) | $(\log n)! = \Theta\big((\log n)^{\log n + 1/2} e^{-\log n}\big) = \Theta\big((\log n)^{\log n+1/2} n^{-\log e}\big)$ |

### 待比較函數範例

$$
\left(\frac{3}{2}\right)^n,\ (\sqrt2)^{\log n},\ n^2,\ (\log n)!,\ n^3,\ \log^2 n,\ \log(n!),\ 2^{2^n},\ n^{1/\log n},\ \log\log n,
$$
$$
n\cdot 2^n,\ 2^n,\ 2^{\log n},\ (\log n)^{\log n},\ 4^{\log n},\ (n+1)!,\ \sqrt{\log n},\ n!,\ 2^{\sqrt{2\log n}},\ n,\ n\log n,\ 1
$$

**解題技巧**：

1. 先用恆等式 (3)(6) 把 $2^{\log n}$、$(\sqrt2)^{\log n}$ 之類的式子化簡成 $n$ 的多項式（$n$、$\sqrt n$），才能與 $n^2, n^3$ 等直接比較次方高低。
2. 含 $\log\log n$、$n^{1/\log n}$ 的式子通常趨近常數或極慢成長，排序上接近 $1$。
3. 含 $n!$、$(n+1)!$、$2^{2^n}$ 的式子成長最快，通常排在最上端；一般排序由高到低約略為：
$2^{2^n} > (n+1)! > n! > n \cdot 2^n > 2^n > \left(\frac32\right)^n > n^3 > n^2 = 4^{\log n} > n\log n > n = 2^{\log n} > (\log n)^{\log n} = n^{\log\log n} > \log(n!) = \Theta(n\log n)\text{（與 }n\log n\text{ 同階）} > \log^2 n > \sqrt{\log n} > \log\log n > n^{1/\log n}=2 > 1$

（含 $(\log n)!$、$2^{\sqrt{2\log n}}$ 等特殊項需個別代入恆等式 (5)(8) 化簡後再插入排序，實際排序請以化簡後的指數/次方大小為準，不要死背名次。）
