> **試題 14**
>
> (9+5%) Let $T: P_1 \to P_1$ be the linear operator defined by $T(p(t)) = p(2t+5)$, that is, $T(a + bt + ct^2) = a + b(2t+5) + c(2t+5)^2$.
>
> (1) (5%) Find the matrix $T$ with respect to the basis $B = \{1, t, t^2\}$.
>
> (2) (5%) Is $T$ one-to-one? If so, find the matrix for $T^{-1}$ with respect to the basis $B$.
>
> 【94 政大資工、99 客委統計、102 台南大學機電融合、101 中正應數】

> **解**
>
> (1) $T(1) = 1$，$T(t) = 5 + 2t$，$T(t^2) = (2t+5)^2 = 4t^2 + 20t + 25$
>
> $$\therefore [T]_B = \begin{bmatrix} 1 & 5 & 25 \\ 0 & 2 & 20 \\ 0 & 0 & 4 \end{bmatrix}$$
>
> (2) 因為 $\det([T]_B) = 8 \neq 0$，故 $T$ 為 one-to-one。
>
> 又 $[T^{-1}]_B = ([T]_B)^{-1} = \begin{bmatrix} 1 & -\frac{5}{2} & \frac{25}{4} \\ 0 & \frac{1}{2} & -\frac{5}{2} \\ 0 & 0 & \frac{1}{4} \end{bmatrix}$
>
> $T^{-1}(a + bt + ct^2) = \left(a - \frac{5}{2}b + \frac{25}{4}c\right) + \left(\frac{1}{2}b - \frac{5}{2}c\right)t + \frac{1}{4}ct^2$
