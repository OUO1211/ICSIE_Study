> **例題 4**
>
> (1) (10%) Let $u=\begin{bmatrix}-1,2\end{bmatrix}$, $v=\begin{bmatrix}3,-5\end{bmatrix}$ and $T:R^2 \to R^3$ be a linear transformation such that $T(u)=\begin{bmatrix}-2,1,0\end{bmatrix}$ and $T(v)=\begin{bmatrix}5,-7,1\end{bmatrix}$. Find $T(a,b)$.
>
> (2) (5%) Find a matrix $A$ of the linear transformation $T:R^2 \to R^2$ with $T\left(\begin{bmatrix}3\\1\end{bmatrix}\right)=\begin{bmatrix}6\\2\end{bmatrix}$ and $T\left(\begin{bmatrix}1\\2\end{bmatrix}\right)=2\begin{bmatrix}1\\2\end{bmatrix}$. 【100 台科資工】
>
> (3) (8%) Let $T:R^2 \to R^3$ be a linear transformation such that $T\left(\begin{bmatrix}1\\0\end{bmatrix}\right)=\begin{bmatrix}-2\\1\\3\end{bmatrix}$ and $T\left(\begin{bmatrix}0\\2\end{bmatrix}\right)=\begin{bmatrix}2\\4\\-2\end{bmatrix}$. Determine $T\left(\begin{bmatrix}x_1\\x_2\end{bmatrix}\right)$ for any $\begin{bmatrix}x_1\\x_2\end{bmatrix}$ in $R^3$. 【104 雲科資工、107 師大生工類、109 師大資工】
>
> **解**
>
> (1)
>
> $$T(a,b)=aT(1,0)+bT(0,1)=aT(5u+2v)+bT(3u+v)$$
>
> $$=(5a+3b)T(u)+(2a+b)T(v)$$
>
> $$=(5a+3b)\begin{bmatrix}-2,1,0\end{bmatrix}+(2a+b)\begin{bmatrix}5,-7,1\end{bmatrix}=\begin{bmatrix}-b,-9a-4b,2a+b\end{bmatrix}.$$
>
> (2)
>
> $$T\left(\begin{bmatrix}1\\0\end{bmatrix}\right)=T\left(\frac{2}{5}\begin{bmatrix}3\\1\end{bmatrix}-\frac{1}{5}\begin{bmatrix}1\\2\end{bmatrix}\right)=\frac{2}{5}T\left(\begin{bmatrix}3\\1\end{bmatrix}\right)-\frac{1}{5}T\left(\begin{bmatrix}1\\2\end{bmatrix}\right)=\frac{2}{5}\begin{bmatrix}6\\2\end{bmatrix}-\frac{1}{5}\begin{bmatrix}2\\4\end{bmatrix}=\begin{bmatrix}2\\0\end{bmatrix}$$
>
> $$T\left(\begin{bmatrix}0\\1\end{bmatrix}\right)=T\left(-\frac{1}{5}\begin{bmatrix}3\\1\end{bmatrix}+\frac{3}{5}\begin{bmatrix}1\\2\end{bmatrix}\right)=-\frac{1}{5}T\left(\begin{bmatrix}3\\1\end{bmatrix}\right)+\frac{3}{5}T\left(\begin{bmatrix}1\\2\end{bmatrix}\right)=-\frac{1}{5}\begin{bmatrix}6\\2\end{bmatrix}+\frac{3}{5}\begin{bmatrix}2\\4\end{bmatrix}=\begin{bmatrix}0\\2\end{bmatrix}$$
>
> $$\therefore\ T\left(\begin{bmatrix}x\\y\end{bmatrix}\right)=xT\left(\begin{bmatrix}1\\0\end{bmatrix}\right)+yT\left(\begin{bmatrix}0\\1\end{bmatrix}\right)=x\begin{bmatrix}2\\0\end{bmatrix}+y\begin{bmatrix}0\\2\end{bmatrix}=\begin{bmatrix}2x\\2y\end{bmatrix}=\begin{bmatrix}2&0\\0&2\end{bmatrix}\begin{bmatrix}x\\y\end{bmatrix},$$
>
> 故可取
>
> $$A=\begin{bmatrix}2&0\\0&2\end{bmatrix}.$$
>
> (3)
>
> $$\because\ T\left(\begin{bmatrix}0\\1\end{bmatrix}\right)=T\left(\frac{1}{2}\begin{bmatrix}0\\2\end{bmatrix}\right)=\frac{1}{2}T\left(\begin{bmatrix}0\\2\end{bmatrix}\right)=\frac{1}{2}\begin{bmatrix}2\\4\\-2\end{bmatrix}=\begin{bmatrix}1\\2\\-1\end{bmatrix},$$
>
> $$\therefore\ T\left(\begin{bmatrix}x_1\\x_2\end{bmatrix}\right)=T\left(x_1\begin{bmatrix}1\\0\end{bmatrix}+x_2\begin{bmatrix}0\\1\end{bmatrix}\right)=x_1T\left(\begin{bmatrix}1\\0\end{bmatrix}\right)+x_2T\left(\begin{bmatrix}0\\1\end{bmatrix}\right)=x_1\begin{bmatrix}-2\\1\\3\end{bmatrix}+x_2\begin{bmatrix}1\\2\\-1\end{bmatrix}=\begin{bmatrix}-2x_1+x_2\\x_1+2x_2\\3x_1-x_2\end{bmatrix}.$$