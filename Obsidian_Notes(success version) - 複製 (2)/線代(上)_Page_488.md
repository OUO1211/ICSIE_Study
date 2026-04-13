## 一般化的座標變換公式

> **定理**
>
> 令 $\beta=\{b_1,b_2,\ldots,b_n\}$，$\beta'=\{b_1',b_2',\ldots,b_m'\}$ 分別為 $V$、$V'$ 之基底，$T\in L(V,V')$，則 $\forall v\in V$，
>
> $$[T(v)]_{\beta'}=[T]_{\beta}^{\beta'}[v]_{\beta}$$

> **Note**
>
> (1) 當 $V=V'$，$\beta=\beta'$ 時，則得 $[T(v)]_{\beta}=[T]_{\beta}[v]_{\beta}$。
>
> (2) 當 $V=V'$，$T$ 取成 $V$ 上的恆位映射 $I$ 時，則得 $[T]_{\beta}^{\beta'}=[I]_{\beta}^{\beta'}=P$。

> **例題 5**
>
> Let $A=\begin{bmatrix}-3&0&-1\\0&-2&0\\-1&0&-3\end{bmatrix}$. If $A$ is the matrix representing the linear transformation $L:P_2\to P_2$ with respect to the basis $\beta=\{t^2+1,t,t-1\}$, please compute $L(t^2+t+1)$.
>
> 【100.106 台北統計】

> **解**
>
> $(t^2+t+1)=1(t^2+1)+1t+0(t-1)$，$\therefore [(t^2+t+1)]_{\beta}=\begin{bmatrix}1\\1\\0\end{bmatrix}$
>
> $$\therefore [L(t^2+t+1)]_{\beta}=[L]_{\beta}\cdot[(t^2+t+1)]_{\beta}=\begin{bmatrix}-3&0&-1\\0&-2&0\\-1&0&-3\end{bmatrix}\begin{bmatrix}1\\1\\0\end{bmatrix}=\begin{bmatrix}-3\\-2\\-1\end{bmatrix}$$
>
> $$\therefore L(t^2+t+1)=-3(t^2+1)-2t-1(t-1)=-3t^2-3t-2$$