> **試題 6**
>
> (15%) Let $u_1 = \begin{bmatrix} 3 \\ 1 \end{bmatrix}$, $u_2 = \begin{bmatrix} 5 \\ 2 \end{bmatrix}$, and let $L$ be the linear operator that rotates vectors in $R^2$ by 45° in the counterclockwise direction. Find the matrix representation of $L$ with respect to the ordered basis $\{u_1, u_2\}$.
>
> 【96 台科台電電機融合、102.104 成大資工】

> **解**
>
> 令 $\beta = \{e_1, e_2\}$ 為 $R^2$ 上的標準基底，則 $[L]_\beta = \begin{bmatrix} \cos 45° & -\sin 45° \\ \sin 45° & \cos 45° \end{bmatrix} = \frac{\sqrt{2}}{2}\begin{bmatrix} 1 & -1 \\ 1 & 1 \end{bmatrix}$。
>
> 令 $\gamma = \{u_1, u_2\}$，則 $\beta$ 到 $\gamma$ 的轉移矩陣為 $P = \begin{bmatrix} 3 & 5 \\ 1 & 2 \end{bmatrix}$。
>
> $\therefore L$ 在 $\gamma$ 下的矩陣表示為 $[L]_\gamma = P^{-1}[L]_\beta P = \begin{bmatrix} 3 & 5 \\ 1 & 2 \end{bmatrix}^{-1} \cdot \frac{\sqrt{2}}{2}\begin{bmatrix} 1 & -1 \\ 1 & 1 \end{bmatrix} \cdot \begin{bmatrix} 3 & 5 \\ 1 & 2 \end{bmatrix}$

---

> **試題 7**
>
> Let $T: P^2 \to P^2$ be given by $T(p(x)) = p(x-1)$. Consider the two ordered bases $\beta = \{x^2, x, 1\}$ and $\gamma = \{x, x+1, x^2-1\}$.
>
> (1) (6%) Find $[T]_\beta$ and $[T]_\gamma$.
>
> (2) (6%) Find the matrix $S$ such that $[T]_\gamma = S[T]_\beta S^{-1}$.
>
> 【110 政大資料】

> **解**
>
> $T(x^2) = (x-1)^2 = x^2 - 2x + 1$，$\therefore [T]_\beta = \begin{bmatrix} 1 & 0 & 0 \\ -2 & 1 & 0 \\ 1 & -1 & 1 \end{bmatrix}$
>
> $T(x) = x-1$，$T(1) = 1$
>
> $T(x^2-1) = (x-1)^2 - 1 = x^2 - 2x$，$\therefore [T]_\gamma = \begin{bmatrix} 2 & 1 & -3 \\ -1 & 0 & 1 \\ 0 & 0 & 1 \end{bmatrix}$
>
> (2) 取 $\beta$ 到 $\gamma$ 的轉移矩陣 $S = \begin{bmatrix} -1 & 1 & 1 \\ 1 & 0 & 0 \\ 0 & 0 & 1 \end{bmatrix}$，可使 $[T]_\gamma = S[T]_\beta S^{-1}$。
