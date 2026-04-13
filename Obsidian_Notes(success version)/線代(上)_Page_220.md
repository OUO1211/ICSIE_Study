### 特殊矩陣的行列式－塊狀矩陣

> **設 $A,B,C$ 均為方陣，則**
>
> (1) $\det\begin{bmatrix} A & O \\ O & I_n \end{bmatrix}=\det(A)=\det\begin{bmatrix} I_n & O \\ O & A \end{bmatrix}$
>
> (2) $\det\begin{bmatrix} A & C \\ O & I_n \end{bmatrix}=\det(A)=\det\begin{bmatrix} I_n & O \\ C & A \end{bmatrix}$
>
> (3) $\det\begin{bmatrix} A & O \\ C & B \end{bmatrix}=\det(A)\cdot\det(B)$ 【93 交大資工、98 暨南資工】
>
> (4) $\det\begin{bmatrix} A & C \\ O & B \end{bmatrix}=\det(A)\cdot\det(B)$ 【96 暨南資工、102 清大數學、110 交大資工】
>
> (5) $\det\begin{bmatrix} A & O \\ O & B \end{bmatrix}=\det(A)\det(B)$，推廣得
> $$
 \det\begin{bmatrix}
 A_1 & 0 & \cdots & 0 \\
 0 & A_2 & \cdots & 0 \\
 \vdots & \vdots & \ddots & \vdots \\
 0 & 0 & \cdots & A_n
 \end{bmatrix}
 =\det(A_1)\det(A_2)\cdots\det(A_n).
 $$
>
> (6) $\det\begin{bmatrix} A & B \\ B & A \end{bmatrix}=\det(A+B)\cdot\det(A-B)$ 【93 交大資科、99 台大數學】
>
> (7) $\det\begin{bmatrix} I_m & B \\ -C & I_n \end{bmatrix}=\det(I_n+CB)=\det(I_m+BC)$ 【95 中央統計、102 華南應數】

> **Note**
>
> (1)(2) 以降階陣開問題項可得
>
> (3)
> $$
 \because
 \begin{bmatrix} A & O \\ C & B \end{bmatrix}
 =
 \begin{bmatrix} A & O \\ C & I \end{bmatrix}
 \begin{bmatrix} I & O \\ O & B \end{bmatrix},
 \therefore
 \det\begin{bmatrix} A & O \\ C & B \end{bmatrix}
 =
 \det\begin{bmatrix} A & O \\ C & I \end{bmatrix}
 \det\begin{bmatrix} I & O \\ O & B \end{bmatrix}
 =
 \det(A)\cdot\det(B).
 $$>
> (4)
> $$
 \because
 \begin{bmatrix} A & C \\ O & B \end{bmatrix}
 =
 \begin{bmatrix} I & O \\ O & B \end{bmatrix}
 \begin{bmatrix} A & C \\ O & I \end{bmatrix},
 \therefore
 \det\begin{bmatrix} A & C \\ O & B \end{bmatrix}
 =
 \det\begin{bmatrix} I & O \\ O & B \end{bmatrix}
 \det\begin{bmatrix} A & C \\ O & I \end{bmatrix}
 =
 \det(A)\det(B).
 $$
>
> (6)
> $$
 \because
 \begin{bmatrix} I & I \\ O & I \end{bmatrix}
 \begin{bmatrix} A & B \\ B & A \end{bmatrix}
 =
 \begin{bmatrix} A+B & A+B \\ B & A \end{bmatrix},
 $$
 $$\therefore 
\begin{bmatrix} 
I & I \\ 
O & I 
\end{bmatrix} 
\begin{bmatrix} 
A & B \\ 
B & A 
\end{bmatrix} 
\begin{bmatrix} 
I & -I \\ 
O & I 
\end{bmatrix} 
= 
\begin{bmatrix} 
A+B & O \\ 
B & A-B 
\end{bmatrix}$$
> $$
 \therefore
 \det\begin{bmatrix} A+B & O \\ B & A-B \end{bmatrix}
 =
 \det\begin{bmatrix} I & I \\ O & I \end{bmatrix}
 \det\begin{bmatrix} A & B \\ B & A \end{bmatrix}
 \det\begin{bmatrix} I & -I \\ O & I \end{bmatrix}
 =
 \det\begin{bmatrix} A & B \\ B & A \end{bmatrix}.
 $$
 
 > 即 $\det(A+B)\det(A-B)=\det\begin{bmatrix} A & B \\ B & A \end{bmatrix}$
>
> 另一解：$\begin{bmatrix} A & B \\ B & A \end{bmatrix}$ 作列運算（不做交換與倍數）可得 $\begin{bmatrix} A+B & A+B \\ B & A \end{bmatrix}$