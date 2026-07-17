## 第 4 章 線性映射 577

> **試題 3**
>
> (10%) Given an input image whose constituting pixels with integer coordinates represented by the Cartesian product $[0,700] \times [0,500]$, it will be transformed to new coordinates represented by $[-1,1] \times [-1,1]$ for a certain purpose as Figure 1 shows. Please find the transformation matrix to achieve such a normalization process.
>
> 【100 台科資工甲、108 台科資工】

$$\text{Figure 1}$$

$$[0,500] \xrightarrow{\quad} [-1,1]$$

$$(0,0) \quad (700,0) \qquad (-1,-1) \quad (1,-1)$$

$$(0,500) \qquad \quad (700,500) \qquad (-1,1) \qquad (1,1)$$

**解**

先考慮縮放矩陣 $A$，則

$$\begin{bmatrix}700&0\\0&500\end{bmatrix}\begin{bmatrix}2\\2\end{bmatrix} \cdot \begin{bmatrix}A&0\\0&2\end{bmatrix} = \begin{bmatrix}2/700&0\\0&2/500\end{bmatrix}$$

然後再平移矩陣為

$$\begin{bmatrix}-1\\-1\end{bmatrix}$$

所以求矩陣為

$$A = \begin{bmatrix}2/700&0&-1\\0&2/500&-1\\0&0&1\end{bmatrix}$$
