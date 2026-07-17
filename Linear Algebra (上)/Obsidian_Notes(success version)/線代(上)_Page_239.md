> **試題 3**
>
> Denote $Z_5$ the finite field of 5 elements, in which the addition/multiplication are the same as in integers except taking modulo 5. Notice that there are exactly $625$ $2 \times 2$ matrices whose entries are in $Z_5$.
>
> (1) Determine the total number of $2 \times 2$ symmetric matrices over $Z_5$.
>
> (2) Determine the total number of nonsingular $2 \times 2$ symmetric matrices over $Z_5$.
>
> (3) Determine the total number of nonsingular $2 \times 2$ matrices over $Z_5$.
>
> (4) For every $n \geq 1$, determine the total number of upper-triangular nonsingular $n \times n$ matrices over $Z_5$.
>
> 【101 台大數學】

**解**

(1) 令 $A = \begin{bmatrix} a & b \\ b & c \end{bmatrix}$，$a, b, c$ 均為 0～4 種元素素可放入，故有 $5^3$ 種對稱矩陣在 $Z_5$。

(2) 令 $A = \begin{bmatrix} a & b \\ b & c \end{bmatrix}$，$\det(A) = ac - b^2$，

$ac = b^2$ 時，分類成 $b^2 = 0, 1, 2, 3, 4$ 加總得 $9 + 8 + 0 + 0 + 8 = 25$ 種。

$\therefore$ 在 $Z_5$ 中，非奇異且對稱矩陣有 $125 - 25 = 100$ 種。

(3) 令 $A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$，$\det(A) = ad - bc$，

$ad = bc$ 時，分類成 $0, 1, 2, 3, 4$，加總得 $9^2 + 4^2 + 4^2 + 4^2 + 4^2 = 145$ 種。

$\therefore$ 在 $Z_5$ 中，非奇異矩陣有 $625 - 145 = 480$ 種。【104 清大數學矩陣】

(4) 對角元素均可 1～4 共 $4^n$ 種變化，

上三角元素共 $1 + 2 + \cdots + (n-1) = \dfrac{n(n-1)}{2}$ 個，每個 5 種變化，

$\therefore$ 非奇異且上三角矩陣有 $4^n \times 5^{n(n-1)/2}$ 種。

---

> **試題 4**
>
> True or false:
>
> (1) (10%) If $A$ and $B$ are $4 \times 4$ real matrices such that $AB = -BA$, then at least one of $A$ and $B$ is not invertible. Prove or disprove this statement.
>
> 【100 台大數學】
>
> (2) If $A$ is invertible, then $A + B$ and $I + BA^{-1}$ are both invertible or both not invertible.
