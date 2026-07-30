---
subject: Data Structure
status: finished
---

## 定義

**排列組合生成（Permutation Generation）**：給定 $n \geq 1$ 個元素所成的集合，印出此集合的所有可能排列。$n$ 個相異元素共有 $n!$ 種排列。

屬於 [[遞迴Recursion基礎與範例分類|遞迴]] 的「其他類」經典範例，核心設計概念是**固定第一個位置的元素，遞迴地對剩餘元素生成排列**。

## 核心模型/公式

### 範例：$\{a, b, c\}$ 的所有排列

$$
(a,b,c) \ (a,c,b) \ (b,a,c) \ (b,c,a) \ (c,a,b) \ (c,b,a)
$$

### 遞迴設計概念：$\{a, b, c, d\}$

將排列生成拆解為 4 個子問題：

1. `a` 開頭，後接 $\{b,c,d\}$ 的所有排列
2. `b` 開頭，後接 $\{a,c,d\}$ 的所有排列
3. `c` 開頭，後接 $\{a,b,d\}$ 的所有排列
4. `d` 開頭，後接 $\{a,b,c\}$ 的所有排列

### 遞迴演算法（原地交換法）

```c
void perm(char *list, int i, int n)
/* Generate all permutations of list[i] to list[n] */
{
    int j;
    if (i == n) {
        /* 已排到最後一個位置，輸出目前排列 */
        for (j = 0; j <= n; j++) printf("%c", list[j]);
        printf("\n");
    } else {
        /* list[i] 依序與 list[i..n] 中每個元素交換，遞迴排列剩餘元素 */
        for (j = i; j <= n; j++) {
            SWAP(list[i], list[j]);
            perm(list, i+1, n);
            SWAP(list[i], list[j]); /* 交換回來，恢復原順序 */
        }
    }
}
```

**時間複雜度**：$n$ 個元素的排列演算法時間複雜度為 $O(n \cdot n!)$（共 $n!$ 種排列，每種輸出需 $O(n)$）。
