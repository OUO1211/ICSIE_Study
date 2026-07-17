> **例題 2**
>
> (8%) Let $T : P_3 \to P_3$ be the transformation $T(p(x)) = 2p(x) - p'(x)$.
>
> $B = \{3 + 2x + x^2, -x + 2x^2, 1 + x^2\}$. Write down the matrix $T$ with respect to the basis $B$.
>
> 【109 台科資工】

> **解**
>
> $T(3 + 2x + x^2) = 2(3 + 2x + x^2) - (2 + 2x) = 4 + 2x + 2x^2$
>
> $= 1(3 + 2x + x^2) + 0(-x + 2x^2) + 1(1 + x^2)$
>
> $T(-x + 2x^2) = 2(-x + 2x^2) - (-1 + 4x) = 1 - 6x + 4x^2$
>
> $= -\frac{9}{2}(3 + 2x + x^2) - 3(-x + 2x^2) + \frac{29}{2}(1 + x^2)$
>
> $T(1 + x^2) = 2(1 + x^2) - 2x = 2 - 2x + 2x^2$
>
> $= -2(3 + 2x + x^2) - 2(-x + 2x^2) + 8(1 + x^2)$
>
> $$\therefore [T]_B = \begin{bmatrix} 1 & -4.5 & -2 \\ 0 & -3 & -2 \\ 1 & 14.5 & 8 \end{bmatrix}$$

> **例題 3**
>
> (8%) Let $L : P_2 \to P_2$ be a linear transformation satisfying
>
> $L(2t^2 + 3t + 1) = 4t^2 + 3t + 1$
>
> $L(3t^2 + 2) = 6t^2 + 2$
>
> $L(t) = t$
>
> Please find the matrix representing $L$ with respect to
>
> $S = \{2t^2 + 3t + 1, 3t^2 + 2, t\}$ and
>
> $T = \{t - 1, t + 1, t^2 + 1\}$.
>
> 【94 中興資科類題、99 台北統計】

> **解**
>
> $L(2t^2 + 3t + 1) = 4t^2 + 3t + 1 = 3(t - 1) + 0(t + 1) + 4(t^2 + 1),$
>
> $L(3t^2 + 2) = 2(t - 1) - 2(t + 1) + 6(t^2 + 1),$
>
> $L(t) = \frac{1}{2}(t - 1) + \frac{1}{2}(t + 1) + 0(t^2 + 1),$
>
> 故所求為
>
> $$\begin{bmatrix} 3 & 2 & 1/2 \\ 0 & -2 & 1/2 \\ 4 & 6 & 0 \end{bmatrix}$$