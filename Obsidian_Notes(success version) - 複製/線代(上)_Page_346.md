> **例題 11**
>
> Let $P_2$ be the vector space of polynomials of degree $\le 2$. Determine which of the following sets are bases for the given vector spaces.
>
> (1) $\{f, g, h\}$，where $f(x) = x^2 + 2x - 1$，$g(x) = x + 3$，$h(x) = x^2 + 3x + 2$，for $P_2$。
>
> (2) $\{f, g, h\}$，where $f(x) = x^2 + 2x - 3$，$g(x) = x^2 - x + 1$，$h(x) = x^2 + x + 1$，for $P_2$。
>
> 【101 台北統計 題組，95 中典資料】

**解**

(1) No.

考慮以其係數列向量所成矩陣 $\begin{bmatrix} 1 & 2 & -1 \\ 0 & 1 & 3 \\ 1 & 3 & 2 \end{bmatrix}$，列運算後可得 $\begin{bmatrix} 1 & 2 & -1 \\ 0 & 1 & 3 \\ 0 & 0 & 0 \end{bmatrix}$，

即 $rank = 2$，

故此三項量為線性相依，故不為基底。

(2) Yes.

考慮以其係數列向量所成矩陣 $\begin{bmatrix} 1 & 2 & -3 \\ 1 & -1 & 1 \\ 1 & 1 & 1 \end{bmatrix}$，列運算後可得 $\begin{bmatrix} 1 & 2 & -3 \\ 0 & -3 & 4 \\ 0 & 0 & 8/3 \end{bmatrix}$，

即 $rank = 3$，

即此三項量為線性獨立，又因 $\dim(P_2) = 3$，為 $P_2$ 的基底。

> **例題 12**
>
> Find a basis of the following subspaces:
>
> (1) $W = \{f(x) \mid \deg(f) \le 3, f(1) = f(-1) = 0\}$。
>
> (2) $W = \{f(x) \mid \deg(f) \le 4, f'(2) = 0\}$。
>
> 【107 中央數學】

**解**

(1) 令 $f(x) = a + bx + cx^2 + dx^3 \in W$，則

$\begin{cases} f(1) = 0: a + b + c + d = 0 \\ f(-1) = 0: a - b + c - d = 0 \end{cases}$，$\begin{cases} a + c = 0 \\ b + d = 0 \end{cases}$

$\therefore W = \{a + bx - ax^2 - bx^3 \mid a, b \in \mathbb{R}\} = \{a(1-x^2) + b(x-x^3) \mid a, b \in \mathbb{R}\}$，

$\therefore S = \{(1-x^2), (x-x^3)\}$ 為線性獨立集，$\therefore$ 取 $S$ 可為 $W$ 的一組基底。

(2) 令 $f(x) = a + bx + cx^2 + dx^3 + ex^4 \in W$，則 $f'(x) = b + 2cx + 3dx^2 + 4ex^3$，

$f \in W \Leftrightarrow b + 4c + 12d + 32e = 0$，

$\therefore W = \{a + (-4c - 12d - 32e)x + cx^2 + dx^3 + ex^4 \mid a, c, d, e \in \mathbb{R}\}$
