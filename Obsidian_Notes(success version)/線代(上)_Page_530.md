## 第 4 章 線性映射 539

> **例題 2**
>
> Let $T: R^{2 \times 2} \to R^{2 \times 2}$ be the linear transformation given by $T(A) = A\begin{bmatrix}1&1\\1&0\end{bmatrix} - \begin{bmatrix}1&1\\0&1\end{bmatrix}A$. Find bases for the kernel (nullspace) and the image of $T$.
>
> 【94,100 整南資工、94 成大應數、中正資工、97 交大資工、103 台大數學甲題】

**解**

$$T\begin{pmatrix}\begin{bmatrix}a&b\\c&d\end{bmatrix}\end{pmatrix} = \begin{bmatrix}a&b\\c&d\end{bmatrix}\begin{bmatrix}1&1\\1&0\end{bmatrix} - \begin{bmatrix}1&1\\0&1\end{bmatrix}\begin{bmatrix}a&b\\c&d\end{bmatrix} = \begin{bmatrix}b-c & a-b-d\\c+d-a & c-b\end{bmatrix}$$

(1) $\ker(T) = \left\{\begin{bmatrix}a&b\\c&d\end{bmatrix} \mid \begin{cases}(a+b)-(a+c)=0\\(c+d)-a=0\\c-b=0\end{cases}\right\}$

$$= \left\{\begin{bmatrix}a&b\\c&d\end{bmatrix} \mid \begin{cases}b-c=0\\(c+d)-a=0\\c-b=0\end{cases}\right\}$$

$$= \left\{\begin{bmatrix}b+d&b\\b&d\end{bmatrix} \mid b,d \in R\right\}$$

$$= \text{span}\left\{\begin{bmatrix}1&1\\1&0\end{bmatrix}, \begin{bmatrix}1&0\\0&1\end{bmatrix}\right\}$$

故可取 $\left\{\begin{bmatrix}1&1\\1&0\end{bmatrix}, \begin{bmatrix}1&0\\0&1\end{bmatrix}\right\}$ 為 $\ker(T)$ 的一組基底。

(2) $\text{Im}(T) = \text{span}\left(T\begin{bmatrix}1&0\\0&0\end{bmatrix}, T\begin{bmatrix}0&1\\0&0\end{bmatrix}, T\begin{bmatrix}0&0\\1&0\end{bmatrix}, T\begin{bmatrix}0&0\\0&1\end{bmatrix}\right)$

$$= \text{span}\left\{\begin{bmatrix}0&1\\-1&0\end{bmatrix}, \begin{bmatrix}1&-1\\0&-1\end{bmatrix}, \begin{bmatrix}-1&0\\1&1\end{bmatrix}, \begin{bmatrix}0&-1\\1&0\end{bmatrix}\right\} = \text{span}\left\{\begin{bmatrix}0&1\\-1&0\end{bmatrix}, \begin{bmatrix}1&-1\\0&-1\end{bmatrix}\right\}$$

故可取 $\left\{\begin{bmatrix}0&1\\-1&0\end{bmatrix}, \begin{bmatrix}1&-1\\0&-1\end{bmatrix}\right\}$ 為 $\text{Im}(T)$ 的一組基底。

> **例題 3**
>
> Define a linear transformation $T(f(x)) = f(2)$ from $R_2[x]$ to $R$. Find a basis for the kernel of $T$.

**解**

$\ker(T) = \{f \in R_2[x] \mid f(2) = 0\} = \{a + bx + cx^2 \mid a, b, c \in R,\ a + 2b + 4c = 0\}$

$= \{(-2b - 4c) + bx + cx^2 \mid b, c \in R\} = \text{span}\{(-2 + x),\ (-4 + x^2)\}$

因為 $(-2 + x)$、$(-4 + x^2)$ 為線性獨立，故可取 $\{-2 + x,\ -4 + x^2\}$ 為 $\ker(T)$ 的一組基底。
