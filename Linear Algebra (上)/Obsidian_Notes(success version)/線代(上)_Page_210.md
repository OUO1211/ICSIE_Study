### 特殊矩陣的行列式－三斜矩陣

> **例 13**
>
> $$\Leftrightarrow A_{n \times n} = \begin{bmatrix} 2 & 1 & & \\ 1 & 2 & 1 & \\ & 1 & \ddots & 1 \\ & & \ddots & 2 & 1 \\ & & & 1 & 2 \end{bmatrix}$$，左證 $\det(A_{n \times n}) = n + 1$。

**解** 令 $a_n = \det(A_{n \times n})$，時候展開階後：

$$a_n = 2 \cdot \begin{vmatrix} 2 & 1 & & \\ 1 & 2 & 1 & \\ & 1 & \ddots & 1 \\ & & \ddots & 2 & 1 \\ & & & & 1 & 2 \end{vmatrix}_{(n-1)\times(n-1)} - 1 \cdot \begin{vmatrix} 1 & 2 & 1 & \\ & 1 & \ddots & \\ & & \ddots & 2 & 1 \\ & & & & 1 & 2 \end{vmatrix}_{(n-1)\times(n-1)}$$

$$= 2a_{n-1} - 1 \cdot \begin{vmatrix} 1 & & \\ 1 & 2 & 1 \\ & \ddots & \\ & & 1 & 2 \end{vmatrix}_{(n-2)\times(n-2)} = 2a_{n-1} - a_{n-2}$$

$a_n = 2a_{n-1} - a_{n-2}$，$n \geq 3$。

又，明顯可得 $a_1 = 2$，$a_2 = 3$，故 $a_n = 2a_{n-1} - a_{n-2}$，$n \geq 3$，$a_1 = 2$，$a_2 = 3$。

再對 $n$ 以歸納法證之：

$n = 1$ 時 $\det(A_1) = a_1 = 2 = 1 + 1$ 成立。

$n = 2$ 時 $\det(A_2) = a_2 = 3 = 2 + 1$ 成立。

設 $n \leq k$ 時 $a_n = n + 1$，

則 $a_{k+1} = 2a_k - a_{k-1} = 2(k+1) - k = k + 2$ 亦成立。

故由數學歸納法 $a_n = n + 1$，$\forall n \geq 1$。
