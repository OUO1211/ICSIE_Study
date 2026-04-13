## 558 線性代數(上)

> **例題 8**
>
> (8%) Assume that $L$ is a linear transformation system from $R^4$ to $R^3$, where
>
> $$L\begin{pmatrix}x\\y\\z\\w\end{pmatrix}=\begin{pmatrix}x+y+z\\y+z+w\\-y-z-w\end{pmatrix}$$
>
> Please find:
>
> (1) the range of $L$.
>
> (2) the null space of $L$.
>
> (3) Is $L$ one-to-one? Explain why.
>
> (4) Is $L$ onto? Explain why.
>
> 【96 墊南資工類題、108 中山通訊】

**解**

$$L\begin{pmatrix}x\\y\\z\\w\end{pmatrix}=\begin{bmatrix}1&1&1&0\\0&1&1&1\\0&-1&-1&-1\end{bmatrix}\begin{pmatrix}x\\y\\z\\w\end{pmatrix},\ A\ 可列運算成\ \begin{bmatrix}1&0&0&-1\\0&1&1&1\\0&0&0&0\end{bmatrix}$$

(1) $\text{Range}(L)=CS(A)=\text{span}\left\{\begin{pmatrix}1\\0\\0\end{pmatrix},\begin{pmatrix}1\\1\\-1\end{pmatrix}\right\}$。

(2) $\text{Null}(L)=\ker(A)=\left\{\begin{pmatrix}x\\y\\z\\w\end{pmatrix}\mid\begin{cases}x-w=0\\y+z+w=0\end{cases}\right\}=\left\{\begin{pmatrix}w\\-z-w\\z\\w\end{pmatrix}\mid z,w\in R\right\}$

$$=\text{span}\left\{\begin{pmatrix}0\\-1\\1\\0\end{pmatrix},\begin{pmatrix}1\\-1\\0\\1\end{pmatrix}\right\}。$$

(3) $L$ 不是一對一。

(4) $L$ 不是 onto。