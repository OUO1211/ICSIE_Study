### 特殊矩陣的行列式－Vandermonde 矩陣

> **定義**
>
> 若 $\forall i$，$x_i \neq 0$，則
>
> $$\begin{vmatrix} 1 & 1 & 1 & \cdots & 1 \\ x_1 & x_2 & x_3 & \cdots & x_n \\ x_1^2 & x_2^2 & x_3^2 & \cdots & x_n^2 \\ \vdots & \vdots & \vdots & & \vdots \\ x_1^{n-1} & x_2^{n-1} & x_3^{n-1} & \cdots & x_n^{n-1} \end{vmatrix} = \prod_{1 \leq i < j \leq n} (x_j - x_i)$$
>
> 【108 中正數學】

對 $n$ 做歸納法：

$n = 2$ 時顯然成立。

設對 $(n-1)$ 階的 Vandermonde 矩陣，命題都成立，

則對 $n \times n$ 的 Vandermonde 矩陣，

$$\begin{vmatrix} 1 & 1 & 1 & \cdots & 1 \\ x_1 & x_2 & x_3 & \cdots & x_n \\ x_1^2 & x_2^2 & x_3^2 & \cdots & x_n^2 \\ \vdots & & & & \vdots \\ x_1^{n-1} & x_2^{n-1} & x_3^{n-1} & \cdots & x_n^{n-1} \end{vmatrix}$$

$$\xrightarrow{c_j - x_1 c_{j-1}} \begin{vmatrix} 1 & 0 & 0 & \cdots & 0 \\ x_1 & x_2 - x_1 & x_3 - x_1 & \cdots & x_n - x_1 \\ x_1^2 & x_2^2 - x_1 x_2 & x_3^2 - x_1 x_3 & \cdots & x_n^2 - x_1 x_n \\ \vdots & \vdots & \vdots & & \vdots \\ x_1^{n-1} & x_2^{n-1} - x_1 x_2^{n-2} & x_3^{n-1} - x_1 x_3^{n-2} & \cdots & x_n^{n-1} - x_1 x_n^{n-2} \end{vmatrix}$$

$$= \left(\prod_{j=2}^{n}(x_j - x_1)\right) \begin{vmatrix} 1 & 1 & \cdots & 1 \\ x_2 & x_3 & \cdots & x_n \\ x_2^2 & x_3^2 & \cdots & x_n^2 \\ \vdots & & & \vdots \\ x_2^{n-2} & x_3^{n-2} & \cdots & x_n^{n-2} \end{vmatrix} = \left(\prod_{j=2}^{n}(x_j - x_1)\right)\left(\prod_{2 \leq i < j \leq n}(x_j - x_i)\right) = \prod_{1 \leq i < j \leq n}(x_j - x_i)$$

> **Note**
>
> $$\begin{vmatrix} x_1 & x_2 & \cdots & x_n \\ x_1^2 & x_2^2 & \cdots & x_n^2 \\ \vdots & & & \vdots \\ x_1^n & x_2^n & \cdots & x_n^n \end{vmatrix}$$
>
> 也有上述結果。
