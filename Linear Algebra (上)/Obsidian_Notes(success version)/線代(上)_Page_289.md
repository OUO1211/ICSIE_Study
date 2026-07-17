> **例題 2**
>
> (10%) Let $S = \begin{Bmatrix} \begin{bmatrix} 1 & 2 \\ 0 & 3 \end{bmatrix}, \begin{bmatrix} 0 & 1 \\ 0 & 1 \end{bmatrix}, \begin{bmatrix} 1 & 3 \\ 0 & 4 \end{bmatrix} \end{Bmatrix}$. Let $c$ be a constant. For what values of $c$ is the matrix $\begin{bmatrix} c^2 & -5c \\ c^2 - 4 & -6 \end{bmatrix}$ in the span of $S$.
>
> 【100 中興資科機難、110 台大工工】

**解**

$\begin{bmatrix} 1 & 2 & 0 & 3 \\ 0 & 1 & 0 & 1 \\ 0 & 1 & 0 & 4 \end{bmatrix} \xrightarrow{\text{化簡}} \begin{bmatrix} 1 & 0 & 0 & 1 \\ 0 & 1 & 0 & 1 \\ 0 & 0 & 0 & -5 & -6 \end{bmatrix}$

只可以取 $c = 2$，才可再經過列運算把矩陣列到最後成零列數。

---

> **例題 3**
>
> Show that the vectors $A_1 = (1, -2, -2, 1)$，$A_2 = (0, 1, 3, 0)$，$A_3 = (1, -1, -1, 1)$ and $B_1 = (0, -1, -1, 0)$，$B_2 = (1, 0, 0, 1)$ span the same linear subspace of $R^4$.
>
> 【97 交大資科】

**方法一：**

$\begin{bmatrix} A_1 \\ A_2 \\ A_3 \end{bmatrix} = \begin{bmatrix} 1 & -2 & -2 & 1 \\ 0 & 1 & 3 & 0 \\ 1 & -1 & -1 & 1 \end{bmatrix} \xrightarrow{r_3 \to r_3 - r_1} \begin{bmatrix} 1 & 0 & 0 & 1 \\ 0 & 1 & 3 & 0 \\ 0 & -1 & -1 & 0 \end{bmatrix} \xrightarrow{} \begin{bmatrix} 1 & 0 & 0 & 1 \\ 0 & 1 & 3 & 0 \\ 0 & 0 & 0 & 0 \end{bmatrix}$

$\therefore \text{span}(\{A_1, A_2, A_3\}) = \text{span}(\{B_1, B_2\})$。

**方法二：**

$\because A_3 = 2B_1 + B_2$，$A_1 = B_1 + A_2 = B_1 + B_2$，$\therefore \{A_1, A_2, A_3\} \subseteq \text{span}(\{B_1, B_2\})$，

故得 $\text{span}(\{A_1, A_2, A_3\}) \subseteq \text{span}(\{B_1, B_2\})$。

又 $B_1 = A_3 - A_1$，$2A_2 + 4A_3 = \cdots$，$\therefore \{B_1, B_2\} \subseteq \text{span}(\{A_1, A_2, A_3\})$，

故得 $\text{span}(\{B_1, B_2\}) \subseteq \text{span}(\{A_1, A_2, A_3\})$，

故得 $\text{span}(\{A_1, A_2, A_3\}) = \text{span}(\{B_1, B_2\})$。
