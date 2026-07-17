# 第一章 矩陣 102

## 線性代數（上）

> **試題 8**
>
> (16%) Let $A = \begin{bmatrix} \cos\alpha & \sin\alpha \\ -\sin\alpha & \cos\alpha \end{bmatrix}$，$B = (I - A)(I + A)^{-1}$，和 $C = (I - B^3)(I + B^3)^{-1}$。
>
> (1) Show that $A^t = A^{-1}$ and hence show that $A$ is invertible.
>
> (2) It is shown that $I + B^3$ and $I - B^3$ are both invertible. Show that $C$ is **orthogonal** (i.e., $CC^T = I$).
>
> 【98 淡江統計】

**解**

(1) $A$ 正交矩陣故 $A^t = A^{-1}$，

故 $\det(A + A) = \det(A^t A) = \det(I) = 1 \neq 0$，故 $(I+A)$ 可逆。

$$\det(I + A) = \det\begin{bmatrix} 1+\cos\alpha & \sin\alpha \\ -\sin\alpha & 1+\cos\alpha \end{bmatrix} = (1+\cos\alpha)^2 + \sin^2\alpha = \frac{(2+2\cos\alpha)}{2} = 2 + 2\cos\alpha$$

先說明 $B$ 也為反對稱矩陣：

$(B^T + B) = ((I-A)(I+A)^{-1})^T + (I-A)(I+A)^{-1}$

$= ((I+A)^{-1})^T (I-A)^T + (I-A)(I+A)^{-1}$

$= (I+A^T)^{-1}(I-A^T) + (I-A)(I+A)^{-1}$

$= (I+A^{-1})^{-1}(I-A^{-1}) + (I-A)(I+A)^{-1}$

先證明 $(I+A^{-1})^{-1}(I-A^{-1}) = -(I-A)(I+A)^{-1}$：

$(I+A^{-1})^{-1}(I-A^{-1})(I-A)(I+A)^{-1}$

$= (I+A^{-1})^{-1}(I-A^{-1})(I-A)(I+A)^{-1}$

$\ldots$

$\therefore CC^T = I$，$C$ 為正交矩陣。