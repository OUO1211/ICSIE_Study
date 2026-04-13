> **例 5**
>
> $$A = \begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix}, \quad B = \begin{bmatrix} a_{11} & a_{13} & a_{12} \\ a_{21}+2a_{31} & a_{23}+2a_{33} & a_{22}+2a_{32} \\ a_{31} & a_{33} & a_{32} \end{bmatrix}$$
>
> $$C = \begin{bmatrix} a_{11}-a_{31}\sin\theta & a_{12}-a_{32}\sin\theta & a_{13}-a_{33}\sin\theta \\ a_{21}-a_{31}\cos\theta & a_{22}-a_{32}\cos\theta & a_{23}-a_{33}\cos\theta \\ a_{31} & a_{32} & a_{33} \end{bmatrix}$$
>
> (1) If $|A|=10$, please find $|B|$.  (2) If $A^{-1}=\begin{bmatrix} \sin\theta & \cos\theta & -1 \\ \cos\theta & \sin\theta & -\sin 2\theta \\ \sin\theta & \cos\theta & 2 \end{bmatrix}$, find $C^{-1}$.
>
> 【109 中山通訊】

**解**

(1) $-10$。

(2) $C^{-1}=\left(\begin{bmatrix} 1 & 0 & -\sin\theta \\ 0 & 1 & -\cos\theta \\ 0 & 0 & 1 \end{bmatrix}\begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix}\right)^{-1}=\begin{bmatrix} \sin\theta & \cos\theta & -1 \\ \cos\theta & \sin\theta & -\sin 2\theta \\ \sin\theta & \cos\theta & 2 \end{bmatrix}\begin{bmatrix} 1 & 0 & \sin\theta \\ 0 & 1 & \cos\theta \\ 0 & 0 & 1 \end{bmatrix}$

$$=\begin{bmatrix} \sin\theta & \cos\theta & 0 \\ \cos\theta & \sin\theta & 0 \\ \sin\theta & \cos\theta & 3 \end{bmatrix}$$