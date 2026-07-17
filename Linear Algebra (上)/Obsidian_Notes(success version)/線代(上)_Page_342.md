> **例題 10**
>
> True or False: There exists a $2 \times 2$ matrix $A$ such that the space of all matrices commuting with $A$ is two dimensional.
>
> 【105 台科資工】

**解**

True. 令 $A = \begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}$。

$$W = \left\{ B = \begin{bmatrix} a & c \\ b & d \end{bmatrix} \mid AB = BA \right\} = \left\{ \begin{bmatrix} a & c \\ b & d \end{bmatrix} \begin{bmatrix} a & 0 \\ 0 & 0 \end{bmatrix} = \begin{bmatrix} a & 0 \\ 0 & 0 \end{bmatrix} \begin{bmatrix} a & c \\ b & d \end{bmatrix} \right\} = \left\{ \begin{bmatrix} a & 0 \\ 0 & d \end{bmatrix} \mid a, d \in \mathbb{R} \right\}$$

$\dim(W) = 2$。
