## 第 4 章 線性映射 583

> **試題 9**
>
> (10%) Let $f_i: R^3 \to R$, $i = 1,2,3$, be given by
>
> $f_1(x,y,z) = x - 2y$, $f_2(x,y,z) = x + y + z$, $f_3(x,y,z) = y - 3z$.
>
> (1) Show that $\{f_1, f_2, f_3\}$ form a basis of the dual space of $R^3$.
>
> (2) Find the dual basis $\{x_1, x_2, x_3\}$.
>
> 【102 成大應數】

**解**

(1) $\because \begin{cases} x - 2y = f_1 \\ x + y + z = f_2 \\ y - 3z = f_3 \end{cases}$，可解得 $x = \dfrac{-f_1 - 2f_2}{5}$，$y = \dfrac{-3f_1 - f_2}{5}$，$z = \dfrac{4f_1 + 5f_2 + 3f_3}{5}$。

$\therefore f(x,y,z) = ax + by + cz = a \cdot \dfrac{-f_1-2f_2}{5} + b \cdot \dfrac{-3f_1-f_2}{5} + c \cdot \dfrac{4f_1+5f_2+3f_3}{5}$

$= \dfrac{1}{5}(-a-3b+4c)f_1 + \dfrac{1}{5}(-2a-b+5c)f_2 + \dfrac{1}{5}(-2a-b+3c)f_3$

$\therefore \{f_1, f_2, f_3\}$ 可為 $R^3$ 的對偶空間的一組基底。

(2) 令 $\{x_1, x_2, x_3\}$ 為 $R^3$ 的基底，對偶基底為 $\{f_1, f_2, f_3\}$，

則：$f(x_i) = \delta_{ij}$，即

$$x_1 = \dfrac{1}{5}(-1,-3,4),\quad x_2 = (0,0,1),\quad x_3 = \dfrac{1}{5}(-2,-1,3)$$

因為 $(-2+x)$, $(-4+x^2)$ 為線性獨立，即所求二元基底為 $\dfrac{1}{5}(-1,-3,4)$, $(0,0,1)$, $\dfrac{1}{5}(-2,-1,3)$。

> **試題 10**
>
> (20%) Fix a matrix $A \in M_{n \times n}(R)$ and let $T: M_{n \times n}(R) \to M_{n \times n}(R)$ be the linear operator defined by $T(M) = AM$ for all $M \in M_{n \times n}(R)$. (1) Prove that $T$ is an isomorphism if and only if the matrix $A$ is invertible. (2) Show that $\text{rank}(T) = n \cdot \text{rank}(A)$.
>
> 【102 師大數學】

**解**

(1) $\{v_1, \ldots, v_k\} \in \ker(T) \Leftrightarrow 0 \Leftrightarrow A\mathbf{v}_i = 0$，$\forall i$，

$\therefore T$ 為同構映射 $\Leftrightarrow \ker(T) = \{0\} \Leftrightarrow A$ 可逆。

(2) 設 $\dim(\ker(A)) = n - k$，則 $\text{rank}(A) = n - k$，

且 $\dim(\ker(T)) = nk$，故 $\text{rank}(T) = n^2 - nk = n(n-k) = n \cdot \text{rank}(A)$。
