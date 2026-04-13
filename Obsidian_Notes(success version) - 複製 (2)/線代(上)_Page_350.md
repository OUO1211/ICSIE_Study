## 求算四大子空間的基底

對矩陣 $A$，利用列運算找出梯形式矩陣 $B$：

> (1) 用 $B$ 的非零列，做為 $RS(A)$ 的一組基底。
>
> (2) 求算 $\ker(B)$ 的基底，即為 $\ker(A)$ 的基底。
>
> (3) 把 $B$ 的 pivot 找出並，對應回 $A$ 的行向量，即為 $CS(A)$ 的基底。
>
> （也可 $A$ 行運算到最簡成梯形 $C$，用 $C$ 的非零行，做為 $CS(A)$ 的一組基底）
>
> (4) $\ker(A) = CS(A)$ 的正交補空間，故找到 $CS(A)$ 的基底都查在向量即為 $L\ker(A)$ 的基底。

> **例題 14**
>
> Given $A = \begin{bmatrix} 2 & 4 & 1 & -1 & 2 \\ -1 & -2 & 3 & 0 & -2 \\ 0 & 0 & 1 & 8 & -4 \\ 0 & 0 & -1 & 1 & 1 \\ 0 & 0 & 0 & -1 & 3 \end{bmatrix}$，find 【99.106 海洋資工】
>
> (1) A basis for the row space of $A$.
>
> (2) A basis for the kernel of $A$.
>
> 【98 中正矩數，99 雲科資工，99 中山應數，97 中正資工，107 中央通訊題組】

**解**

$A = \begin{bmatrix} 2 & 4 & 1 & -1 & 2 \\ -1 & -2 & 3 & 0 & -2 \\ 0 & 0 & 1 & 8 & -4 \\ 0 & 0 & -1 & 1 & 1 \\ 0 & 0 & 0 & -1 & 3 \end{bmatrix} \xrightarrow{\text{列運算}} \begin{bmatrix} 1 & 2 & 0 & 0 & 0 \\ 0 & 0 & 1 & 0 & 0 \\ 0 & 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 0 & 1 \\ 0 & 0 & 0 & 0 & 0 \end{bmatrix} = B$，$rank(A) = 4$。

(1) $\therefore RS(A) = RS(B) = span\{[1\ 2\ 0\ 0\ 0], [0\ 0\ 1\ 0\ 0], [0\ 0\ 0\ 1\ 0], [0\ 0\ 0\ 0\ 1]\}$

可取 $S$ 為 $RS(A)$ 之一基底。

(2) $\ker(A) = \ker(B) = \left\{ \begin{bmatrix} a \\ b \\ c \\ d \\ e \end{bmatrix} \middle| \begin{array}{l} a + 2b = 0 \\ c = 0 \\ d = 0 \\ e = 0 \end{array} \right\} = span\left\{ \begin{bmatrix} 2 \\ -1 \\ 0 \\ 0 \\ 0 \end{bmatrix} \right\}$，可取 $T$ 為 $\ker(A)$ 之一基底。
