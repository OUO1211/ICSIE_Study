## 580 線性代數(上)

$$\therefore \mathbf{r}=x\mathbf{e}_x+y\mathbf{e}_y+z\mathbf{e}_z+\mathbf{o}_1$$

$$=x(1\mathbf{e}_u+0\mathbf{e}_v+0\mathbf{e}_w)+y\left(0\mathbf{e}_u+\frac{1}{2}\mathbf{e}_v+\frac{\sqrt{3}}{2}\mathbf{e}_w\right)+z\left(0\mathbf{e}_u-\frac{\sqrt{3}}{2}\mathbf{e}_v+\frac{1}{2}\mathbf{e}_w\right)+1\mathbf{e}_u+2\mathbf{e}_v+1\mathbf{e}_w+\mathbf{o}_2$$

$$=(1x+0y+0z+1)\mathbf{e}_u+\left(0x+\frac{1}{2}y-\frac{\sqrt{3}}{2}z+2\right)\mathbf{e}_v+\left(0x+\frac{\sqrt{3}}{2}y+\frac{1}{2}z+1\right)\mathbf{e}_w+\mathbf{o}_2$$

整理：

$$
\left\{
\begin{aligned}
1x+0y+0z+1&=u\\
0x+\frac{1}{2}y-\frac{\sqrt{3}}{2}z+2&=v\\
0x+\frac{\sqrt{3}}{2}y+\frac{1}{2}z+1&=w\\
1&=1
\end{aligned}
\right.
$$

得

$$
\begin{bmatrix}
1 & 0 & 0 & 1\\
0 & 1/2 & -\sqrt{3}/2 & 2\\
0 & \sqrt{3}/2 & 1/2 & 1\\
0 & 0 & 0 & 1
\end{bmatrix}
\begin{bmatrix}
x\\
y\\
z\\
1
\end{bmatrix}
=
\begin{bmatrix}
u\\
v\\
w\\
1
\end{bmatrix}
$$

$$
\begin{bmatrix}
1 & 0 & 0 & 1\\
0 & 1/2 & -\sqrt{3}/2 & 2\\
0 & \sqrt{3}/2 & 1/2 & 1\\
0 & 0 & 0 & 1
\end{bmatrix}^{-1}
\begin{bmatrix}
u\\
v\\
w\\
1
\end{bmatrix}
=
\begin{bmatrix}
x\\
y\\
z\\
1
\end{bmatrix}
$$

> **試題 5**
>
> Let $f:R^2\times R^2\to R$ be defined by $f(x,y)=x_1y_1+x_2y_2,\ x=\begin{bmatrix}x_1\\x_2\end{bmatrix}\in R^2,\ y=\begin{bmatrix}y_1\\y_2\end{bmatrix}\in R^2$.
>
> Let $\alpha=\left\{\alpha_1=\begin{bmatrix}2\\1\end{bmatrix},\alpha_2=\begin{bmatrix}0\\2\end{bmatrix}\right\}$ be a basis of $R^2$. Further, there exists a Gram matrix of $f$ with respect to $\alpha,\alpha$, such that
>
> $$f\left(\sum_{i=1}^2x_i\alpha_i,\sum_{i=1}^2y_i\alpha_i\right)=[x_1\ x_2]A\begin{bmatrix}y_1\\y_2\end{bmatrix}.$$
>
> (1) Find the Gram matrix of $f$ with respect to the basis $\alpha$.
>
> (2) Use the result obtained from (1) to find $f\left(\begin{bmatrix}3\\-1\end{bmatrix},\begin{bmatrix}1\\2\end{bmatrix}\right)$.
>
> 【98 中正統計】

**解**

(1) $\because f(x,y)=x^Ty$，

$$\therefore f\left(\sum_{i=1}^2x_i\alpha_i,\sum_{i=1}^2y_i\alpha_i\right)=f\left(\begin{bmatrix}2&0\\1&2\end{bmatrix}\begin{bmatrix}x_1\\x_2\end{bmatrix},\begin{bmatrix}2&0\\1&2\end{bmatrix}\begin{bmatrix}y_1\\y_2\end{bmatrix}\right)$$

$$=[x_1\ x_2]\begin{bmatrix}2&1\\0&2\end{bmatrix}\begin{bmatrix}2&0\\1&2\end{bmatrix}\begin{bmatrix}y_1\\y_2\end{bmatrix}$$

$$=[x_1\ x_2]\begin{bmatrix}5&2\\2&4\end{bmatrix}\begin{bmatrix}y_1\\y_2\end{bmatrix}$$

$$\therefore A=\begin{bmatrix}5&2\\2&4\end{bmatrix}$$