> **例 7**
>
> Determine $S=\left\{\begin{bmatrix}1\\1\\5\end{bmatrix},\begin{bmatrix}1\\2\\7\end{bmatrix},\begin{bmatrix}1\\3\\9\end{bmatrix},\begin{bmatrix}2\\4\\11\end{bmatrix}\right\}$ is linearly independent.
>
> 【87 交大資料，95 成大資工網路，108 中山丙數】
	
**解** 將四個矩陣各以列向量對應成矩陣
$$
\begin{bmatrix}
1 & 1 & 1 & 2\\
1 & 2 & 3 & 4\\
5 & 7 & 9 & 11
\end{bmatrix}
$$

列運算後成
$$
\begin{bmatrix}
1 & 1 & 1 & 1\\
0 & 1 & 2 & 3\\
0 & 0 & 0 & 0
\end{bmatrix},
$$

所以 $S$ 是線性相依的。

> **例 8**
>
> 令多項式 $p_1=1-x$，$p_2=5+3x-2x^2$，$p_3=1+3x-x^2$。
>
> (1) (10%) 試說明 $p_1,p_2,p_3$ 是否線性獨立。
>
> (2) (10%) 試寫出 $span(p_1,p_2,p_3)$（由三者所張出的向量空間）。
>
> 【108 交大統計】

**解** (1) 考慮以其係數為列向量所對應的矩陣
$$
\begin{bmatrix}
1 & -1 & 0\\
5 & 3 & -2\\
1 & 3 & -1
\end{bmatrix}
$$
，可列運算成
$$
\begin{bmatrix}
1 & -1 & 0\\
0 & 4 & -1\\
0 & 0 & 0
\end{bmatrix}
$$

故 $p_3$ 可被 $p_1,p_2$ 組合，所以這個集合不是線性獨立的。

(2) 由(1)可得
$$
span\{p_1,p_2,p_3\}=\{a(1-x)+b(4x-x^2)\mid a,b\in\mathbb{R}\}.
$$