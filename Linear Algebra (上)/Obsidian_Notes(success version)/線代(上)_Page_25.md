> **例題 5**
>
> (12%) For the matrix
>
> $$A = \begin{bmatrix} 1 & 0 & 0 & \frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\ 0 & 1 & 0 & \frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\ 0 & 0 & 1 & \frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\ 0 & 0 & 0 & \frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\ 0 & 0 & 0 & \frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\ 0 & 0 & 0 & \frac{1}{3} & \frac{1}{3} & \frac{1}{3} \end{bmatrix}$$
>
> Determine $A^{300}$.
>
> **解：**
>
> 令 $B = \dfrac{1}{3}\begin{bmatrix} 1 & 1 & 1 \\ 1 & 1 & 1 \\ 1 & 1 & 1 \end{bmatrix}$，則
>
> $$B^2 = BB = \begin{bmatrix} 3 & 3 & 3 \\ 3 & 3 & 3 \\ 3 & 3 & 3 \end{bmatrix} \cdot \frac{1}{9} = B, \ldots, B^n = B \text{，對任何 } n \geq 2$$
>
> 故 $A = \begin{bmatrix} I & B \\ 0 & B \end{bmatrix}$，
>
> 且 $A^2 = \begin{bmatrix} I & B \\ 0 & B \end{bmatrix}\begin{bmatrix} I & B \\ 0 & B \end{bmatrix} = \begin{bmatrix} I & B+B^2 \\ 0 & B^2 \end{bmatrix} = \begin{bmatrix} I & 2B \\ 0 & B \end{bmatrix}$
>
> $A^3 = \begin{bmatrix} I & 2B \\ 0 & B \end{bmatrix}\begin{bmatrix} I & B \\ 0 & B \end{bmatrix} = \begin{bmatrix} I & B+2B^2 \\ 0 & B^2 \end{bmatrix} = \begin{bmatrix} I & 3B \\ 0 & B \end{bmatrix}$
>
> $\ldots$
>
> 故 $A^{300} = \begin{bmatrix} I & 300B \\ 0 & B \end{bmatrix} = \begin{bmatrix} 1 & 0 & 0 & 100 & 100 & 100 \\ 0 & 1 & 0 & 100 & 100 & 100 \\ 0 & 0 & 1 & 100 & 100 & 100 \\ 0 & 0 & 0 & \frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\ 0 & 0 & 0 & \frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\ 0 & 0 & 0 & \frac{1}{3} & \frac{1}{3} & \frac{1}{3} \end{bmatrix}$
