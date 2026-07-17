> **試題 1**
>
> Let $L: R^2 \to R^3$ be a linear transformation. Assume $L\begin{bmatrix} 1 \\ 2 \end{bmatrix} = \begin{bmatrix} 3 \\ 0 \\ 1 \end{bmatrix}$ and $L\begin{bmatrix} 2 \\ 3 \end{bmatrix} = \begin{bmatrix} 5 \\ 1 \\ 3 \end{bmatrix}$. In addition, $B_1 = \left\{\begin{bmatrix} 1 \\ 2 \end{bmatrix}, \begin{bmatrix} 2 \\ 3 \end{bmatrix}\right\}$ is an ordered basis of $R^2$, and $B_2 = \left\{\begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}, \begin{bmatrix} 1 \\ 1 \\ 0 \end{bmatrix}, \begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix}\right\}$, $B_3 = \left\{\begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}, \begin{bmatrix} 5 \\ 1 \\ 3 \end{bmatrix}, \begin{bmatrix} 3 \\ 0 \\ 1 \end{bmatrix}\right\}$ are ordered basis of $R^3$.
>
> (1) (4%) Find the matrix representation of $L$ with respect to the bases $B_1$ and $B_3$.
>
> (2) (4%) Find the coordinate transition matrix from the basis $B_2$ to the basis $B_3$.
>
> (3) Solve $L\begin{bmatrix} 1 \\ 0 \end{bmatrix}$ and $L\begin{bmatrix} 0 \\ 1 \end{bmatrix}$.
>
> (4) Find the standard matrix representing $L$.
>
> 【99 政大統計、104 交大資訊】

> **解**
>
> (1)
>
> $$L\begin{bmatrix} 1 \\ 2 \end{bmatrix}=\begin{bmatrix} 3 \\ 0 \\ 1 \end{bmatrix}=0\cdot\begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}+0\cdot\begin{bmatrix} 5 \\ 1 \\ 3 \end{bmatrix}+1\cdot\begin{bmatrix} 3 \\ 0 \\ 1 \end{bmatrix},$$
>
> $$L\begin{bmatrix} 2 \\ 3 \end{bmatrix}=\begin{bmatrix} 5 \\ 1 \\ 3 \end{bmatrix}=0\cdot\begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}+1\cdot\begin{bmatrix} 5 \\ 1 \\ 3 \end{bmatrix}+0\cdot\begin{bmatrix} 3 \\ 0 \\ 1 \end{bmatrix}.$$
>
> $$\therefore [L]_{B_1}^{B_3}=\begin{bmatrix} 0 & 0 \\ 0 & 1 \\ 1 & 0 \end{bmatrix}.$$
>
> (2)
>
> $$[I_{R^3}]_{B_3}^{B_2}=([I_{R^3}]_{B_2}^{B_3})^{-1}=\begin{bmatrix} 1 & 5 & 3 \\ 0 & 1 & 0 \\ 0 & 3 & 1 \end{bmatrix}^{-1}=\cdots=\begin{bmatrix} 1 & 4 & -3 \\ 0 & 1 & 0 \\ 0 & -3 & 1 \end{bmatrix}.$$
>
> (3)
>
> $$L\begin{bmatrix} 1 \\ 0 \end{bmatrix}=L\left(-3\begin{bmatrix} 1 \\ 2 \end{bmatrix}+2\begin{bmatrix} 2 \\ 3 \end{bmatrix}\right)=-3L\begin{bmatrix} 1 \\ 2 \end{bmatrix}+2L\begin{bmatrix} 2 \\ 3 \end{bmatrix}=-3\begin{bmatrix} 3 \\ 0 \\ 1 \end{bmatrix}+2\begin{bmatrix} 5 \\ 1 \\ 3 \end{bmatrix}=\begin{bmatrix} 1 \\ 2 \\ 3 \end{bmatrix},$$
>
> $$L\begin{bmatrix} 0 \\ 1 \end{bmatrix}=L\left(2\begin{bmatrix} 1 \\ 2 \end{bmatrix}-\begin{bmatrix} 2 \\ 3 \end{bmatrix}\right)=2L\begin{bmatrix} 1 \\ 2 \end{bmatrix}-L\begin{bmatrix} 2 \\ 3 \end{bmatrix}=2\begin{bmatrix} 3 \\ 0 \\ 1 \end{bmatrix}-\begin{bmatrix} 5 \\ 1 \\ 3 \end{bmatrix}=\begin{bmatrix} 1 \\ -1 \\ -1 \end{bmatrix}.$$
>
> (4)
>
> 由 (3) 得 $L$ 的標準矩陣表示為
>
> $$\begin{bmatrix} 1 & 1 \\ 2 & -1 \\ 3 & -1 \end{bmatrix}.$$