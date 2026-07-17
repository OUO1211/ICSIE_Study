> **例題 1**
>
> Compute the following matrices:
>
> (1) $A^{20}$, where $A=\begin{bmatrix} 1 & -3 \\ 1 & 1 \end{bmatrix}$
>
> (2) $A^{100}$, where $A=\begin{bmatrix} 1 & 2 \\ 0 & 1 \end{bmatrix}$
>
> 【110 清大資工】
>
> **解**
>
> (1) $A=\begin{bmatrix} 1 & -3 \\ 1 & 1 \end{bmatrix},\quad A^2=AA=\begin{bmatrix} -2 & -6 \\ 2 & -2 \end{bmatrix},\quad A^3=A^2A=\begin{bmatrix} -8 & 0 \\ 0 & -8 \end{bmatrix}=-8I$
>
> $$\therefore A^{20}=(A^3)^6A^2=(-8I)^6A^2=8^6IA^2=8^6\times\begin{bmatrix} -2 & -6 \\ 2 & -2 \end{bmatrix}=\begin{bmatrix} -2\times 8^6 & -6\times 8^6 \\ 2\times 8^6 & -2\times 8^6 \end{bmatrix}$$
>
> (2) $A^2=AA=\begin{bmatrix} 1 & 2 \\ 0 & 1 \end{bmatrix}\begin{bmatrix} 1 & 2 \\ 0 & 1 \end{bmatrix}=\begin{bmatrix} 1 & 4 \\ 0 & 1 \end{bmatrix}$
>
> $$A^3=A^2A=\begin{bmatrix} 1 & 4 \\ 0 & 1 \end{bmatrix}\begin{bmatrix} 1 & 2 \\ 0 & 1 \end{bmatrix}=\begin{bmatrix} 1 & 6 \\ 0 & 1 \end{bmatrix}$$
>
> 依此類推可得 $A^{100}=\begin{bmatrix} 1 & 200 \\ 0 & 1 \end{bmatrix}$。
>
> **例題 2**
>
> Let $A$ be a matrix given by $A=PQ$, where $P=\begin{bmatrix} 1 \\ 2 \\ 1 \end{bmatrix},\ Q=[2\ -1\ 2]$. Find $A,\ A^2,\ A^{100}$.
>
> **解**
>
> $$A=PQ=\begin{bmatrix} 2 & -1 & 2 \\ 4 & -2 & 4 \\ 2 & -1 & 2 \end{bmatrix}$$
>
> $$A^2=(PQ)(PQ)=P(QP)Q=P[2\ -1\ 2]\begin{bmatrix} 1 \\ 2 \\ 1 \end{bmatrix}Q=P2Q=2(PQ)=2A=\begin{bmatrix} 4 & -2 & 4 \\ 8 & -4 & 8 \\ 4 & -2 & 4 \end{bmatrix}$$
>
> $$A^{100}=\underbrace{(PQ)(PQ)\cdots(PQ)}_{100}=P(QP)^{99}Q=2^{99}PQ=2^{99}A$$
>
> $$=\begin{bmatrix} 2^{100} & -2^{99} & 2^{100} \\ 2^{101} & -2^{100} & 2^{101} \\ 2^{100} & -2^{99} & 2^{100} \end{bmatrix}$$