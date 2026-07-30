---
subject: Data Structure
status: finished
---

## 定義

**效能評估（Performance Evaluation）** 分為兩類：

- **Performance Analysis（效能分析）**：估算程式執行所需的時間與空間，屬於 machine-independent 的理論估計，即 Complexity Theory。
- **Performance Measurement（效能量測）**：實際量測程式在特定機器上的執行時間，屬於 machine-dependent。

**空間複雜度（Space Complexity）**：一個程式從開始執行到結束，所需要的記憶體總量。

## 核心模型/公式

### Space Complexity 的組成

$$
S(P) = c + S_P(\text{instance characteristics})
$$

- **固定部分（Fixed Part）** $c$：與輸入實例無關，例如指令、簡單變數、固定大小的變數所佔空間。
- **變動部分（Variable Part）** $S_P$：與特定輸入實例相關，例如遞迴呼叫的堆疊空間、動態配置的空間。

### 範例：陣列傳遞方式對 Space Complexity 的影響

對函數 `sum(list, n)`（計算陣列元素總和）：

| 傳遞方式 | 說明 | Space Complexity |
|---|---|---|
| **Call-by-value** | 整個陣列被複製到 temporary storage | $S_{sum}(n) = O(n)$ |
| **Call-by-address** | 只傳遞陣列第一個元素的位址 | $S_{sum}(n) = O(1)$（不含遞迴時每層呼叫的固定負擔） |

### 範例：遞迴函數的空間複雜度計算

```c
float rsum(float list[], int n) {
    if (n != 0) return rsum(list, n-1) + list[n-1];
    return list[0];
}
```

假設 `int`、`pointer` 各佔 2 bytes，`float` 佔 4 bytes，`list[]` 採 call-by-address 傳遞。每次遞迴呼叫，system stack 需儲存：

| Type | Name | Bytes |
|---|---|---|
| Parameter = pointer (float list[]) | list[] | 2 |
| Parameter = integer | n | 2 |
| Return address | — | 2 |

每次遞迴呼叫需 $6$ bytes，共 $n$ 次遞迴呼叫，故：

$$
\text{Space Complexity} = O(6n) = O(n)
$$

**解題技巧**：計算遞迴函數空間複雜度的關鍵，是先列出每次呼叫需存入 stack 的（參數 + 區域變數 + 回傳位址）位元組數，再乘上總遞迴呼叫次數。
