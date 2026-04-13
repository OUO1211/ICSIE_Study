以下題目用到以下性質：設 $A = PR$，其中 $rank(A) = r$，$P$ 為可逆矩陣，$R$ 為 $A$ 的簡化列梯陣，則 $P$ 的最左邊 $r$ 個列向量可為 $A$ 的行空間的一組基底。 【95 台大電機】

> **例題**
>
> We are given the $LU$ decomposition of $B = LU = \begin{bmatrix} 1 & 0 & 0 & 0 \\ 2 & 1 & 0 & 0 \\ 2 & 1 & 1 & 0 \\ 3 & 2 & 4 & 1 \end{bmatrix} \begin{bmatrix} 1 & 2 & 0 & 1 & 2 & 1 \\ 0 & 0 & 2 & 2 & 0 & 0 \\ 0 & 0 & 0 & 0 & 0 & 1 \\ 0 & 0 & 0 & 0 & 0 & 0 \end{bmatrix}$。
>
> (1) (3%) What is the rank of matrix $B$? Show your work.
>
> (2) (7%) Find a basis for the null space of matrix $B$? Show your work.
>
> (3) (5%) Find a basis for the column space of matrix $B$? Show your work. 【107 成大統計】

**解**

(1) 由題意知 $B$ 可列運算成 $U$，即 $B$ 與 $U$ 列等價，故 $rank(B) = rank(U) = 3$。

(2) 因為 $B$ 與 $U$ 列等價，故

$$
\text{nullspace}(B)=\text{nullspace}(U)
=\left\{
\begin{bmatrix}
a\\
b\\
c\\
d\\
e\\
f
\end{bmatrix}
\middle|
\begin{array}{l}
a+2b+d+2e+f=0\\
2c+2d=0\\
f=0
\end{array}
\right\}
=
\left\{
\begin{bmatrix}
-2b-d-2e\\
b\\
-d\\
d\\
e\\
0
\end{bmatrix}
\middle| b,d,e\in\mathbb{R}
\right\}
$$

$$
=\operatorname{span}\left\{
\begin{bmatrix}
-2\\
1\\
0\\
0\\
0\\
0
\end{bmatrix},
\begin{bmatrix}
-1\\
0\\
-1\\
1\\
0\\
0
\end{bmatrix},
\begin{bmatrix}
-2\\
0\\
0\\
0\\
1\\
0
\end{bmatrix}
\right\}
$$

又因 $S$ 為獨立集，故可成為 $\text{nullspace}(B)$ 的一組基底。

(3) 因為 $rank(B)=3$，故可取 $L$ 的前三列

$$
\begin{bmatrix}
1\\
2\\
2\\
3
\end{bmatrix},
\begin{bmatrix}
0\\
1\\
1\\
2
\end{bmatrix},
\begin{bmatrix}
0\\
0\\
1\\
4
\end{bmatrix}
$$

為 $CS(B)$ 的一組基底。