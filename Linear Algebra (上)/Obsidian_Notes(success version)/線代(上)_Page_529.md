## 538 線性代數(上)

## 求核空間與值域

> **例題 1**
>
> Let $L: R^4 \to R^3$ is defined by $L\begin{pmatrix}x\\y\\z\\w\end{pmatrix} = \begin{pmatrix}x+y+z\\z+w\\x+z+2\end{pmatrix}$. Find bases for $\ker(L)$ and $\text{Range}(L)$.

**解**

$$[A] = \begin{bmatrix}1&1&0&0\\0&0&1&1\\1&0&1&0\end{bmatrix}$$

(1) 方法一：$\ker(L) = \ker(A)$，行化簡列梯陣形：

$$\begin{bmatrix}1&0&0&-1\\0&1&0&1\\0&0&1&1\end{bmatrix} \Rightarrow \ker(L) = \text{span}\left\{\begin{pmatrix}1\\-1\\-1\\1\end{pmatrix}\right\} \in R$$

方法二：$\ker(L) = \left\{\begin{pmatrix}a\\b\\c\\d\end{pmatrix} \mid \begin{cases}a+b=0\\c+d=0\\a+c=0\end{cases}\right\} = \left\{\begin{pmatrix}t\\-t\\-t\\t\end{pmatrix} \mid t \in R\right\}$

故可取 $\{(1,-1,-1,1)\}$ 為 $\ker(L)$ 的一組基底。

(2) 方法一：$\text{Range}(L) = CS(A) = \text{span}\left\{A_1, A_2, A_3\right\}$，（因為 $A$ 的簡化列梯陣中 pivot 在第 1,2,3 行）

方法二：$\text{Range}(L) = \text{span}\left(L\begin{pmatrix}1\\0\\0\\0\end{pmatrix}, L\begin{pmatrix}0\\1\\0\\0\end{pmatrix}, L\begin{pmatrix}0\\0\\1\\0\end{pmatrix}, L\begin{pmatrix}0\\0\\0\\1\end{pmatrix}\right)$

$$= \text{span}\left\{\begin{pmatrix}1\\0\\1\end{pmatrix}, \begin{pmatrix}1\\0\\0\end{pmatrix}, \begin{pmatrix}0\\1\\1\end{pmatrix}, \begin{pmatrix}0\\1\\0\end{pmatrix}\right\}$$

方法三：$\because \dim(\text{Range}(L)) = \dim(R^4) - \dim(\ker(L)) = 4 - 1 = 3$，

又 $\text{Range}(L) \subseteq R^3$，故 $\text{Range}(L) = R^3$，

故可取 $R^3$ 的標準基底 $\{e_1, e_2, e_3\}$ 為 $\text{Range}(L)$ 的基底。
