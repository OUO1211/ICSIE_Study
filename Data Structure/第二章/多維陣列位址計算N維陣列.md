---
subject: Data Structure
status: finished
---

## 定義

**多維陣列（N-dimensional Array）**：宣告方式為 $A(1:\mu_1, 1:\mu_2, \cdots, 1:\mu_n)$，其中 $\mu_k$ 為第 $k$ 維的大小。將 [[二維陣列位址計算RowColumnMajor|二維陣列的 Row-major／Column-major 位址公式]] 推廣到 $n$ 維，即可得到通用的多維陣列位址公式。

## 核心模型/公式

設 $A(1,1,\cdots,1)$ 的位址為 $L_0$，元素大小 $d=1$。

### Row-major（以最後一維變動最快）

$$
\text{Loc}\big(A(i_1, i_2, \cdots, i_n)\big) = L_0 + \sum_{j=1}^{n} (i_j - 1)\, a_j
$$

其中

$$
a_j = \prod_{k=j+1}^{n} \mu_k \quad (1 \leq j \leq n), \qquad a_n = 1
$$

推導邏輯：固定前面維度不變，只變動最後一維 $i_n$ 時，每增加 1 位移量最小；固定 $i_1$ 不變，變動 $i_2,\ldots,i_n$ 需跳過 $\mu_2\mu_3\cdots\mu_n$ 個位置，依此類推逐維展開。

### Column-major（以第一維變動最快）

$$
\text{Loc}\big(A(i_1, i_2, \cdots, i_n)\big) = L_0 + \sum_{j=1}^{n} (i_j - 1)\, a_j
$$

其中

$$
a_j = \prod_{k=1}^{j-1} \mu_k \quad (2 \leq j \leq n), \qquad a_1 = 1
$$

推導邏輯：視為有 $\mu_n$ 個 $(n-1)$ 維陣列、每個 $(n-1)$ 維陣列又有 $\mu_{n-1}$ 個 $(n-2)$ 維陣列……以此類推，第一維 $i_1$ 每增加 1 位移量最小。

**解題技巧**：

1. Row-major 與 Column-major 的公式結構完全對稱——只是 $a_j$ 的連乘方向相反：Row-major 的權重 $a_j$ 是「該維度**之後**所有維度大小的連乘積」；Column-major 的權重 $a_j$ 是「該維度**之前**所有維度大小的連乘積」。
2. 二維陣列公式是此通用公式在 $n=2$ 時的特例：Row-major 時 $a_1 = \mu_2 = n$（行數）、$a_2=1$；與 [[二維陣列位址計算RowColumnMajor]] 中的公式一致。
3. 元素大小 $d \neq 1$ 時，只需將整個 $\sum (i_j-1)a_j$ 乘上 $d$ 即可。
