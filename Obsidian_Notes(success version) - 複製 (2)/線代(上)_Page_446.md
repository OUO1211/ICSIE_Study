> **例題 1**
>
> Determine whether the following transformations are linear.
>
> (1) $T[x_1,x_2,x_3]^T=[x_1+1,x_2-1,x_3]^T$。【107 中央資工】
>
> (2) $T:R^2\to R^2$，$T(x,y)=(x+y,x)$。【107 中央工類、107 台大電機】
>
> (3) $L(a,b,c)^T=a+\sqrt{2}b-c$。
>
> (4) $T:R^2\to R^2$，$T(x)=\begin{bmatrix}1&2\\3&4\end{bmatrix}x$ for any vector $x$ in $R^2$。
>
> (5) $L:R^3\to R^2$，$L(x)=(x_1+2x_2,3x_2+x_3)^T$。【108 台光資工】
>
> (6) $L:R^3\to R^3$，$L(x)=x+a$，where $a$ is a constant vector in $R^3$。
>
> (7) $L:R^2\to R^3$，$L(x)=[(x_1+x_2)^2,x_1+x_2,x_2]^T$。【97.99 成大資工、101 台大電工】

> **解**
>
> (1) 不是線性映射，因為
>
> $$T\begin{bmatrix}0\\0\\0\end{bmatrix}=\begin{bmatrix}1\\-1\\0\end{bmatrix}\ne\begin{bmatrix}0\\0\\0\end{bmatrix}。$$
>
> (2) 是線性映射。
>
> $$\forall \alpha\in R,(a,b),(c,d),T(\alpha(a,b)+(c,d))=T(\alpha a+c,\alpha b+d)$$
>
> $$=(\alpha a+c+\alpha b+d,\alpha a+c)=\alpha(a+b,a)+(c+d,c)=\alpha T(a,b)+T(c,d)。$$
>
> (3) 是線性映射。
>
> $$\forall \alpha\in R,\begin{bmatrix}a\\b\\c\end{bmatrix},\begin{bmatrix}x\\y\\z\end{bmatrix},L\left(\alpha\begin{bmatrix}a\\b\\c\end{bmatrix}+\begin{bmatrix}x\\y\\z\end{bmatrix}\right)=L\begin{bmatrix}\alpha a+x\\ \alpha b+y\\ \alpha c+z\end{bmatrix}$$
>
> $$=(\alpha a+x)+\sqrt{2}(\alpha b+y)-(\alpha c+z)=\alpha(a+\sqrt{2}b-c)+(x+\sqrt{2}y-z)$$
>
> $$=\alpha L\begin{bmatrix}a\\b\\c\end{bmatrix}+L\begin{bmatrix}x\\y\\z\end{bmatrix}。$$
>
> (4) 是線性映射。
>
> (5) 是線性映射。
>
> (6) 不是線性映射，需 $a$ 為零向量才可以。
>
> (7) 不是線性映射，因為
>
> $$L\begin{bmatrix}2\\0\end{bmatrix}=\begin{bmatrix}4\\2\\0\end{bmatrix},L\begin{bmatrix}1\\0\end{bmatrix}=\begin{bmatrix}1\\1\\0\end{bmatrix},L\begin{bmatrix}2\\0\end{bmatrix}\ne 2L\begin{bmatrix}1\\0\end{bmatrix}。$$