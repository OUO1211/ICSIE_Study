> **例題 2**
>
> (15%) Let $A_{n \times n} = (a_{ij})$ where $a_{ij} = 1$ for all $i, j$. Find $\text{rank}(A - xI)$ in terms of $x$.
>
> 【101 台大數學、107 高雄師數數理】

解：

$$A - xI = \begin{bmatrix} 1-x & 1 & \cdots & 1 \\ 1 & 1-x & \cdots & 1 \\ \vdots & & \ddots & \vdots \\ 1 & 1 & \cdots & 1-x \end{bmatrix}$$

$$\text{rank}(A - xI) = \text{rank}\begin{bmatrix} 1-x & 1 & \cdots & 1 \\ 1 & 1-x & \cdots & 1 \\ \vdots & & & \vdots \\ 1 & 1 & \cdots & 1-x \end{bmatrix}$$

$$= \text{rank}\begin{bmatrix} n-x & n-x & n-x & \cdots & n-x \\ 1 & 1-x & 1 & \cdots & 1 \\ 1 & 1 & 1-x & \cdots & 1 \\ \vdots & & & \ddots & \vdots \\ 1 & 1 & 1 & \cdots & 1-x \end{bmatrix}$$

$$= \text{rank}\begin{bmatrix} n-x & 1 & \cdots & 1 \\ 0 & -x & \cdots & 0 \\ \vdots & & \ddots & \vdots \\ 0 & 0 & \cdots & -x \end{bmatrix}$$

若 $x \neq n$，則 $\text{rank}(A - xI)$

$$= \text{rank}\begin{bmatrix} 1 & 1 & 1 & \cdots & 1 \\ 1 & 1-x & 1 & \cdots & 1 \\ \vdots & & \ddots & & \vdots \\ 1 & 1 & 1 & \cdots & 1-x \end{bmatrix} \rightarrow \text{rank}\begin{bmatrix} 1 & 1 & \cdots & 1 \\ 0 & -x & \cdots & 0 \\ \vdots & & \ddots & \vdots \\ 0 & 0 & \cdots & -x \end{bmatrix} = n$$

（因為最後這個矩陣有 $n$ 個樞紐位置）

若 $x = n$，

$$\text{rank}(A - xI) = \text{rank}\begin{bmatrix} 0 & 0 & \cdots & 0 \\ 1 & 1-n & \cdots & 1 \\ \vdots & & \ddots & \vdots \\ 1 & 1 & \cdots & 1-n \end{bmatrix} = \text{rank}\begin{bmatrix} 1 & 0 & -n & 0 \\ 1 & -n & 0 & \cdots \\ \vdots & & \ddots & \\ 0 & 0 & \cdots & -n \end{bmatrix}$$

$$\text{rank}(A - xI) = \begin{cases} n-1 & x = n \\ n & x \neq n \end{cases}$$

因為矩陣是 $n \times n$，故 $x \neq 0$，故最後以閉合答 $\text{rank}(A - xI) = \begin{cases} n-1 & x = n \\ n & x \neq n, x = 0 \\ n & \text{else} \end{cases}$
