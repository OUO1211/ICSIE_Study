# 第一章 矩陣 103

$= (I+B^T)^{-1}(I-B^T)(I-B)(I+B)^{-1}$

$= (I+B^T)^{-1}(I-B^T-B^T B + B^T \cdot B)(I+B)^{-1}$

$= (I+B^T)^{-1}(I-B^T)(I-B^T)^{-1}(I+B^T)^{-1}$

先證明 $(-XY)(1-X)(1+Y)^{-1}$、$(-B^T)(I+B^T)^{-1}(I-B) = I$：

$(I+X)^{-1}(I-X)+(I-Y)(I+Y)^{-1}$，

$(I+X)(I-X) = (I-X^2)$，$(I-Y)(I+Y) = (I-Y^2)$，

$\ldots (I+B^T)^{-1}(I-B^T)(I-B^T)^{-1}(I+B^T)^{-1} = I$。

> **試題 9**
>
> Consider a system of the form $\begin{pmatrix} A & a \\ c^T & \beta \end{pmatrix} \begin{pmatrix} x \\ x_{n+1} \end{pmatrix} = \begin{pmatrix} b \\ b_{n+1} \end{pmatrix}$, where $A$ is a nonsingular $n \times n$ matrix and $a$, $b$ and $c$ are vectors. (1) Multiply both side of the system by a matrix to obtain an equivalent triangular system. (2) Set $y = A^{-1}a$ and $z = A^{-1}b$. Show that if $\beta - c^T y \neq 0$, then the solution of the system is given by $x_{n+1} = \dfrac{b_{n+1} - c^T z}{\beta - c^T y}$, $x = z - x_{n+1}y$.
>
> 【89 中興總數‧98 中正統計】

**解**

(1) 設 $\begin{bmatrix} M & p \\ q^T & r \end{bmatrix} = \begin{bmatrix} I & 0 \\ 0^T & 1 \end{bmatrix}$，則得 $\begin{cases} MA + pc^T = I \\ Ma = p \cdot \beta p = 0 \\ q^T a + r\beta = 1 \\ q^T a + r\beta = 1 \end{cases}$

可解出 $M = A^{-1} + \dfrac{A^{-1} a c^T A^{-1}}{\beta - c^T A^{-1} a}$，

故故題等式兩邊左乘以 $\begin{bmatrix} A^{-1} + \dfrac{A^{-1} a c^T A^{-1}}{\beta - c^T A^{-1} a} & \dfrac{-A^{-1} a}{\beta - c^T A^{-1} a} \\ \dfrac{-c^T A^{-1}}{\beta - c^T A^{-1} a} & \dfrac{1}{\beta - c^T A^{-1} a} \end{bmatrix}$ 可使成為三角矩陣。

(2) 由題意得 $\begin{cases} Ax + ax_{n+1} = b \\ c^T x + \beta x_{n+1} = b_{n+1} \end{cases}$

可解得 $x = A^{-1}b - x_{n+1}A^{-1}a = z - x_{n+1}y$，$x_{n+1} = \dfrac{b_{n+1} - c^T z}{\beta - c^T y}$。

> **試題 10**
>
> (10%) Let $L = \begin{bmatrix} A & B \\ B^T & C \end{bmatrix}$ where $A$ and $C$ have the inverse. Let $L^{-1} = \begin{bmatrix} E & F \\ F^T & G \end{bmatrix}$. Write $E$ and $G$ in terms of $A$, $B$, and $C$.
>
> 【101 中央統計】

**解**

$\because \begin{bmatrix} I & O \\ -B^T A^{-1} & I \end{bmatrix} \begin{bmatrix} A & B \\ B^T & C \end{bmatrix} \begin{bmatrix} I & -A^{-1}B \\ O & I \end{bmatrix} = \begin{bmatrix} A & O \\ O & C - B^T A^{-1}B \end{bmatrix}$，$\ldots (*)$
