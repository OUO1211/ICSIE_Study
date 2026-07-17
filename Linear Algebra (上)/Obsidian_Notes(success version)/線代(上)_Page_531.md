## 540 線性代數(上)

> **例題 4**
>
> (4%) Let $L$ be the linear transformation from $R^3$ to $R^3$ having the following matrix representation with respect to the standard basis:
>
> $$\begin{bmatrix}\cos\theta & 0 & \sin\theta\\0 & 1 & 0\\-\sin\theta & 0 & \cos\theta\end{bmatrix}$$
>
> Find $L(L(L(v)))$,
>
> where $v=\begin{bmatrix}x\\y\\z\end{bmatrix}$. Find the dimension of the kernel space, find a basis for the range space of $L$.
>
> 【96 交大資工】

**解**

此映射為繞 $y$ 軸由 $z$ 向 $x$ 軸旋轉 $\theta$ 角，故連做三次運算其轉角 $3\theta$，

即
$$L\left(L\left(L\left(\begin{bmatrix}x\\y\\z\end{bmatrix}\right)\right)\right)=\begin{bmatrix}\cos 3\theta & 0 & \sin 3\theta\\0 & 1 & 0\\-\sin 3\theta & 0 & \cos 3\theta\end{bmatrix}\begin{bmatrix}x\\y\\z\end{bmatrix}.$$

又因為 $L$ 的矩陣表示的行列式為 $1$，故 $L$ 可逆，故 $\ker(L)=\{0\}$，所以 $\dim(\ker(L))=0$，

又：$\dim(\text{Range}(L))=\dim(R^3)-\dim(\ker(L))=3$ 且 $\text{Range}(L)\subseteq R^3$，

故得 $\text{Range}(L)=R^3$。

故可取 $\left\{\begin{bmatrix}1\\0\\0\end{bmatrix},\begin{bmatrix}0\\1\\0\end{bmatrix},\begin{bmatrix}0\\0\\1\end{bmatrix}\right\}$ 為 $\text{Range}(L)$ 的一組基底。

> **例題 5**
>
> (20%) Suppose that $V$ is a vector space, and three vectors $e_1,e_2,e_3$ form a basis for $V$. Suppose that $L:V\to V$ is a linear transformation such that $L(e_1)=e_2+e_3,\ L(e_2)=e_2,\ \text{and}\ L(e_3)=e_1$. Find the dimension of the space $\{v\in V\mid L(v)=0\}$ and the dimension of the range of $L$. Justify your answer.
>
> 【104 成大統計】

**解**

取 $V$ 的基底：$\beta=\{e_1,e_2,e_3\}$，則 $[L]_\beta=\begin{bmatrix}0 & 0 & 1\\1 & 1 & 0\\1 & 0 & 0\end{bmatrix}$。

則由 $\dim(\text{Im}(L))=\text{rank}(A)=3$，且 $\text{Im}(L)\subseteq V$，故 $\text{Im}(L)=V$，

且 $\dim(\ker(L))=\dim(\ker(A))=0$，故 $\ker(L)=\{0\}$。