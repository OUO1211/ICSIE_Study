# 1-2 列運算與行運算

## 基本列運算 (elementary row operation)

> **定義：基本列運算**
>
> 給定矩陣 $A$，
>
> (1) 第一型列運算：以 $r_{ij}(A)$ 表將 $A$ 的第 $i$ 列與第 $j$ 列對調。
>
> (2) 第二型列運算：以 $r_i^{(k)}(A)$ 表將 $A$ 的第 $i$ 列的元素均乘以 $k$，$k \neq 0$。
>
> (3) 第三型列運算：以 $r_{ij}^{(k)}(A)$ 表將 $A$ 的第 $i$ 列中的元素乘以 $k$ 後，加到第 $j$ 列。

**Note**

(1) 通常從 $A \xrightarrow{r} B$，表對 $A$ 做列運算 $r$ 而得到 $B$。

(2) 若矩陣 $A$ 可經由若干列運算得到矩陣 $B$，則稱 $A$ 與 $B$ 列等價，記作 $A \sim B$。

例如：

$$A = \begin{bmatrix} 1 & 4 \\ 2 & 5 \\ 3 & 6 \end{bmatrix}, \quad r_{12}(A) = \begin{bmatrix} 2 & 5 \\ 1 & 4 \\ 3 & 6 \end{bmatrix}, \quad r_1^{(3)}(A) = \begin{bmatrix} 1 & 4 \\ 2 & 5 \\ 3 & 6 \end{bmatrix} \xrightarrow{r_1^{(3)}} \begin{bmatrix} 3 & 12 \\ 2 & 5 \\ 1 & 2 \end{bmatrix}$$

$$B = \begin{bmatrix} 1 & 4 & 5 & 6 \\ 2 & 0 & 1 & 2 \\ 3 & 0 & 2 & 3 \end{bmatrix} \xrightarrow{r_{21}^{(2)}} \begin{bmatrix} 1 & 4 & 5 & 6 \\ 4 & 5 & 6 \end{bmatrix} \xrightarrow{r_{21}^{(-2)}} \begin{bmatrix} 1 & 4 & 5 & 6 \\ 0 & -8 & -9 & -10 \\ 0 & -24 & -26 & -30 \end{bmatrix}$$

$$C = \begin{bmatrix} 1 & 0 & 1 \\ 2 & 2 & 0 \\ 3 & 4 & 0 \end{bmatrix} \xrightarrow{} \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$$

(3) 此三種運算皆為可逆的運算：$(r_g)^{-1} = r_g$；$(r_i^{(k)})^{-1} = r_i^{(1/k)}$；$(r_{ij}^{(k)})^{-1} = r_{ij}^{(-k)}$。

(4) 運算關係保具反身性、對稱性、遞移性（即為等價關係）。

(5) 對單位矩陣做列運算所得矩陣為基本列矩陣：$R_{ij} = r_{ij}(I)$，$R_i^{(k)} = r_i^{(k)}(I)$，$R_{ij}^{(k)} = r_{ij}^{(k)}(I)$。

(6) 基本列矩陣均可逆且 $(R_{ij})^{-1} = R_{ij}$，$(R_i^{(k)})^{-1} = R_i^{(1/k)}$，$(R_{ij}^{(k)})^{-1} = R_{ij}^{(-k)}$。

(7) 對矩陣 $A$ 作列運算等於在 $A$ 的**左邊**上對應的列基本矩陣：

（即 $B = r_{ij}(A) = R_{ij} A$，$B = r_i^{(k)}(A) = R_i^{(k)} A$，$B = r_{ij}^{(k)}(A) = R_{ij}^{(k)} A$）

(8) $A$ 列等價於 $B \Leftrightarrow$ 存在一可逆矩陣 $P$ 使 $B = PA$。

例如：

$$A = \begin{bmatrix} 1 & 3 & 5 \\ 2 & 4 & 6 \end{bmatrix}, \quad R_{12} = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}, \quad R_1^{(-2)} = \begin{bmatrix} 1 & 0 \\ 0 & -2 \end{bmatrix}, \quad R_{12}^{(-2)} = \begin{bmatrix} 1 & 0 \\ -2 & 1 \end{bmatrix}$$
