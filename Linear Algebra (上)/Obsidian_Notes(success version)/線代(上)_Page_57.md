## 可逆與塊狀矩陣

> **定理：可逆與塊狀矩陣**
>
> (1) 若 $A=\begin{bmatrix} A_{11} & O \\ A_{21} & A_{22} \end{bmatrix}$，且 $A_{11}$，$A_{22}$ 可逆，則
> $A^{-1}=\begin{bmatrix} A_{11}^{-1} & O \\ -A_{22}^{-1}A_{21}A_{11}^{-1} & A_{22}^{-1} \end{bmatrix}$。
>
> 〔109 台聯電機〕
>
> (2) 若 $A=\begin{bmatrix} A_{11} & A_{12} \\ O & A_{22} \end{bmatrix}$，且 $A_{11}$，$A_{22}$ 可逆，則
> $A^{-1}=\begin{bmatrix} A_{11}^{-1} & -A_{11}^{-1}A_{12}A_{22}^{-1} \\ O & A_{22}^{-1} \end{bmatrix}$。
>
> 〔101 中興統計、107 台大資工、108 台大工科〕
>
> (3) 若 $A=\begin{bmatrix} A_{11} & O \\ O & A_{22} \end{bmatrix}$，且 $A_{11}$，$A_{22}$ 可逆，則
> $A^{-1}=\begin{bmatrix} A_{11}^{-1} & O \\ O & A_{22}^{-1} \end{bmatrix}$。

**【證明】**

(1) 今令 $A^{-1}=\begin{bmatrix} P & Q \\ R & S \end{bmatrix}$，則由 $AA^{-1}=I$ 可得

$$
\left\{
\begin{aligned}
A_{11}P &= I\\
A_{11}Q &= O\\
A_{21}P + A_{22}R &= O\\
A_{21}Q + A_{22}S &= I
\end{aligned}
\right.
\qquad
\left\{
\begin{aligned}
P &= A_{11}^{-1}\\
Q &= O\\
R &= -A_{22}^{-1}A_{21}A_{11}^{-1}\\
S &= A_{22}^{-1}
\end{aligned}
\right.
$$

故得 $A^{-1}=\begin{bmatrix} A_{11}^{-1} & O \\ -A_{22}^{-1}A_{21}A_{11}^{-1} & A_{22}^{-1} \end{bmatrix}$

(2) 證明方式與(1)類似，請讀者自行練習。

(3) 由(1)或(2)代入 $A_{12}=A_{21}=O$ 即可。

**Note**

(1) 由(3)可推得若 $c_1 \sim c_n$ 均非零，則 $\mathrm{diag}(c_1,c_2,\ldots,c_n)^{-1}=\mathrm{diag}(c_1^{-1},c_2^{-1},\ldots,c_n^{-1})$。

(2) 上（下）三角矩陣的反矩陣必為上（下）三角。