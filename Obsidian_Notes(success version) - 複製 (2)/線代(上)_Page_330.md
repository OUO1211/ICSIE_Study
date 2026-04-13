> **例題 4**
>
> (15%) Given $v_1 = (1,1,1)^T$ and $v_2 = (3,-1,4)^T$。
>
> (1) (3%) Do $v_1$ and $v_2$ span $\mathbb{R}^3$？ Explain.
>
> (2) (3%) Let $v_3$ be a third vector in $\mathbb{R}^3$ and set $X = \{v_1, v_2, v_3\}$. What condition(s) would $X$ have to satisfy in order for $v_1$, $v_2$ and $v_3$ form a basis for $\mathbb{R}^3$？
>
> (3) (4%) Find a third vector $v_3$ that will extend the set $X = \{v_1, v_2, v_3\}$ to a basis for $\mathbb{R}^3$。
>
> 【99 中正資工 題組，101 成大資工】

**解**

(1) No，因 $\dim(span\{v_1, v_2\}) = 2 < \dim(\mathbb{R}^3)$。

(2) $X$ 須為線性獨立的集合，才可使 $X$ 為 $\mathbb{R}^3$ 的一組基底。

(3) 例如取 $v_3 = (1,0,0)^T$，則 $\det \begin{bmatrix} 1 & 3 & 1 \\ 1 & -1 & 0 \\ 1 & 4 & 0 \end{bmatrix} = 5 \ne 0$，故 $X$ 為線性獨立的集合。

> **例題 5**
>
> Give the vectors $v_1 = (2,1,3)$，$v_2 = (5,3,1)$，and $v_3 = (1,7,2)$。
>
> (1) Show that they are linearly independent.
>
> (2) Give the space $S$ which they span. What is the dimension of $S$？
>
> (3) Which matrices $M$ have $S$ as their column space？
>
> (4) Given an invertible $n$ by $n$ matrix $A$. Show that $\{Av_1, Av_2, Av_3\}$ is also a basis for $S$。
>
> 【107 台北資工】

**解**

(1) $rank\begin{bmatrix} 2 & 1 & 3 \\ 5 & 3 & 1 \\ 1 & 7 & 2 \end{bmatrix} = rank\begin{bmatrix} 0 & -13 & -1 \\ 0 & -32 & -9 \\ 1 & 7 & 2 \end{bmatrix} = 3$，故 $\{v_1, v_2, v_3\}$ 為獨立集。

(2) 獨立集 $\{v_1, v_2, v_3\} \subseteq \mathbb{R}^3$，且 $\dim(\mathbb{R}^3) = 3$，故 $\{v_1, v_2, v_3\}$ 為 $\mathbb{R}^3$ 的一組基底，即 $span\{v_1, v_2, v_3\} = \mathbb{R}^3 = S$。

(3) 可取 $M = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$，則 $CS(M) = S$。（只要是可逆的 $M$ 均可）

(4) 設 $c_1 Av_1 + \ldots + c_3 Av_3 = 0$，則 $A(c_1 v_1 + \ldots + c_3 v_3) = 0$，

又因 $A$ 可逆，故 $A^{-1}A(c_1 v_1 + \ldots + c_3 v_3) = A^{-1}0$，

即得 $c_1 v_1 + \ldots + c_3 v_3 = 0$，

再由 $\{v_1, \ldots, v_3\}$ 為獨立集，故 $c_1 = \ldots = c_n = 0$，

故證得 $\{Av_1, \ldots, Av_3\}$ 為獨立集，而為 $\mathbb{R}^3$ 的一組基底。
