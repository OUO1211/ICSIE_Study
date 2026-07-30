---
subject: Data Structure
status: finished
---

## 定義

陣列元素在記憶體中實際上是**一維連續空間**，多維陣列必須先決定「線性化」的順序，才能算出每個元素的位址：

- **Row-major（以列為主）**：先存完第一列所有元素，再存第二列……逐列（row by row）存放。
- **Column-major（以行為主）**：先存完第一行所有元素，再存第二行……逐行（column by column）存放。

**一維陣列 $A(1:m)$ 位址公式**：若起始位址為 $L_0$，每個元素佔 $d$ 個空間，則

$$
\text{Loc}(A(i)) = L_0 + (i-1) \cdot d
$$

## 核心模型/公式

### 二維陣列 $A(1:m, 1:n)$ 位址公式（元素大小 $d$，起始位址 $L_0$）

$$
\text{Row-major：} \quad \text{Loc}(A(i,j)) = L_0 + \big[(i-1) \cdot n + (j-1)\big] \cdot d
$$

$$
\text{Column-major：} \quad \text{Loc}(A(i,j)) = L_0 + \big[(j-1) \cdot m + (i-1)\big] \cdot d
$$

其中 $m$ 為總列數、$n$ 為總行數。

### 判斷 Row-major 或 Column-major 的原則

給定兩個已知位址，欲反推公式：

$$
\text{Row-major} \Rightarrow \text{可求出 } L_0 \text{ 及行數 } n \text{（但列數不需知道）}
$$
$$
\text{Column-major} \Rightarrow \text{可求出 } L_0 \text{ 及列數 } m \text{（但行數不需知道）}
$$

**解題技巧**：拿到題目先判斷是哪種排列方式，再設未知數（通常是 $n$ 或 $m$ 與 $d$）列聯立方程式求解。

### 範例：陣列宣告含負索引（例題 2-1、2-2）

Row-major、元素大小 $d$、起始位址 $L_0=100$：宣告 `A: array[-4..3, -3..2]`，$m = 3-(-4)+1=8$，$n = 2-(-3)+1=6$：

$$
A(1,1) = 100 + \big[(1-(-4)) \cdot 6 + (1-(-3))\big] \cdot 1 = 134
$$

**解題技巧**：索引範圍為 $[lo, hi]$ 時，總數為 $hi - lo + 1$；下限非 1（如從 $-4$ 開始）時，公式中的 $(i-1)$ 要改成 $(i - lo)$。

### 範例：已知兩點位址反推 Row-major 公式（例題 2-8）

二維陣列 $B(1{:}m, 1{:}n)$，已知 $B(2,3)$ 位址為 18、$B(3,2)$ 位址為 28、$B(1,1)$ 位址為 2，求 $B(4,5)$。

$$
\begin{aligned}
18 &= 2 + \big[(2-1)n + (3-1)\big] d \\
28 &= 2 + \big[(3-1)n + (2-1)\big] d
\end{aligned}
$$

解聯立得 $d=2, n=6$，代入：

$$
B(4,5) = 2 + \big[(4-1) \cdot 6 + (5-1)\big] \cdot 2 = 46
$$

### 範例：已知兩對角點位址（$i=j$ 情形，例題 2-5）

$A(1,1)=1204$，$A(3,3)=1244$，$d=1$，因對角線上 $i=j$，Row-major 與 Column-major 算法相同：

$$
A(3,3) = A(1,1) + (3-1)\cdot n \cdot d + (3-1)\cdot d \Rightarrow 1244 = 1204 + 2n + 2 \Rightarrow n = 19
$$

$$
A(4,4) = A(1,1) + (4-1)\cdot 19 \cdot 1 + (4-1)\cdot 1 = 1204 + 57 + 3 = 1264
$$

**解題技巧**：若已知的兩點恰好落在對角線（$i=j$），無法直接判斷是 Row-major 還是 Column-major，但因公式對稱、算法一致，可直接套用任一方向的公式求解。
