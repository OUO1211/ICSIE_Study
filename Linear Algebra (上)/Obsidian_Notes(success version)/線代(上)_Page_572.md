## 第 4 章 線性映射 581

$$= \left[x_1\; x_2\right]\begin{bmatrix}2&0\\1&2\end{bmatrix}\begin{bmatrix}y_1\\y_2\end{bmatrix} = \left[x_1\; x_2\right]\begin{bmatrix}2&0\\1&2\end{bmatrix}\begin{bmatrix}y_1\\y_2\end{bmatrix}$$

$$\therefore A = \begin{bmatrix}5&2\\2&4\end{bmatrix}$$

(2) $f\left(\begin{bmatrix}3\\-1\end{bmatrix}, \begin{bmatrix}2\\1\end{bmatrix}\right) = \left[3\; -1\right]\begin{bmatrix}2&1\\1&4\end{bmatrix}\begin{bmatrix}2\\1\end{bmatrix} \cdot \begin{bmatrix}2\\1\end{bmatrix} = \left[3\; -1\right]\begin{bmatrix}5\\2\\1\\4\end{bmatrix}\begin{bmatrix}3\\-1\end{bmatrix} = \frac{1}{4}\begin{bmatrix}3\\-1\end{bmatrix} = 1$

> **試題 6**
>
> (10%) Define function $f: R^2 \times R^2 \to R$ as $f(x,y) = x_1 y_1 - x_1 y_2 - x_2 y_1 + 4x_2 y_2$, for any vector $\mathbf{x}$ (respectively, $y$) with standard coordinate $(x_1, x_2)$ (respectively, $(y_1, y_2)$). Let $u = (1,0)$. Find a vector $v$ such that $f(x, v) = x_1 t_1 + x_2 t_2$, where $(x_1, x_2)$ (respectively, $(t_1, t_2)$) is the coordinate of $x$ (respectively, $y$) with respect to the ordered basis of $R^2$ consisting of $u$ and $v$.
>
> 【106 台大資工】

**解**

令所求 $v = (a, b)$，

則 $\mathbf{x} = \begin{bmatrix}x_1\\x_2\end{bmatrix} = x_1\begin{bmatrix}1\\0\end{bmatrix} + x_2\begin{bmatrix}0\\b\end{bmatrix}$，$y = \begin{bmatrix}y_1\\y_2\end{bmatrix} = t_1\begin{bmatrix}1\\0\end{bmatrix} + t_2\begin{bmatrix}0\\b\end{bmatrix}$

$$f(x,y) = x_1 y_1 - x_1 y_2 - x_2 y_1 + 4x_2 y_2 = [x_1\; x_2]\begin{bmatrix}1&-1\\-1&4\end{bmatrix}\begin{bmatrix}y_1\\y_2\end{bmatrix}$$

$$= [x_1\; x_2]\begin{bmatrix}1&0\\a&b\end{bmatrix}\begin{bmatrix}1&-1\\-1&4\end{bmatrix}\begin{bmatrix}1&a\\0&b\end{bmatrix}\begin{bmatrix}t_1\\t_2\end{bmatrix}$$

$$= [s_1\; s_2]\begin{bmatrix}1&a-b\\a-b&a^2-2ab+4b^2\end{bmatrix}\begin{bmatrix}t_1\\t_2\end{bmatrix}$$

而欲使 $f(x,v) = s_1 t_1 + s_2 t_2 = [s_1\; s_2]\begin{bmatrix}1&0\\0&1\end{bmatrix}\begin{bmatrix}t_1\\t_2\end{bmatrix}$，

故解 $\begin{cases}a - b = 0\\ a^2 - 2ab + 4b^2 = 1\end{cases}$，得 $a = b = \pm\dfrac{1}{\sqrt{3}}$，故可取 $v = \left(\dfrac{1}{\sqrt{3}}, \dfrac{1}{\sqrt{3}}\right)$ 或 $v = \left(-\dfrac{1}{\sqrt{3}}, -\dfrac{1}{\sqrt{3}}\right)$。
