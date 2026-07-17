## 常見空間的標準基底(standard basis)

> **1. 歐式空間（$\mathbb{R}^n$ 或 $\mathbb{C}^n$）的標準基底：$\{(1,0,0,\cdots,0),(0,1,0,\cdots,0),\cdots,(0,0,0,\cdots,1)\}$。**

例如：
$\{(1,0),(0,1)\}$ 為 $\mathbb{R}^2$ 的標準基底。
$\{(1,0,0),(0,1,0),(0,0,1)\}$ 為 $\mathbb{R}^3$ 的標準基底。

> **Note**
>
> 考慮歐氏空間 $V_F$，其中 $V=\mathbb{C}^n$ 或 $\mathbb{R}^n$，$F=\mathbb{C}$ 或 $\mathbb{R}$，
>
> | $\dfrac{V}{F}$ | 向量空間 | $\dim$ |
> |----|----------|-----|
> | $\mathbb{C}^n/\mathbb{C}$ | 是 |  $n$ |
> | $\mathbb{R}^n/\mathbb{R}$ | 是 | $n$ |
> | $\mathbb{C}^n/\mathbb{R}$ | 是 | $2n$ |
> | $\mathbb{R}^n/\mathbb{C}$ | 不是 | $\times$ |
>
> 例如 $\{(1,0),(0,1),(i,0),(0,i)\}$ 為 $\mathbb{C}^2$ 佈於 $\mathbb{R}$ 的一組基底。

> **2. 矩陣空間（$\mathbb{R}^{m\times n}$ 及 $\mathbb{C}^{m\times n}$）的標準基底：$\{E_{ij}\mid 1\le i\le m,1\le j\le n\}$，其中，$E_{ij}$ 為一 $m\times n$ 矩陣，其元素只在 $(i,j)$ 位置為 $1$，其餘位置為 $0$。**

例如：
$\{E_{11}=\begin{bmatrix}1 & 0\\0 & 0\end{bmatrix},E_{12}=\begin{bmatrix}0 & 1\\0 & 0\end{bmatrix},E_{21}=\begin{bmatrix}0 & 0\\1 & 0\end{bmatrix},E_{22}=\begin{bmatrix}0 & 0\\0 & 1\end{bmatrix}\}$ 為 $\mathbb{R}^{2\times 2}$ 的標準基底且 $\dim(\mathbb{R}^{2\times 2})=4$。

> **3. 多項式空間（$P_n[x]、P[x]$）的標準基底：$\{1,x,x^2,\cdots,x^n\}、\{1,x,x^2,\cdots\}$ 且 $\dim(P_n[x])=n+1$，$\dim(P[x])=\infty$。**

> **Note**
>
> 此處 $P_n[x]$ 收集小於等於 $n$ 次的多項式；有些書上的 $P_n[x]$ 收集小於 $n$ 次的多項式，則其基底為 $\{1,x,x^2,\cdots,x^{n-1}\}$ 而 $\dim(P_n[x])=n$。