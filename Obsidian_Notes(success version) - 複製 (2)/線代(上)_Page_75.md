> **例題 2**
>
> Find elementary matrices $E_1, E_2, E_3, \ldots$, such that:
>
> (1) $AE_1 E_2 E_3 = L$, where $A = \begin{bmatrix} 0 & 1 & 3 \\ 1 & 2 & 1 \\ 3 & 4 & 2 \end{bmatrix}$, $L$ is a lower triangular.
>
> (2) $A = BE_1 E_2 \cdots E_k$, where $A = \begin{bmatrix} 0 & 3 & 1 \\ 0 & 1 & 0 \\ 4 & 0 & 0 \\ 4 & 0 & 0 \end{bmatrix}$, $B = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \\ 0 & 0 & 1 \end{bmatrix}$
>
> 〔94 成大資工〕
>
> **解：**
>
> (1) $\begin{bmatrix} 0 & 1 & 3 \\ 1 & 2 & 1 \\ 3 & 4 & 2 \end{bmatrix} \xrightarrow{c_{12}} \begin{bmatrix} 1 & 0 & 3 \\ 2 & 1 & 1 \\ 4 & 3 & 2 \end{bmatrix} \xrightarrow{c_{13}^{(-3)}} \begin{bmatrix} 1 & 0 & 0 \\ 2 & 1 & -5 \\ 4 & 3 & -10 \end{bmatrix} \xrightarrow{c_{23}^{(5)}} \begin{bmatrix} 1 & 0 & 0 \\ 2 & 1 & 0 \\ 4 & 3 & 5 \end{bmatrix} = L$
>
> 即 $AC_{12} C_{13}^{(-3)} C_{23}^{(5)} = L$，
>
> 即 $\begin{bmatrix} 0 & 1 & 3 \\ 1 & 2 & 1 \\ 3 & 4 & 2 \end{bmatrix} \begin{bmatrix} 0 & 1 & 0 \\ 1 & 0 & 0 \\ 0 & 0 & 1 \end{bmatrix} \begin{bmatrix} 1 & 0 & -3 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix} \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 5 \\ 0 & 0 & 1 \end{bmatrix} = L$。
>
> (2) $A = \begin{bmatrix} 0 & 3 & 1 \\ 0 & 1 & 0 \\ 4 & 0 & 0 \\ 4 & 0 & 0 \end{bmatrix} \xrightarrow{c_{13}} \begin{bmatrix} 1 & 3 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 4 \\ 0 & 0 & 4 \end{bmatrix} \xrightarrow{c_{12}^{(-3)}} \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 4 \\ 0 & 0 & 4 \end{bmatrix} \xrightarrow{c_3^{(1/4)}} \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \\ 0 & 0 & 1 \end{bmatrix} = B$
>
> 即 $AC_{13} C_{12}^{(-3)} C_3^{(1/4)} = B$。
>
> 即 $A = B(C_3^{(1/4)})^{-1}(C_{12}^{(-3)})^{-1}(C_{13})^{-1} = BC_3^{(4)} C_{12}^{(3)} C_{13}$
>
> $$= \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \\ 0 & 0 & 1 \end{bmatrix} \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 4 \end{bmatrix} \begin{bmatrix} 1 & 3 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix} \begin{bmatrix} 0 & 0 & 1 \\ 0 & 1 & 0 \\ 1 & 0 & 0 \end{bmatrix}$$
>
> $$\qquad E_1 \qquad\qquad E_2 \qquad\qquad E_3$$