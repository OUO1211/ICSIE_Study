### 可逆與行列式

> **定義**
>
> 方陣 $A$ 為可逆若且唯若 $\det(A) \neq 0$。
>
> 【95 台大資工、99 雲科資工、102 中正應數、108 台聯電機】

【證明】

$\Rightarrow$ 因 $A$ 可逆，故 $A$ 可表為若干個初等基本矩陣的乘積，設 $A = R_1 \cdots R_k$，又因初等基本矩陣的行列式都不為 0，且 $\det(A) = \det(R_1)\cdots\det(R_k)$，故得 $\det(A) \neq 0$。

$\Leftarrow$ 設 $A$ 不可逆，則 $rank(A) < n$，$A$ 的簡化列梯陣為 $B$，且 $A = R_1 \cdots R_k B$，其中，$R_1, \ldots, R_k$ 為初等基本矩陣且 $B$ 有零列，則 $\det(A) = \det(R_1 \cdots R_k B) = \det(R_1) \cdots \det(R_k)\det(B) = 0$（$\because \det(B) = 0$）

> **Note**
>
> 也可記成：$A$ 不可逆 $\Leftrightarrow \det(A) = 0$。

> **例 7**
>
> (10%) Find the values of $x$ such that $\begin{bmatrix} 1 & x & x^2 & x^3 \\ a & 1 & x & x^2 \\ b & c & 1 & x \\ p & q & r & 1 \end{bmatrix}$ is not invertible.
>
> 【109 成大電機】

**解**

$$0 = \begin{vmatrix} 1 & x & x^2 & x^3 \\ a & 1 & x & x^2 \\ b & c & 1 & x \\ p & q & r & 1 \end{vmatrix} = \begin{vmatrix} 1-ax & 0 & 0 & 0 \\ a & 1 & x & x^2 \\ b & c & 1 & x \\ p & q & r & 1 \end{vmatrix} = \begin{vmatrix} 1-ax & 0 & 0 & 0 \\ a-bx & 1-cx & 0 & 0 \\ b & c & 1 & x \\ p & q & r & 1 \end{vmatrix}$$

$$= \begin{vmatrix} 1-ax & 0 & 0 & 0 \\ a-bx & 1-cx & 0 & 0 \\ b-px & c-qx & 1-rx & 0 \\ p & q & r & 1 \end{vmatrix}$$

$= (1-ax)(1-cx)(1-rx)$，

故 $x = \dfrac{1}{a}$，$\dfrac{1}{c}$ 或 $\dfrac{1}{r}$ 時此矩陣不可逆。
