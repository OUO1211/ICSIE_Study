> **例題 5**
>
> (3%) Let $v_1=\begin{bmatrix} 2 \\ 6 \end{bmatrix}$, $v_2=\begin{bmatrix} 1 \\ 4 \end{bmatrix}$ and $S=\begin{bmatrix} 4 & 1 \\ 2 & 1 \end{bmatrix}$. Find vectors $u_1$ and $u_2$ such that $S$ will be the transition matrix from the ordered basis $\{u_1,u_2\}$ to the ordered basis $\{v_1,v_2\}$.
>
> 【110 中山電機類、105 交大資工】

解：

$u_1=4v_1+2v_2=\begin{bmatrix} 10 \\ 32 \end{bmatrix}$，

$u_2=v_1+v_2=\begin{bmatrix} 3 \\ 10 \end{bmatrix}$

> **例題 6**
>
> (10%) Let $B$, $C$ be two bases for $P_2$. If $B=\{x,1+x,1-x+x^2\}$ and the change-of-basis matrix from $B$ to $C$ is $P_{C \leftarrow B}=\begin{bmatrix} 1 & 0 & 0 \\ 0 & 2 & 1 \\ -1 & 1 & 1 \end{bmatrix}$. Please find $C$.
>
> 【107 台北城市】

解：

$$P_{B \leftarrow C}=(P_{C \leftarrow B})^{-1}=\begin{bmatrix} 1 & 0 & 0 \\ 0 & 2 & 1 \\ -1 & 1 & 1 \end{bmatrix}^{-1}=\begin{bmatrix} 1 & 0 & 0 \\ -1 & 1 & -1 \\ 2 & -1 & 2 \end{bmatrix}$$

$1\cdot x-1(1+x)+2(1-x+x^2)=1-2x+2x^2$，

$0\cdot x+1(1+x)-1(1-x+x^2)=0+2x-x^2$，

$0\cdot x-1(1+x)+2(1-x+x^2)=1-3x+2x^2$，

$\therefore C=\{1-2x+2x^2,\;2x-x^2,\;1-3x+2x^2\}$