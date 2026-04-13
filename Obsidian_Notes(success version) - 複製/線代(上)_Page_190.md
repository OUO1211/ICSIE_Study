> **例 6**
>
> determinants:
>
> (1) $\det\begin{bmatrix} 1 & 2 & 3 & \cdots & n \\ n+1 & n+2 & n+3 & \cdots & 2n \\ 2n+1 & 2n+2 & 2n+3 & \cdots & 3n \\ \vdots & & & & \vdots \\ (n-1)n+1 & (n-1)n+2 & (n-1)n+3 & \cdots & n^2 \end{bmatrix} = ?$
>
> (2) $\det\begin{bmatrix} x+a & a & \cdots & a \\ a & x+a & \cdots & a \\ \vdots & & \ddots & \vdots \\ a & a & \cdots & x+a \end{bmatrix} = ?$
>
> 【張家齊】

**解**

(1) $n=1$ 時，明顯可得行列式為 1；

$n=2$ 時，明顯可得行列式 $= \begin{vmatrix} 1 & 2 \\ 3 & 4 \end{vmatrix} = -2$；

$n \geq 3$ 時，將第一列乘上 1 與第二列乘上 $(-2)$，一起加到第三列，可使第三列成為零列，故行列式 $= 0$。

(2) 將第 $2, 3, \ldots, n$ 列均加到第 1 列，使成為 $\det\begin{bmatrix} x+na & x+na & \cdots & x+na \\ a & x+a & \cdots & a \\ \vdots & & \ddots & \vdots \\ a & a & \cdots & x+a \end{bmatrix}$，

再將第一列提出 $x+na$，使成為 $\det\begin{bmatrix} 1 & 1 & \cdots & 1 \\ a & x+a & \cdots & a \\ \vdots & & \ddots & \vdots \\ a & a & \cdots & x+a \end{bmatrix}$，

再將第一列乘上 $-a$ 加到各行，則成為 $\det\begin{bmatrix} 1 & 0 & \cdots & 0 \\ 0 & x & \cdots & 0 \\ \vdots & & \ddots & \vdots \\ 0 & 0 & \cdots & x \end{bmatrix} = x^{n-1}$，

故得 $\det = (x+na)x^{n-1}$。
