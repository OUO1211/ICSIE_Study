> **試題 12**
>
> Let $g(x) = 3 + x$, $\beta = \{1, x, x^2\}$ and $\gamma = \{x, x+1, x^2-1\}$ be the standard basis for $P_3(R)$.
>
> Define $T: P_3(R) \to P_3(R)$ by $T(f)(x) = f^2 + 2f + U$, $T(f)(x) = 2x + 2$. Compute $[U]_{\beta}^{\gamma} [T]_\gamma^{\beta}$, $[T]_\gamma$, $[U]_\gamma^{\beta}$.
>
> 【99 中山應數、97 中山電信】

> **解**
>
> (1) $U(1) = (0,1,0)$，$U(x) = (1,0,0)$，$U(x^2) = (0,0,1)$，故 $[U]_\beta^e = \begin{bmatrix} 1 & 1 & 1 \\ 2 & 0 & 0 \end{bmatrix}$

---

> **試題 13**
>
> Let $\beta$ be the ordered basis $\{1, x, x^2\}$ for $P_2(R)$. Let $T: P_2 \to P_2$ be the linear transformation such that $T(1) = 3$, $T(x) = 2 + 3x$, $T(x^2) = 1 + 3x^2$. Find $T^4(x+2)$.

> **解**
>
> (1) $T(1) = 1$，$T(x) = 2x$，$T(x^2) = (x+1)^2$，$\therefore [T]_\beta = \begin{bmatrix} 3 & 2 & 0 \\ 0 & 3 & 0 \\ 0 & 0 & 1 \end{bmatrix}$
>
> $[T^4]_\beta = ([T]_\beta)^4 = \begin{bmatrix} 3 & 2 & 0 \\ 0 & 3 & 0 \\ 0 & 0 & 1 \end{bmatrix}^4 = \begin{bmatrix} 205 & 102 & 0 \\ 102 & 52 & 0 \\ 97 & 46 & 16 \end{bmatrix}$
>
> $[T^4(x+2)]_\beta = [T^4]_\beta \cdot [x+2]_\beta = \begin{bmatrix} 205 & 102 & 0 \\ 102 & 52 & 0 \\ 97 & 46 & 16 \end{bmatrix}\begin{bmatrix} 2 \\ 1 \\ 0 \end{bmatrix} = \begin{bmatrix} 512 \\ 256 \\ 240 \end{bmatrix}$
>
> $\therefore T^4(x+2) = 512 + 256x + 240x^2$
