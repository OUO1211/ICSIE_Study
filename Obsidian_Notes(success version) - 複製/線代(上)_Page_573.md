## 582 線性代數(上)

> **試題 7**
>
> (10%) Let $V$ be the vector space consisting of all $2 \times 2$ real matrices. Let $\beta$ be the standard ordered basis consisting of $\beta_1, \ldots, \beta_4$ in the order, where
>
> $$\beta_1 = \begin{bmatrix}1&0\\0&0\end{bmatrix},\quad \beta_2 = \begin{bmatrix}0&1\\0&0\end{bmatrix},\quad \beta_3 = \begin{bmatrix}0&0\\1&0\end{bmatrix},\quad \beta_4 = \begin{bmatrix}0&0\\0&1\end{bmatrix}$$
>
> The function $f$ defined by $f(X, Y) = \text{tr}(X) \cdot \text{tr}(Y)$ for any matrices $X$ and $Y$ in $V$ is known to be in bilinear form. What is the matrix representation of the function $f$ in bilinear form with respect to the ordered basis $\beta$? (The answer is a $4 \times 4$ real matrix.)
>
> 【104 台大資工】

**解**

$\text{tr}(\beta_1) = 1$，$\text{tr}(\beta_2) = 0$，$\text{tr}(\beta_3) = 0$，$\text{tr}(\beta_4) = 1$，

$\therefore f(\beta_i, \beta_j) = \text{tr}(\beta_i) \times \text{tr}(\beta_j) = 1, 0, \ldots$

故所求為

$$\begin{bmatrix}f(\beta_1,\beta_1)&f(\beta_1,\beta_2)&f(\beta_1,\beta_3)&f(\beta_1,\beta_4)\\f(\beta_2,\beta_1)&f(\beta_2,\beta_2)&f(\beta_2,\beta_3)&f(\beta_2,\beta_4)\\f(\beta_3,\beta_1)&f(\beta_3,\beta_2)&f(\beta_3,\beta_3)&f(\beta_3,\beta_4)\\f(\beta_4,\beta_1)&f(\beta_4,\beta_2)&f(\beta_4,\beta_3)&f(\beta_4,\beta_4)\end{bmatrix} = \begin{bmatrix}1&0&0&1\\0&0&0&0\\0&0&0&0\\1&0&0&1\end{bmatrix}$$

> **試題 8**
>
> (8%) Give a basis for the vector space of the linear transformations from the vector space $R^3$ of real triples to the vector space $R^2$ of real pairs. 【108 台大資工、95 中山應數】

**解**

考慮 $R^3$ 與 $R^2$ 的基底 $\beta = \left\{\begin{bmatrix}1\\0\\0\end{bmatrix}, \begin{bmatrix}0\\1\\0\end{bmatrix}, \begin{bmatrix}0\\0\\1\end{bmatrix}\right\}$，$\gamma = \left\{\begin{bmatrix}1\\0\end{bmatrix}, \begin{bmatrix}0\\1\end{bmatrix}\right\}$。

考慮函數 $f_1 \sim f_6$ 定義如下：

$f_1(x, y, z) = (x, 0)$，$f_2(x, y, z) = (y, 0)$，$f_3(x, y, z) = (z, 0)$，

$f_4(x, y, z) = (0, x)$，$f_5(x, y, z) = (0, y)$，$f_6(x, y, z) = (0, z)$，

則 $[f_1]_\beta^\gamma = \begin{bmatrix}1&0&0\\0&0&0\end{bmatrix}$，$[f_2]_\beta^\gamma = \begin{bmatrix}0&1&0\\0&0&0\end{bmatrix}$，$[f_3]_\beta^\gamma = \begin{bmatrix}0&0&1\\0&0&0\end{bmatrix}$，

$[f_4]_\beta^\gamma = \begin{bmatrix}0&0&0\\1&0&0\end{bmatrix}$，$[f_5]_\beta^\gamma = \begin{bmatrix}0&0&0\\0&1&0\end{bmatrix}$，$[f_6]_\beta^\gamma = \begin{bmatrix}0&0&0\\0&0&1\end{bmatrix}$，

而因為任意 $R^3$ 到 $R^2$ 的線性映射在矩陣表示都形成 $R^{2 \times 3}$，

這六個向量線性獨立且構成 $R^{2 \times 3}$ 的一組基底，

故 $\{f_1, f_2, f_3, f_4, f_5, f_6\}$ 可為 $L(R^3, R^2)$ 的一組基底。
