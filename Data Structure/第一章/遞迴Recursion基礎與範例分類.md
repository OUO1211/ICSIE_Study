---
subject: Data Structure
status: finished
---

## 定義

**遞迴（Recursion）**：一個函數（或程序）在其定義中直接或間接呼叫自己的技巧。設計遞迴演算法時，必須具備兩個要素：

- **終止條件（Base Case）**：不再遞迴呼叫、直接給出結果的邊界情況，用來停止遞迴。
- **遞迴呼叫（Recursive Case）**：將原問題拆解成規模更小、但形式相同的子問題，並呼叫自身求解。

若缺少終止條件，遞迴會無窮呼叫下去，最終導致 stack overflow。

## 核心模型/公式

### 考研常見遞迴題型分類

1. **數學類**：階乘（Factorial）、二項式係數（Binomial Coefficient）、Ackermann's Function、費氏數列（Fibonacci）。
2. **資結類**：遞迴版二分搜尋法（Recursive Binary Search）、Linked List／Tree／Graph 的遞迴走訪。
3. **其他類**：排列組合（Permutation）、河內塔（Tower of Hanoi）。

### 遞迴呼叫的系統負擔

每一次遞迴呼叫，compiler 都必須將下列資訊存入 system stack：

1. 參數（Parameters）
2. 區域變數（Local Variables）
3. 回傳位址（Return Address）

因此遞迴呼叫次數越多，所需的堆疊空間（[[效能分析與空間複雜度SpaceComplexity|Space Complexity]]）也越大，這也是遞迴法在空間效率上常受質疑之處。

### 本章遞迴範例對照表

| 類型 | 範例 | 備註 |
|---|---|---|
| 數學類 | [[階乘與二項式係數遞迴Factorial-Binomial]] | 例題 1-3～1-6 |
| 數學類 | [[Ackermann函數]] | 例題 1-7 |
| 資結類 | [[選擇排序與二分搜尋法]] | 例題 1-1、1-2、1-9 |
| 其他類 | [[排列組合遞迴生成Permutations]] | 例題 1-10 |
