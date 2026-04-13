## 第 2 章　線性方程組與求解

而得 $\det(D_n)=\det\begin{bmatrix} \dfrac{1}{2} & \dfrac{1}{3} & \cdots & \dfrac{1}{n} \\ \dfrac{1}{3} & \dfrac{1}{4} & \cdots & \dfrac{1}{n+1} \\ \vdots & \vdots & & \vdots \\ \dfrac{1}{n} & \dfrac{1}{n+1} & \cdots & \dfrac{1}{2n-2} \end{bmatrix}=\det(P_{n-1})$

故得 $\det(P_n)=\dfrac{(n!)^2((n-1)!)^2}{(2n-1)!(2n)!}\times\det(P_{n-1})$，

故 $\dfrac{\det(P_{n+1})}{\det(P_n)}=\dfrac{((n+1)!)^2(n!)^2}{(2n)!(2n+1)!}$

---

> **試題 12**
>
> If $F(x)=\det\begin{bmatrix} 1 & x & x^2 & x^3 \\ 0 & 1 & 2x & 3x^2 \\ 0 & 0 & 2 & 3 \\ 1 & e^x & e^{2x} & e^{3x} \end{bmatrix}$, calculate the derivate $F'(x)$.

**解** $F(x)=\det\begin{bmatrix} 1 & x & x^2 & x^3 \\ 0 & 1 & 2x & 3x^2 \\ 0 & 0 & 2 & 3 \\ 1 & e^x & e^{2x} & e^{3x} \end{bmatrix}=\begin{vmatrix} 1 & 2x & 3x^2 \\ 0 & 2 & 3 \\ e^x & 2e^{2x} & 3e^{3x} \end{vmatrix}-\begin{vmatrix} x & x^2 & x^3 \\ 1 & 2x & 3x^2 \\ 0 & 2 & 3 \end{vmatrix}=2e^{3x}-3e^{2x}+3x^2-2x^3,$

$\therefore F'(x)=6e^{3x}-6e^{2x}+6x-6x^2.$

---

> **試題 13**
>
> If $F(x)=\begin{vmatrix} f_1(x) & f_2(x) & f_3(x) \\ f_1'(x) & f_2'(x) & f_3'(x) \\ f_1''(x) & f_2''(x) & f_3''(x) \end{vmatrix}$, find $F'(x)$ in term of a 3 by 3 determinant.

**解** $F'(x)=\begin{vmatrix} f_1(x) & f_2(x) & f_3(x) \\ f_1'(x) & f_2'(x) & f_3'(x) \\ f_1'''(x) & f_2'''(x) & f_3'''(x) \end{vmatrix}$