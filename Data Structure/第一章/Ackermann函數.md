---
subject: Data Structure
status: finished
---

## 定義

**Ackermann's Function** $A(m, n)$ 是一個成長速度極快、且不能用單純迴圈（非遞迴）改寫的著名遞迴函數，常用來說明「遞迴的表達能力超越簡單迭代」。定義如下：

$$
A(m, n) = \begin{cases}
n + 1 & \text{, if } m = 0 \\
A(m-1, 1) & \text{, if } n = 0 \\
A(m-1, A(m, n-1)) & \text{, otherwise}
\end{cases}
$$

屬於 [[遞迴Recursion基礎與範例分類|遞迴]] 的數學類經典範例，是雙參數遞迴（同時對 $m$、$n$ 遞減）的代表題型。

## 核心模型/公式

### 遞迴演算法

```
Procedure Ack(int n, int m) {
    if (m == 0) return (n + 1);
    else if (n == 0) return Ack(m-1, 1);
    else return Ack(m-1, Ack(m, n-1));
}
```

### 經典例題

$$
A(2, 2) = 7
$$

### 練習

$$
A(2,1) = 5, \quad A(1,2) = 4, \quad A(2,3) = 9
$$

**解題技巧**：Ackermann's Function 的展開通常需要先固定 $m$、逐步降低 $n$；當遇到第三個分支 $A(m-1, A(m, n-1))$ 時，要先算內層 $A(m, n-1)$ 得到一個數值 $k$，再代入外層 $A(m-1, k)$，逐層向下遞迴直到 $m=0$ 或 $n=0$ 觸底。
