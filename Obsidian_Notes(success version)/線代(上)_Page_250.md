$$= \begin{vmatrix} x_2 - x_1 & x_3 - x_1 & \cdots & x_{k+1} - x_1 \\ x_2^2(x_2 - x_1) & x_3^2(x_3 - x_1) & \cdots & x_{k+1}^2(x_{k+1} - x_1) \\ \vdots & \vdots & & \vdots \\ x_2^{k-1}(x_2 + x_1) & x_3^{k-1}(x_3 + x_1) & \cdots & x_{k+1}^{k-1}(x_{k+1} + x_1) \end{vmatrix}$$

$$= \prod_{i=2}^{k+1}(x_i - x_1) \begin{vmatrix} 1 & 1 & \cdots & 1 \\ x_2 + x_1 & x_3 + x_1 & \cdots & x_{k+1} + x_1 \\ \vdots & \vdots & & \vdots \\ x_2^{k-1} + \cdots & x_3^{k-1} + \cdots & \cdots & x_{k+1}^{k-1} + \cdots \end{vmatrix}$$

$$= \prod_{i=2}^{k+1}(x_i - x_1) \cdot \sum_{j=2}^{k+1} \begin{vmatrix} 1 & 1 & \cdots & 1 \\ x_2 & x_3 & \cdots & x_{k+1} \\ \vdots & \vdots & & \vdots \\ x_2^{k-1} & x_3^{k-1} & \cdots & x_{k+1}^{k-1} \end{vmatrix}$$

$$= \prod_{i=2}^{k+1}(x_i - x_1) \cdot \sum_{j=2}^{k+1} \prod_{2 \leq i < j \leq k+1}(x_j - x_i)$$

$$= \sum_{j=2}^{k+1}\prod_{i=2}^{k+1}(x_i - x_1) \cdot \prod_{2 \leq i < j \leq k+1}(x_j - x_i) = \sum_{j=1}^{k+1}\prod_{1 \leq i < j \leq k+1}(x_j - x_i) = \text{右式}$$

---

> **試題 21**
>
> $$\det\begin{bmatrix} (2n-1)^2 & (2n-2)^2 & \cdots & n^2 & (2n)^2 \\ (2n-1)^n & (2n-2)^n & \cdots & n^n & (2n)^n \\ \vdots & \vdots & & \vdots & \vdots \\ 2n-1 & 2n-2 & \cdots & n & 2n \\ 1 & 1 & \cdots & 1 & 1 \end{bmatrix} = ?$$

**解** 跨第 1 列第 $\sim$ 1 列互換；跨第 2 列第 $\sim$ 2 列互換；跨第 3 列第 $\sim$ $-1$ 列互換……

跨第 1 行第 $\sim$ 1 行互換；跨第 2 行第 $\sim$ 2 行互換；跨第 $-1$ 行第 $\sim$ $-2$ 行互換……
