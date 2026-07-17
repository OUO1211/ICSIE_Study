## 線性映射的判別

> **定理**
>
> 考慮函數 $T: V \to V'$，則 (1)～(3) 式為等價條件：
>
> (1) $T$ 為線性。
>
> (2) $\forall u, v \in V$，$a \in F$，$T(au + v) = aT(u) + T(v)$。
>
> (3) 對 $V$ 中的任意線性組合 $\sum_{i=1}^n a_i v_i$，$a_i \in F$，$T\left(\sum_{i=1}^n a_i v_i\right) = \sum_{i=1}^n a_i T(v_i)$。

> **Note**
>
> 若 $T: V \to V'$ 為線性映射，則
>
> (1) $T(\mathbf{0}) = \mathbf{0}$。
>
> (2) $T(-v) = -T(v)$。
>
> (3) $\forall u, v \in V$，$T(u - v) = T(u) - T(v)$。
>
> (4) 常用 (1) 與 (2) 做為判斷是否為線性映射的必要條件。

---

> **試題 1**
>
> Determine whether the following transformations are linear.
>
> (1) $T[x_1, x_2, x_3]^T = [x_1 + 1, x_2 - 1, x_3]^T$。【107 中央資工】
>
> (2) $T: R^2 \to R^2$，$T(x, y) = (x + y, x)$。【107 中央資工電機融合、107 台大電機】
>
> (3) $L(\begin{bmatrix} a \\ b \\ c \end{bmatrix}) = a + \sqrt{2}b - c$。
>
> (4) $T: R^2 \to R^2$，$T(x) = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} x$ for any vector $x$ in $R^2$。
>
> (5) $L: R^3 \to R^2$，$L(x) = (x_1 + 2x_2, 3x_2 + x_3)^T$。【108 台北資工】
>
> (6) $L: R^3 \to R^3$，$L(x) = x + a$，其中 $a$ is a constant vector in $R^3$。
>
> (7) $L: R^2 \to R^3$，$L(x) = \begin{bmatrix} (x_1 + x_2)^2 , x_1 + x_2 , x_2\end{bmatrix}^T$。【97、99 成大資工、101 台大電信】

> **解**
>
> (1) 不是線性映射，因為
>
> $$T\left(\begin{bmatrix} 0 \\ 0 \\ 0 \end{bmatrix}\right)=\begin{bmatrix} 1 \\ -1 \\ 0 \end{bmatrix}\neq \begin{bmatrix} 0 \\ 0 \\ 0 \end{bmatrix}。$$
>
> (2) 是線性映射：
>
> $\forall a \in R$，$(b,c),(d,e) \in R^2$，
>
> $$T(a(b,c)+(d,e))=T(ab+d,ac+e)=(ab+d+ac+e,ab+d)$$
>
> $$=(ab+ac,ab)+(d+e,d)=aT(b,c)+T(d,e)。$$
>
> (3) 是線性映射：
>
> $\forall a \in R$，$\begin{bmatrix} b \\ c \\ d \end{bmatrix}, \begin{bmatrix} x \\ y \\ z \end{bmatrix} \in R^3$，
>
> $$L\left(a\begin{bmatrix} b \\ c \\ d \end{bmatrix}+\begin{bmatrix} x \\ y \\ z \end{bmatrix}\right)=L\left(\begin{bmatrix} ab+x \\ ac+y \\ ad+z \end{bmatrix}\right)$$
>
> $$=(ab+x)+\sqrt{2}(ac+y)-(ad+z)$$
>
> $$=a(b+\sqrt{2}c-d)+(x+\sqrt{2}y-z)$$
>
> $$=aL\left(\begin{bmatrix} b \\ c \\ d \end{bmatrix}\right)+L\left(\begin{bmatrix} x \\ y \\ z \end{bmatrix}\right)。$$
>
> (4) 是線性映射。
>
> (5) 是線性映射。
>
> (6) 不是線性映射，當 $a$ 為零向量時才可以。
>
> (7) 不是線性映射，因為
>
> $$L\left(\begin{bmatrix} 2 \\ 0 \end{bmatrix}\right)=\begin{bmatrix} 4 \\ 2 \end{bmatrix}，\quad L\left(\begin{bmatrix} 1 \\ 0 \end{bmatrix}\right)=\begin{bmatrix} 1 \\ 1 \end{bmatrix}，$$
>
> 但
>
> $$L\left(2\begin{bmatrix} 1 \\ 0 \end{bmatrix}\right)\neq 2L\left(\begin{bmatrix} 1 \\ 0 \end{bmatrix}\right)。$$