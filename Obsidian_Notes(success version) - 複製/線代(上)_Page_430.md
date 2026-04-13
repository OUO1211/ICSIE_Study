## 空間的直和(direct sum)

考慮向量空間 $V$，$W_1, W_2, \ldots, W_k \subseteq V$，

若 $V = W_1 + W_2 + \cdots + W_k$，且 $W_1, W_2, \ldots, W_k$ 為獨立子空間，

則稱 $W_1, W_2, \ldots, W_k$ 形成 $V$ 的一組直和，並記成 $V = W_1 \oplus W_2 \oplus \cdots \oplus W_k$。

> **Note**
>
> (1) 例如，取 $V = R^3$，$W_1 = x$-軸，$W_2 = y$-軸，$W_3 = z$-軸，則 $V = W_1 \oplus W_2 \oplus W_3$。
>
> (2) 設 $V = F^{n \times n}$，$\begin{cases} W_1 = \{A \in V \mid A^T = A\} \\ W_2 = \{A \in V \mid A^T = -A\} \end{cases}$，則 $V = W_1 \oplus W_2$。

> **故任一個方陣必可表成一個對稱矩陣與一個斜對稱矩陣的和！**

> **【證明】**
>
> (a) 先證 $V = W_1 + W_2$：
>
> 已知 $W_1 + W_2 \subseteq V$，又任取 $A \in V$，因為 $= \underbrace{\frac{A+A^T}{2}}_{B} + \underbrace{\frac{A-A^T}{2}}_{C} ,$，
>
> 且 $B^T = \dfrac{A^T + (A^T)^T}{2} = B$，故 $B \in W_1$，又 $C^T = \dfrac{A^T - (A^T)^T}{2} = \dfrac{A^T - A}{2} = -C$，
>
> 故 $C \in W_2$，得 $A \in W_1 + W_2$，
>
> $\therefore V \subseteq W_1 + W_2$，得 $V = W_1 + W_2$。
>
> (b) 再證 $W_1 \cap W_2 = \{0\}$：
>
> 任取 $A \in W_1 \cap W_2$
>
> 由 $A \in W_1$，$\therefore A = A^T$
>
> 由且 $A \in W_2$，$\therefore A = -A^T$
>
> $\therefore A = -A$，得 $A = O$，故 $W_1 \cap W_2 = \{0\}$。
>
> 故得證 $V = W_1 \oplus W_2$。

> **(3) 設 $V = \{f \mid f: R \to R\}$，$\begin{cases} W_1 = \{f \in V \mid f(-x) = f(x)\} \\ W_2 = \{f \in V \mid f(-x) = -f(x)\} \end{cases}$，則 $V = W_1 \oplus W_2$。**
>
> 【86.97 成大應數、92 交大資料、94 暨南資工、99 台大數學】

> **故任一函數必可表成一個奇函數與一個偶函數的和！**

> **【證明】**
>
> $\forall f \in V$，$f(x) = \dfrac{f(x) + f(-x)}{2}$（令為 $f_e(x)$）$+ \dfrac{f(x) - f(-x)}{2}$（令為 $f_o(x)$），
>
> $\therefore f_e(-x) = \dfrac{f(-x) + f(x)}{2} = f_e(x)$，$\therefore f_e(x) \in W_1$，
>
> $f_o(-x) = \dfrac{f(-x) - f(x)}{2} = -f_o(x)$，$\therefore f_o(x) \in W_2$。