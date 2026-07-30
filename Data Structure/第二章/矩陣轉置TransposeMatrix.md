---
subject: Data Structure
status: finished
---

## 定義

**轉置矩陣（Transpose Matrix）**：$A \rightarrow A^t$，即 $a_{ij} \rightarrow a_{ji}$（列與行互換）。當矩陣以**稀疏矩陣的三元組（row, col, value）陣列**表示時，轉置不能單純逐一搬移，需特別設計演算法才能維持結果依序排列。

## 核心模型/公式

### 演算法一：依原陣列順序搬移（不可行）

```
for each row i do
    take element(i, j, value) from A
    and store it in (j, i, value) of At
end;
```

**問題**：原陣列 $A$ 是依 row 排序，搬移後的結果理應依新的 row（即原本的 column）排序，但逐一搬移時無法預先知道每個新 row 在結果陣列中該放的位置——例如搬移 $(1,6,-15) \to (6,1,-15)$ 時，尚未掃完整個陣列，不知道 $(6,1,-15)$ 之後是否還有更小 row 的元素要插入它前面。此法行不通。

### 演算法二：依 Column 順序搬移（可行但較慢）

```
for all elements in column j do
    place element(i, j, value)
    and store it in position(j, i, value)
end;
```

改為逐欄（column）搜尋整個 $A$，依序取出屬於該 column 的元素搬入結果，即可保證結果依序排列。

**複雜度分析**：設 $A$ 為 $n$ 個 columns、$t$ 個非零項：

- 外層「依 column 掃描」需執行 $n$ 次；
- 每次外層都要重新掃描整個陣列找出屬於該 column 的元素，內層需執行 $t$ 次；
- 故總時間複雜度為 $O(nt)$。
- 當非零項數量與 $n \times m$ 同數量級（$t = nm$）時，退化為 $O(n^2 m)$，比直接用二維陣列做轉置的 $O(nm)$ 還差。

### 演算法三：Fast Transpose（快速轉置）

**核心概念**：先統計每個 column 各有幾個非零項（`row_terms`），再用累加的方式算出每個 column 在結果陣列中應該從哪個位置開始擺放（`starting_pos`），如此只需掃描原陣列**一次**即可把每個元素直接放到正確位置，不必重複搜尋。

Step 1：計算每個 column（即轉置後的 row）含有的非零項數 `row_terms[j]`。

Step 2：依 `row_terms` 累加，算出每個 column 對應的起始位置 `starting_pos[j] = starting_pos[j-1] + row_terms[j-1]`。

Step 3：掃描原陣列 $A$ 一次，對每個元素 $(i,j,value)$，依 `starting_pos[j]` 決定其在結果陣列 $B$ 中的位置，放入後將 `starting_pos[j]` 加一（讓同一 column 的下一個元素接續放在後面）。

```c
void fast_transpose(term a[], term b[]) {
    /* the transpose of a is placed in b */
    int row_terms[MAX_COL], starting_pos[MAX_COL];
    int i, j, num_cols = a[0].col, num_terms = a[0].value;
    b[0].row = num_cols;
    b[0].col = a[0].row;
    b[0].value = num_terms;
    if (num_terms > 0) {          /* nonzero matrix */
        /* Step 1: 統計各 column 的非零項數 */
        for (i = 0; i < num_cols; i++) row_terms[i] = 0;
        for (i = 1; i <= num_terms; i++) row_terms[a[i].col]++;
        /* Step 2: 累加求各 column 的起始位置 */
        starting_pos[0] = 1;
        for (i = 1; i < num_cols; i++)
            starting_pos[i] = starting_pos[i-1] + row_terms[i-1];
        /* Step 3: 掃描一次 A，直接放入 B 對應位置 */
        for (i = 1; i <= num_terms; i++) {
            j = starting_pos[a[i].col]++;
            b[j].row = a[i].col;
            b[j].col = a[i].row;
            b[j].value = a[i].value;
        }
    }
}
```

**複雜度分析**：4 個迴圈分別執行 $n$、$t$、$n-1$、$t$ 次，故時間複雜度為 $O(n+t)$；當 $t = nm$ 時退化為 $O(nm)$，與直接用二維陣列轉置相同，但一般情況（$t$ 遠小於 $nm$）下遠優於演算法二的 $O(nt)$。

**解題技巧**：三種演算法的效率排序為 **Fast Transpose $O(n+t)$ ＜ 演算法二 $O(nt)$**；核心差異在於 Fast Transpose 用「事先統計 + 累加位置」的技巧，把「重複搜尋」換成「一次線性掃描」。
