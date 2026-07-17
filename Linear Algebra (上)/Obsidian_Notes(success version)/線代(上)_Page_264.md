## 第 3 章　向量空間

> **例題 2**
>
> Determine whether $S$ is a subspace of $V = R^3 - R^4$:
>
> (1) $S = \begin{Bmatrix} \begin{bmatrix} a \\ b \\ c \end{bmatrix} \mid a - b + c = 0 \end{Bmatrix}$。 【106 台大電機領題、102 成大數學、93,101 政大資科】
>
> (2) $S = \{(a, b, c) \mid a = 2b = 3c\}$。 【95 雲科資工、94 中正資工領題、101 政大資科】
>
> (3) $S = \{(x_1, x_2, x_3, x_4) \mid x_2 = 5x_3 - 7x_4\}$。 【101 交大資工】
>
> (4) $S$ is the set of all vectors of the form $(a + 3b, a - 3b, 2a)$。 【101 交大資工】
>
> (5) $S$ is the set of all vectors $(a + b^3)$。 【101 交大資工】
>
> (6) $S = \left\{ \begin{bmatrix} a + 2b + 2c \\ -2b + c \\ a + 3c \end{bmatrix} \mid a, b, c \in R \right\}$。 【103 成大數學】

**解** (1) True.

$\because 0 \in S$，$\therefore S \neq \emptyset$。

$\forall a \in R$，$\begin{bmatrix} x_1 \\ y_1 \\ z_1 \end{bmatrix}$，$\begin{bmatrix} x_2 \\ y_2 \\ z_2 \end{bmatrix} \in S$，$\because x_1 - y_1 + z_1 = 0$，$x_2 - y_2 + z_2 = 0$，

$\therefore (ax_1 + x_2) - (ay_1 + y_2) + (az_1 + z_2) = a(x_1 - y_1 + z_1) + (x_2 - y_2 + z_2) = 0$。

即 $a\begin{bmatrix} y_1 \\ y_1 \\ z_1 \end{bmatrix} + \begin{bmatrix} x_2 \\ y_2 \\ z_2 \end{bmatrix} = \begin{bmatrix} ax_1 + x_2 \\ ay_1 + y_2 \\ az_1 + z_2 \end{bmatrix} \in S$。

(2) True.

(3) True. 可用(1)的方式完成證明，也可由下一小節生成空間的概念：

$S = \{(x_1, 5x_3 - 7x_4, x_3, x_4) \mid x_i \in R\} = \text{span}\{(1, 0, 0, 0), (0, 5, 1, 0), (0, -7, 0, 1)\}$

即為了的生成空間。

(4) True.

(5) True.

(6) True. 可用(1)的方式完成證明，也可之後會提到到矩陣的空間概念：

即為 $S = \left\{ \begin{bmatrix} a + 2b + 2c \\ -2b + c \\ a + 3c \end{bmatrix} \mid a, b, c \in R \right\} = CS\left(\begin{bmatrix} 1 & 2 & 2 \\ 0 & -2 & 1 \\ 1 & 0 & 3 \end{bmatrix}\right)$
