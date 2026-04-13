> **試題 8**
>
> (12%) Given a basis $\beta = \left\{\begin{bmatrix} 1 \\ 0 \\ 1 \end{bmatrix}, \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}, \begin{bmatrix} 0 \\ 1 \\ 1 \end{bmatrix}\right\}$, $T(0) = \begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix}$, $T\begin{bmatrix} 1 \\ 0 \end{bmatrix} = \begin{bmatrix} 2 \\ 1 \\ 0 \end{bmatrix}$, and $T\begin{bmatrix} 0 \\ 1 \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix}$，determine
>
> (1) $[T]_\beta$
>
> (2) The standard matrix of $T$, and
>
> (3) An explicit formula for $T(x)$.
>
> 【99 中山應數、95 交大資訊、106.108 師範大學、99 台北資工】

> **解**
>
> (1) 由題意知 $[T]_\beta = \begin{bmatrix} 0 & 0 & 1 \\ -1 & 0 & 2 \\ 0 & 2 & 0 \end{bmatrix}$。（直接由定義填入各基底像的座標）
>
> (2) 令 $\beta$ 到 $\beta$ 的座標變換矩陣為 $[I_\beta]_\beta^e$，則 $\beta$ 矩陣為
>
> $$[I_\beta]_\beta^e = \begin{bmatrix} 1 & 1 & 0 \\ 0 & 0 & 1 \\ 1 & 0 & 1 \end{bmatrix}$$
>
> 則由 $\beta$ 到 $\beta$ 的轉移矩陣 $[I_\beta]_e^{\beta}$：
>
> $$\begin{bmatrix} 1 & 1 & 0 \\ 0 & 1 & 0 \\ 1 & 0 & 2 \end{bmatrix} \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 1 \\ 0 & 0 & 1 \end{bmatrix} \to \cdots \to [T]_e = \begin{bmatrix} 1 & 0 & 2 \\ 0 & 2 & -1 \\ 0 & 0 & -1 \end{bmatrix}$$
>
> (3) $T\begin{bmatrix} a \\ b \\ c \end{bmatrix} = \begin{bmatrix} -a+2b+c \\ 2b-c \\ a-c \end{bmatrix}$