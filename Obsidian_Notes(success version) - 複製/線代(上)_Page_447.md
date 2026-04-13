> **例題 2**
>
> Determine whether the following transformations are linear.
>
> (1) $T: M_{22} \to M_{22}$，$T(A)=A^T$。【90 成大資科、95 中興資科、99 中正數學】
>
> (2) $T: M_{2\times 2} \to M_{2\times 2}$，$T\left(\begin{bmatrix} a & b \\ c & d \end{bmatrix}\right)=\begin{bmatrix} a+b & 0 \\ 0 & c+d \end{bmatrix}$
>
> (3) $T: R^{n\times n} \to R$，$T(A)=\operatorname{tr}(A)$，$\forall A \in R^{n\times n}$
>
> (4) $T: M_{22} \to R$，$T(A)=\det(A)$。【107 高師應數、109 成大電通】
>
> (5) $T: M_{22} \to M_{22}$，$T(A)=A^2$。
>
> (6) $L$ is defined on $R^{n\times n}$，$L(A)=e^A$。【97.99 成大資工、107 中央資工】
>
> **解**
>
> (1) 是線性映射，
>
> $\forall \alpha,\forall A,B \in M_{22},T(\alpha A+B)=(\alpha A+B)^T=\alpha A^T+B^T=\alpha T(A)+T(B)$。
>
> (2) 是線性映射，
>
> $\forall \begin{bmatrix} a & b \\ c & d \end{bmatrix},\begin{bmatrix} w & x \\ y & z \end{bmatrix}\in M_{2\times 2}(R),\alpha \in R,$
>
> $$T\left(\alpha \begin{bmatrix} a & b \\ c & d \end{bmatrix}+\begin{bmatrix} w & x \\ y & z \end{bmatrix}\right)=T\left(\begin{bmatrix} \alpha a+w & \alpha b+x \\ \alpha c+y & \alpha d+z \end{bmatrix}\right)$$
>
> $$=\begin{bmatrix} (\alpha a+w)+(\alpha b+x) & 0 \\ 0 & (\alpha c+y)+(\alpha d+z) \end{bmatrix}$$
>
> $$=\alpha \begin{bmatrix} a+b & 0 \\ 0 & c+d \end{bmatrix}+\begin{bmatrix} w+x & 0 \\ 0 & y+z \end{bmatrix}=\alpha T\left(\begin{bmatrix} a & b \\ c & d \end{bmatrix}\right)+T\left(\begin{bmatrix} w & x \\ y & z \end{bmatrix}\right)$$
>
> (3) 是線性映射，
>
> $\forall A,B \in R^{n\times n},\alpha \in R,T(\alpha A+B)=\operatorname{tr}(\alpha A+B)=\alpha \operatorname{tr}(A)+\operatorname{tr}(B)=\alpha T(A)+T(B)$
>
> 故 $T$ 為 $R^{n\times n}$ 上的線性算子
>
> (4) 不是線性映射，
>
> $$T\left(\begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}+\begin{bmatrix} 0 & 0 \\ 0 & 1 \end{bmatrix}\right)=\det\left(\begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}\right)=1,$$
>
> 但
>
> $$T\left(\begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}\right)+T\left(\begin{bmatrix} 0 & 0 \\ 0 & 1 \end{bmatrix}\right)=0+0=0。$$
>
> (5) 不是線性映射，
>
> $$T\left(\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}\right)=\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}^2=\begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix},$$
>
> 但
>
> $$T\left(\begin{bmatrix} 0 & 2 \\ 2 & 0 \end{bmatrix}\right)=\begin{bmatrix} 0 & 2 \\ 2 & 0 \end{bmatrix}^2=\begin{bmatrix} 4 & 0 \\ 0 & 4 \end{bmatrix}\ne 2T\left(\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}\right)。$$
>
> (6) 不是線性映射，
>
> 因為 $L(A+B)=e^{A+B},L(A)=e^A,L(B)=e^B,L(A+B)\ne L(A)+L(B)$。