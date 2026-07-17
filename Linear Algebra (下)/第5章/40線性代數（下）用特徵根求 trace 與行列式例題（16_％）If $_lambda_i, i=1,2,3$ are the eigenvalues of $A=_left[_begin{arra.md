40

線性代數（下）



用特徵根求 trace 與行列式



例題

（16\％）If $\lambda_i, i=1,2,3$ are the eigenvalues of $A=\left[\begin{array}{ccc}1 & 2 & 0 \\ 2 & 5 & 1 \\ 0 & 1 & 17\end{array}\right]$ ，find $\sum_{i=1}^3 \lambda_i$ and $\prod_{i=1}^3 \lambda_i$ ．

【109 中央統計】

解 因為 $A$ 有特徵根 $\lambda_1, \lambda_2, \lambda_3$ ，

故 $\operatorname{char}_A(x)=\left(\lambda_1-x\right)\left(\lambda_2-x\right)\left(\lambda_3-x\right)$

$$

=-x^3+\left(\lambda_1+\lambda_2+\lambda_3\right) x^2-\left(\lambda_1 \lambda_2+\lambda_3 \lambda_1+\lambda_2 \lambda_3\right) x+\lambda_1 \lambda_2 \lambda_3,

$$



另外， $\operatorname{char}_A(x)=\left|\begin{array}{ccc}1-x & 2 & 0 \\ 2 & 5-x & 1 \\ 0 & 1 & 17-x\end{array}\right|=(1-x)\left|\begin{array}{cc}5-x & 1 \\ 1 & 17-x\end{array}\right|-2\left|\begin{array}{cc}2 & 0 \\ 1 & 17-x\end{array}\right|$

$$

=(1-x)\left(x^2-22 x+84\right)-2(34-2 x)=-x^3+23 x^2-102 x+16,

$$



故得 $\lambda_1+\lambda_2+\lambda_3=23, \lambda_1 \lambda_2 \lambda_3=16$ ．

另解：

$\operatorname{trace}(A)=23=$ 特徵根之和， $\operatorname{det}(A)=16=$ 特徵根之積。



例題 10

Let $A$ be a $3 \times 3$ matrix with eigenvalues $-1,0,1$ ．Compute the determinant of the matrix $A^5+2 A^2+3 I$ ．

解 令 $f(x)=x^5+2 x^2+3$ ，

則 $f(A)$ 的特徵根為 $f(-1), f(0), f(1)$ ，

$$

\therefore \operatorname{det}\left(A^5+2 A^2+3 I\right)=\operatorname{det}(f(A))=f(-1) f(0) f(1)=4 \cdot 3 \cdot 6=72 .

$$