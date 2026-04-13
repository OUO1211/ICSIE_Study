## 第 2 章　線性方程組與求解

得原式 $= (-1)^{\frac{n+1}{2}} \cdot (-1)^{\frac{n}{2}} \cdot \det\begin{bmatrix} 1 & \cdots & 1 & 1 & 1 \\ n & \cdots & (2n-2) & (2n-1) & 2n \\ n^2 & \cdots & (2n-2)^2 & (2n-1)^2 & (2n)^2 \\ \vdots & & \vdots & \vdots & \vdots \\ n^n & \cdots & (2n-2)^n & (2n-1)^n & (2n)^n \end{bmatrix}$

再利用 Vandermonde 的結果得

$(-1)^{\frac{n+1}{2}} \cdot (-1)^{\frac{n}{2}} \cdot \left[\prod_{k=0}^{n}(2n-k) - n\right] \cdot \left[\prod_{k=0}^{n}(2n-k) - (n+1)\right] \cdots = (-1)^n \cdot n! \cdot (n-1)! \cdots 1!$

---

> **試題 22**
>
> Using a 3 by 3 matrix, show that the inverse of the triangular matrix is also a triangular matrix.

**解** 設 $A = \begin{bmatrix} a & b & c \\ 0 & d & e \\ 0 & 0 & f \end{bmatrix} = [a_{ij}]$ 為上三角矩陣，則 $\text{adj}(A) = \begin{bmatrix} d_{11} & d_{12} & d_{13} \\ d_{21} & d_{22} & d_{23} \\ d_{31} & d_{32} & d_{33} \end{bmatrix}$，

其中，$d_{ij} = \text{cof}(a_{ji})$。

又 $d_{21} = \text{cof}(a_{12}) = (-1)^{1+2}\begin{vmatrix} 0 & e \\ 0 & f \end{vmatrix} = 0$，$d_{31} = \text{cof}(a_{13}) = (-1)^{1+3}\begin{vmatrix} 0 & d \\ 0 & 0 \end{vmatrix} = 0$，

$d_{32} = \text{cof}(a_{23}) = (-1)^{2+3}\begin{vmatrix} a & b \\ 0 & 0 \end{vmatrix} = 0$，故 $A^{-1} = \dfrac{1}{\det(A)}\begin{bmatrix} d_{11} & d_{12} & d_{13} \\ 0 & d_{22} & d_{23} \\ 0 & 0 & d_{33} \end{bmatrix}$ 為上三角矩陣

而若 $A$ 為下三角，則 $A^T$ 為上三角，故 $(A^T)^{-1} = (A^{-1})^T$ 亦為上三角，

$\therefore A^{-1}$ 為下三角，得證。

---

> **試題 23**
>
> Let $A$ be invertible $n \times n$ matrix with real coefficients. (1) Show that if $\text{adj}(A)$ is symmetric, then $A$ is alsosymmetric. (2) Show that if $\text{adj}(A) = I$，$n \geq 2$，then $A = I$ or $A = -I$.
>
> 【105 中央數學】

**解** (1) $A \cdot \text{adj}(A) = \det(A) \cdot I$ $\therefore A^{-1} = \dfrac{1}{\det(A)} \text{adj}(A)$。

(2) $\because \text{adj}(A)^T = \text{adj}(A)$，

$\therefore (A^{-1})^T = \left(\dfrac{1}{\det(A)}\text{adj}(A)\right)^T = \dfrac{1}{\det(A)}\text{adj}(A)^T = \dfrac{1}{\det(A)}\text{adj}(A) = A^{-1}$，

故 $A^T = (((A^{-1})^T)^{-1}) = (A^{-1})^{-1} = A$。