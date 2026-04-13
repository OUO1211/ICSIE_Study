> **例題 21**
>
> Find the dimensions of $W_1, W_2, W_1 + W_2, W_1 \cap W_2$.
>
> (1) $W_1 = \left\{ \begin{bmatrix} a+b & 2a+3b \\ b & b \end{bmatrix} \mid a, b \in \mathbb{R} \right\}$，
>
> $W_2 = \left\{ \begin{bmatrix} 0 & a \\ -a+2b & b \end{bmatrix} \mid a, b \in \mathbb{R} \right\}$。 【102 政大資料 題組，106 成大應數】
>
> (2) $W_1 = \left\{ \begin{bmatrix} x & 0 & z \\ 0 & -x & 0 \\ y & 0 & x \end{bmatrix} \mid x, y, z \in \mathbb{R} \right\}$，$W_2 = \left\{ \begin{bmatrix} -a & 0 & b \\ 0 & a & 0 \\ c & 0 & a \end{bmatrix} \mid a, b, c \in \mathbb{R} \right\}$。 【92 清大統計】

**解**

(1)
$$
W_1 = span\left\{ \begin{bmatrix} 1 & 2 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 1 & 3 \\ 1 & 1 \end{bmatrix} \right\}, \quad
W_2 = span\left\{ \begin{bmatrix} 0 & 1 \\ -1 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 \\ 2 & 1 \end{bmatrix} \right\},
$$
$$
W_1 \cap W_2 = \left\{ \begin{bmatrix} 0 & b \\ b & b \end{bmatrix} \mid b \in \mathbb{R} \right\}
= span\left\{ \begin{bmatrix} 0 & 1 \\ 1 & 1 \end{bmatrix} \right\},
$$
$$
\dim(W_1) = 2,\quad \dim(W_2) = 2,\quad \dim(W_1 \cap W_2) = 1,
$$
$$
\therefore \dim(W_1 + W_2) = 2 + 2 - 1 = 3。
$$

或
$$
W_1 + W_2
= span\left\{ \begin{bmatrix} 1 & 2 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 1 & 3 \\ 1 & 1 \end{bmatrix}, \begin{bmatrix} 0 & 1 \\ -1 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 \\ 2 & 1 \end{bmatrix} \right\}
= span\left\{ \begin{bmatrix} 1 & 2 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 1 \\ -1 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 \\ 2 & 1 \end{bmatrix} \right\},
$$
$$
\therefore \dim(W_1 + W_2) = 3。
$$

(2)
$$
W_1 = span\left( \begin{bmatrix} 1 & 0 & 0 \\ 0 & -1 & 0 \\ 0 & 0 & 1 \end{bmatrix}, \begin{bmatrix} 0 & 0 & 0 \\ 0 & 0 & 0 \\ 1 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 & 1 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{bmatrix} \right), \therefore \dim(W_1) = 3。
$$

$$
W_2 = span\left( \begin{bmatrix} -1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}, \begin{bmatrix} 0 & 0 & 1 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 & 0 \\ 0 & 0 & 0 \\ 1 & 0 & 0 \end{bmatrix} \right), \therefore \dim(W_2) = 3。
$$

$$
W_1 + W_2
$$
$$
= span\left( \begin{bmatrix} 1 & 0 & 0 \\ 0 & -1 & 0 \\ 0 & 0 & 1 \end{bmatrix}, \begin{bmatrix} 0 & 0 & 1 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 & 0 \\ 0 & 0 & 0 \\ 1 & 0 & 0 \end{bmatrix}, \begin{bmatrix} -1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}, \begin{bmatrix} 0 & 0 & 1 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 & 0 \\ 0 & 0 & 0 \\ 1 & 0 & 0 \end{bmatrix} \right)
$$
$$
= span\left( \begin{bmatrix} 1 & 0 & 0 \\ 0 & -1 & 0 \\ 0 & 0 & 1 \end{bmatrix}, \begin{bmatrix} 0 & 0 & 1 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 & 0 \\ 0 & 0 & 0 \\ 1 & 0 & 0 \end{bmatrix}, \begin{bmatrix} -1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix} \right),
$$
$$
\therefore \dim(W_1 + W_2) = 4。
$$

$$
\therefore \dim(W_1 \cap W_2) = \dim(W_1) + \dim(W_2) - \dim(W_1 + W_2) = 3 + 3 - 4 = 2。
$$