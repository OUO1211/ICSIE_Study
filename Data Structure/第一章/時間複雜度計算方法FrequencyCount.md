---
subject: Data Structure
status: finished
---

## 定義

**時間複雜度（Time Complexity）** $T(P)$：一個程式 $P$ 所花費的時間，是其編譯時間（compile time）與執行時間（run/execution time）的總和。實務上通常只關注執行時間。

由於直接用系統時鐘（system clock）計時成本太高，故採用 **Frequency Count（頻率計數法）**：計算程式中各敘述的執行次數，作為 machine-independent 的時間估計。

## 核心模型/公式

### Frequency Count 表格法

對每一行敘述，統計：

- **S/E（Steps per Execution）**：該敘述每執行一次所需的 step 數
- **Frequency**：該敘述總共被執行的次數
- **Total steps** = S/E × Frequency

### 範例：矩陣相加 `add(a, b, c, rows, cols)`

```c
void add(int a[][MAX_SIZE], int b[][MAX_SIZE], int c[][MAX_SIZE], int rows, int cols) {
    int i, j;
    for (i = 0; i < rows; i++)
        for (j = 0; j < cols; j++)
            c[i][j] = a[i][j] + b[i][j];
}
```

| Statement | S/E | Frequency | Total steps |
|---|---|---|---|
| `for (i=0; i<rows; i++)` | 1 | rows+1 | rows+1 |
| `for (j=0; j<cols; j++)` | 1 | rows·(cols+1) | rows·(cols+1) |
| `c[i][j]=a[i][j]+b[i][j];` | 1 | rows·cols | rows·cols |
| **Total** | | | $2 \cdot rows \cdot cols + 2 \cdot rows + 1$ |

計數時可在程式中插入 `count++` 於每個迴圈本體與迴圈判斷式結尾，藉此精確追蹤每個敘述的實際執行次數。

去除低階項與常數後，此範例的時間複雜度為 $O(rows \times cols)$，是後續 [[漸近符號O-Omega-Theta|漸近符號]] 分析的基礎。

### 巢狀迴圈直接計數範例

給予下列程式片段，求 `x = x + 1` 之執行次數：

```
For i = 1 to n do
    For j = 1 to i do
        x = x + 1
end;
```

解：內層迴圈執行次數隨 $i$ 而變，總執行次數為

$$
1 + 2 + 3 + \cdots + n = \frac{n(n+1)}{2}
$$

故 Time Complexity $= O(n^2)$。**解題技巧**：巢狀迴圈若內層迴圈上界與外層迴圈變數相關（如 $j$ 跑到 $i$），總次數通常是等差級數求和，可直接套用 $\sum_{i=1}^n i = \frac{n(n+1)}{2}$。
