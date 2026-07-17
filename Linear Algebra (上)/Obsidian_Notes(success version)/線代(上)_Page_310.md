## 判斷相依或獨立－Wronskian

令 $C^{n-1}[a,b]$ 為所有在閉區間 $[a,b]$ 上 $n-1$ 次可微的函數所成的向量空間。

設 $f_1, f_2, \ldots, f_n \in C^{n-1}[a,b]$，

定義其 $f_1, f_2, \ldots, f_n$ 的

$$W(f_1, f_2, \ldots, f_n) = \det \begin{bmatrix} f_1(x) & f_2(x) & \cdots & f_n(x) \\ f_1'(x) & f_2'(x) & \cdots & f_n'(x) \\ \vdots & \vdots & & \vdots \\ f_1^{(n-1)}(x) & f_2^{(n-1)}(x) & \cdots & f_n^{(n-1)}(x) \end{bmatrix}$$

稱為 $f_1, f_2, \ldots, f_n$ 的 Wronskian。

> **Note**
>
> (1) 若存在 $x_0 \in [a,b]$，使得 $W(f_1, f_2, \ldots, f_n)|_{x=x_0} \ne 0$，則 $f_1, f_2, \ldots, f_n$ 為線性獨立。
>
> **【證明】**
>
> 設純量 $\alpha_1, \alpha_2, \ldots, \alpha_n$ 使得 $\alpha_1 f_1(x) + \alpha_2 f_2(x) + \cdots + \alpha_n f_n(x) = 0$，
>
> 對其左右式分別微分可得：
>
> $\alpha_1 f_1'(x) + \alpha_2 f_2'(x) + \cdots + \alpha_n f_n'(x) = 0$
>
> $\alpha_1 f_1''(x) + \alpha_2 f_2''(x) + \cdots + \alpha_n f_n''(x) = 0$
>
> $\vdots$
>
> $\alpha_1 f_1^{(n-1)}(x) + \alpha_2 f_2^{(n-1)}(x) + \cdots + \alpha_n f_n^{(n-1)}(x) = 0$
>
> $$\begin{bmatrix} f_1(x) & f_2(x) & \cdots & f_n(x) \\ f_1'(x) & f_2'(x) & \cdots & f_n'(x) \\ \vdots & \vdots & & \vdots \\ f_1^{(n-1)}(x) & f_2^{(n-1)}(x) & \cdots & f_n^{(n-1)}(x) \end{bmatrix} \begin{bmatrix} \alpha_1 \\ \alpha_2 \\ \vdots \\ \alpha_n \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \\ \vdots \\ 0 \end{bmatrix}$$（令 $Ax = 0$）
>
> 而若存在 $x_0 \in [a,b]$ 使 $\det(A) \ne 0$，則此線性系統有唯一解 $\begin{bmatrix} \alpha_1 \\ \alpha_2 \\ \vdots \\ \alpha_n \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \\ \vdots \\ 0 \end{bmatrix}$，
>
> 即 $f_1(x), f_2(x), \ldots, f_n(x)$ 為線性獨立。
>
> (2) 上述性質的逆命題不成立：
>
> 取 $f_1 = x^2$，$f_2(x) = x|x|$，定義在閉區間 $[-1, 1]$，
>
> 則 $W\{f_1, f_2\} = \det \begin{bmatrix} x^2 & x|x| \\ 2x & 2|x| \end{bmatrix} = 0$，但 $\{f_1, f_2\}$ 為獨立集。
